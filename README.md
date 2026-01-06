# LETZ Data Dashboard

Simple data dashboard for monitoring user activities and product insights.

## Setup

1. **Create virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure database:** 
   The `.env` file should already be set up with your database credentials.

## Running the Dashboard

```bash
streamlit run dashboard.py
```

The dashboard will open at `http://localhost:8501`

## Features

- **Quick Insights**: Overview metrics (total users, new signups, active users)
- **Predefined Queries**: Common queries ready to run
- **Database Explorer**: Browse tables and schemas in the sidebar

---

## Database Schema Reference

### Core Tables

#### `users`
Main user profile table. **Important:** Users may have duplicate rows—always deduplicate by `waid` (WhatsApp ID).

| Column | Type | Description |
|--------|------|-------------|
| `id` | integer | Auto-increment primary key |
| `waid` | text | **WhatsApp ID** — unique identifier per user. Use `DISTINCT waid` for accurate counts |
| `full_name` | text | User's display name |
| `gender` | text | User's gender (e.g., "male", "female") |
| `pillar` | text | Health pillar the user is focused on (e.g., "nutrition", "sleep", "exercise") |
| `goal` | text | User's specific health goal |
| `level` | text | User's experience/progression level |
| `phase` | text | Current journey phase (e.g., onboarding phase number) |
| `is_active` | boolean | Whether user is currently active |
| `timezone` | text | User's timezone (formats: "UTC-3", "America/Sao_Paulo", etc.) |
| `created_at` | timestamp | When the user record was created |
| `onboarding_timestamp` | timestamp | When user completed onboarding |

**Deduplication pattern:**
```sql
-- Get unique users (most recent record per waid)
SELECT DISTINCT ON (waid) *
FROM users
ORDER BY waid, created_at DESC
```

---

#### `messages`
WhatsApp message log between users and the bot.

| Column | Type | Description |
|--------|------|-------------|
| `id` | integer | Primary key |
| `user_id` | integer | FK to `users.id` |
| `sender` | text | Message direction: `"user"` or `"bot"` |
| `type` | text | Message type (text, image, etc.) |
| `message` | jsonb | Raw message payload (complex JSON structure — see parsing notes) |
| `sent_at` | timestamp | When the message was sent |
| `status` | text | Delivery status |

**Message JSON parsing:** The `message` column contains nested JSON. Common structures:
- `{"flows": {"body": {"text": "..."}}}` — Flow messages
- `{"quickReply": {"body": {"text": "..."}}}` — Quick reply messages
- `{"postback": {"payload": {"text": "...", "value": "..."}}}` — Button clicks
- `{"interactive": {"button_reply": {"title": "..."}}}` — Interactive buttons
- `{"image": {...}}`, `{"audio": {...}}`, `{"document": {...}}` — Media messages

**Useful patterns:**
```sql
-- Get user-sent messages (exclude bot messages)
SELECT * FROM messages WHERE sender = 'user';

-- Daily active users (who sent messages)
SELECT DATE(sent_at), COUNT(DISTINCT user_id) 
FROM messages 
WHERE sender = 'user' 
GROUP BY DATE(sent_at);
```

---

#### `events`
Tracks significant user actions/events in the journey.

| Column | Type | Description |
|--------|------|-------------|
| `id` | integer | Primary key |
| `user_id` | integer | FK to `users.id` |
| `event_type` | text | Event category (see common types below) |
| `description` | text | Additional event details |
| `executed_at` | timestamp | When the event occurred |
| `created_at` | timestamp | When the record was created |

**Common `event_type` values:**
- `onboarding_completed` — User finished onboarding
- `complete_activity` — User completed an activity
- `update_experience` — User earned XP
- `settings_updated` — User changed settings

**Funnel analysis:**
```sql
-- User journey conversion rates
SELECT 
    event_type,
    COUNT(DISTINCT user_id) as users
FROM events
WHERE event_type IN ('onboarding_completed', 'complete_activity', 'update_experience')
GROUP BY event_type;
```

---

#### `user_activities`
Tracks user progress on specific activities.

| Column | Type | Description |
|--------|------|-------------|
| `id` | integer | Primary key |
| `user_id` | integer | FK to `users.id` |
| `activity` | text | Activity name/identifier |
| `completed` | boolean | Whether activity is complete |
| `progress` | numeric/integer | Progress percentage or count |
| `days` | jsonb | Scheduled days array, e.g., `["Monday", "Wednesday"]` |
| `created_at` | timestamp | When activity was assigned |
| `last_activity_at` | timestamp | Most recent activity on this item |

**Querying JSONB days:**
```sql
-- Users scheduled for Monday
SELECT * FROM user_activities 
WHERE days::jsonb ? 'Monday';

-- Count users per day
SELECT 
    COUNT(CASE WHEN days::jsonb ? 'Monday' THEN 1 END) as monday_users,
    COUNT(CASE WHEN days::jsonb ? 'Tuesday' THEN 1 END) as tuesday_users
FROM user_activities;
```

---

#### `milestones`
Milestone definitions (reference table).

| Column | Type | Description |
|--------|------|-------------|
| `id` | integer | Primary key |
| `milestone` | text | Milestone name |
| `type` | text | Milestone category |

---

#### `user_milestones`
Junction table tracking which milestones users have reached.

| Column | Type | Description |
|--------|------|-------------|
| `id` | integer | Primary key |
| `user_id` | integer | FK to `users.id` |
| `milestone_id` | integer | FK to `milestones.id` |
| `completed` | boolean | Whether milestone is achieved |
| `created_at` | timestamp | When milestone was reached |

**Milestone completion rates:**
```sql
SELECT 
    m.milestone,
    COUNT(CASE WHEN um.completed THEN 1 END) as completed,
    COUNT(*) as total
FROM user_milestones um
JOIN milestones m ON um.milestone_id = m.id
GROUP BY m.milestone;
```

---

## Common Query Patterns

### User Counts (Always Deduplicate!)
```sql
-- ❌ WRONG: May count duplicate user records
SELECT COUNT(*) FROM users;

-- ✅ CORRECT: Count unique WhatsApp IDs
SELECT COUNT(DISTINCT waid) FROM users;
```

### Active Users
```sql
-- Users who sent messages in the last 7 days
SELECT COUNT(DISTINCT u.waid)
FROM messages m
JOIN users u ON m.user_id = u.id
WHERE m.sender = 'user'
  AND m.sent_at >= NOW() - INTERVAL '7 days';
```

### Cohort Analysis (by Signup Date)
```sql
SELECT 
    DATE(u.created_at) as cohort_date,
    COUNT(DISTINCT u.waid) as signups,
    COUNT(DISTINCT CASE WHEN e.event_type = 'onboarding_completed' THEN u.waid END) as completed_onboarding
FROM users u
LEFT JOIN events e ON e.user_id = u.id
GROUP BY DATE(u.created_at)
ORDER BY cohort_date DESC;
```

### User Segments by Pillar
```sql
SELECT 
    pillar,
    COUNT(DISTINCT waid) as users,
    ROUND(100.0 * COUNT(DISTINCT waid) / SUM(COUNT(DISTINCT waid)) OVER (), 1) as pct
FROM users
WHERE pillar IS NOT NULL
GROUP BY pillar
ORDER BY users DESC;
```

### Message Activity Heatmap
```sql
SELECT 
    EXTRACT(DOW FROM sent_at) as day_of_week,  -- 0=Sun, 6=Sat
    EXTRACT(HOUR FROM sent_at) as hour,
    COUNT(*) as messages
FROM messages
WHERE sent_at IS NOT NULL
GROUP BY 1, 2
ORDER BY 1, 2;
```

### Retention (Day 1, Day 7, Day 30)
```sql
WITH user_cohorts AS (
    SELECT DISTINCT ON (waid) 
        waid, 
        id as user_id, 
        DATE(created_at) as signup_date
    FROM users
    ORDER BY waid, created_at
)
SELECT 
    uc.signup_date,
    COUNT(DISTINCT uc.waid) as cohort_size,
    COUNT(DISTINCT CASE WHEN m.sent_at::date = uc.signup_date + 1 THEN uc.waid END) as d1,
    COUNT(DISTINCT CASE WHEN m.sent_at::date = uc.signup_date + 7 THEN uc.waid END) as d7,
    COUNT(DISTINCT CASE WHEN m.sent_at::date = uc.signup_date + 30 THEN uc.waid END) as d30
FROM user_cohorts uc
LEFT JOIN messages m ON m.user_id = uc.user_id AND m.sender = 'user'
GROUP BY uc.signup_date
ORDER BY uc.signup_date DESC;
```

---

## Timezone Handling

User timezones are stored in various formats:
- Named: `"America/Sao_Paulo"`, `"Europe/London"`
- Offset: `"UTC-3"`, `"GMT+5:30"`, `"-3"`

**Convert timestamps to user's local time:**
```sql
SELECT 
    u.full_name,
    m.sent_at AT TIME ZONE 'UTC' AT TIME ZONE u.timezone as local_time
FROM messages m
JOIN users u ON m.user_id = u.id
WHERE u.timezone ~ '^[A-Z]';  -- Only named timezones work with AT TIME ZONE
```

---

## Customizing Queries

Edit the `QUERIES` dictionary in `dashboard.py` to add/modify predefined queries:

```python
QUERIES = {
    "📊 My Query": """
    SELECT * FROM my_table
    WHERE condition = true
    """,
}
```

---

## Security

⚠️ **Never commit `.env` or `.streamlit/secrets.toml` to version control!**

The `.gitignore` is already configured to exclude them.


