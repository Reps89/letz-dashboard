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
- **Custom Query**: Write and run any SQL query
- **Predefined Queries**: Common queries ready to run
- **Database Explorer**: Browse tables and schemas in the sidebar

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

## Security

⚠️ **Never commit `.env` to version control!**

The `.gitignore` is already configured to exclude it.

