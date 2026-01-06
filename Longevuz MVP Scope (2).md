# Longevuz  MVP Scope

**Version:** 2.1  
**Date:** 18 September 2025  
**Owner:** [Raphael Nehmer](mailto:raphael.nehmer@gmail.com)(Longevuz)  
**Status:** Draft for comments  
**Related docs:** [Longevuz - Product Vision](https://docs.google.com/document/u/0/d/1LuNHjue0vLj4kxpWo9XmSsyo9AN3a_KD1FuihKv7QG8/edit)

---

# Context

Build a **WhatsApp-based MVP** to validate Longevuz’s core value proposition: helping users close the intention action gap for **sleep and movement** through **science-backed guidance**, **behavioural nudges**, and **supportive accountability**.

Pilot in **Brazil**, leveraging founder networks to test with a diverse user base. MVP runs for **8-12 weeks** with \~**150–200 active users**.

# Guiding Principles

* **“Cupcake” principle:** We want to test the full cycle across the journey, not just go deep into a single functionality.  
* **AI-first (with soul):** We want to anchor the experience to be AI-first but humanised, light, empathetic, rewarding \- powered by LLM-based natural conversations that are personalised and contextual.  
* **Win first 3 days:** We want to ‘wow’ the user in their early interactions with the product  
* **Effortless:** Minimal number of clicks, simple to say “yes” (defaults)  
* **Trustworthy:** Adopt tone and language that instills trust, provide clear explanation, backup information and evidence for people who seek to find out more  
* **Connected:** Virtual supportive companion  
* **Motivating:** Behavioural principles employed throughout \- every screen intentionally designed, every piece of content is worded carefully. 

# MVP Focus

## Target Users

**Upper-middle to middle-income, working parents in large cities**

* **Key problems:** Constant fatigue and lack of time; repeated failed attempts at gyms or diets; guilt and overwhelm when advice feels unrealistic; distrust of fad-driven health content.  
* **Motivation:** Want lasting energy and health to be present for their kids and partners, not just aesthetic gains.

## Geographic Area

Brazil, focus on big cities (SP, Rio).

## User Interface

**WhatsApp** only. Interactive, natural language-based experience, with quick-reply flows and native min-app experience (to be discussed); no standalone app.

# User Problem {#user-problem}

**Closing the intention-action gap and keeping it closed:** How might we help users turn health intentions into sustained habits? 

People are **aware** they need to do something to live healthier lives. They also typically have the **intention** to adopt healthier habits (e.g. nearly half of US adults intend to lose weight)[^1]. 

But they face a range of **barriers** in implementing these habits consistently (e.g. a recent study found that only 52.4% of people who intended to engage in a certain level of physical activity were successful in doing so)[^2] \- these barriers are (based on desktop research and user interviews):

* **Emotional pressures \-** Users often feel guilt, shame, or defeat from past failed attempts.  
* **Limiting beliefs \-** “I’m not disciplined enough,” “I always fail at this.”  
* **Intention quality & stability** \- Weak or vague intentions that fade quickly.  
* **Lack of structure** \- Without clear milestones, users lose direction.  
* **Present bias & procrastination \-** Immediate effort outweighs future health gains.  
* **Low self-efficacy** \- Users doubt their ability to succeed.  
* **Distractions, competing priorities** \- Users lose focus amid other demands.

# Success Metrics

Our P0 goal (i.e. the goal we cannot fail) for the MVP is **early user engagement across their first 3 days.** We believe that the first experience with our product will be highly determinate of future behaviour and longer term retention. As such our focus is to solve the initial problem of “getting started”.

| Metric | Definition | Why |
| :---- | :---- | :---- |
| **P0: Activation Rate** | % users that complete onboarding | Measures initial onboarding success. If initial interactions are seamless and engaging, users will complete onboarding. |
| **P0: First action completion rate** | % of onboarded users that complete their first action | Measures critical first day engagement If users have a good first impression, they are more likely to come back the next day. |
| **P0: First 3 days completion rate** | % of onboarded users that complete their first 3 days | Measures critical first 1-3 days engagement If users see value early (first 3 days), they are more likely to stick around. |
| **P1: Weekly active rate:**   | Average number of days active in a week (%) | Measures longer term user mind-share If users see value, they will use our product on several days in their week |
| **P1: 7D, 30D retention:** | % onboarded users active after 7 days, 30 days | Measures longer term user stickiness If we truly build habits, we will see users retain on our product for the longer term |
| **P1: Daily Engagement Rate** | % of users that take at least 1 action[^3]/day | Overall engagement metric.  If users see value in our product they will use it daily. |

# Products

We believe the following **5 core** **product capabilities** are needed to solve our overarching user problem and address the barriers faced by users.

| Product | Description | Barrier Addressed  | Behavioural Mitigation |
| :---- | :---- | :---- | :---- |
| [AI Companion](#ai-companion) | Non-intrusive, but always present conversation-based companion (inside WhatsApp). Adapts tone based on situation & learnt user motivation styles. | Emotional pressures Limiting beliefs | **Reframing** \- Normalising setbacks, highlighting progress. **Personalisation** \- Messages adapted to user tone/style. **Self-affirmation** \- Reinforcing identity (“you are the kind of person who…”). |
| [Goal/Challenge](#goal/challenge) | Specific and science-backed 30-day sleep or movement Goal that users sign-up to as a challenge. Broken into smaller milestones with **Rewards** (see below). | Intention quality & stability Lack of structure | **Milestones** \- Breaking long goals into achievable chunks. **Challenge framing** \- Turning effort into a game-like pursuit. |
| [Reward](#reward) | Rewards (symbolic, and monetary) tied to achieving specific milestones as part of the user’s **Goal**. In addition, surprise rewards for maintaining engagement.  | Present bias & procrastination | **Endowment effect** \- Making rewards feel “owned.” **Variable rewards** \- Surprise elements keep engagement high. **Immediate reinforcement** \- Closing the feedback loop with near-term rewards. |
| [Daily Micro Ritual](#daily-micro-ritual) | Personalised daily nudge for the user to complete a curated, achievable micro-ritual. Micro-ritual aligns with the **Goal** and milestones, and offers explanation and tips.  | Low self-efficacy Distractions, competing priorities | **Habit loops \-** Cue → routine → reward. **Temptation bundling** \- Pair “should” with “want.” **Fresh-start effect** \- Leverage temporal landmarks. |
| [Accountability Partner](#accountability-partner) | Users can sign up for a shared **Goal** and **Rewards** with a real-world partner. They receive updates on their partner’s progress and hold each other accountable. | Present bias & procrastination | **Commitment device** \- Social “cost” of falling short.  **Relatedness** \- Feeling seen and connected increases motivation.  **Social norms** \- Seeing partner progress creates upward motivation. |

![][image1]

# Enablers

These platform-level capabilities are what make the six product surfaces work together. They are the building blocks that let the Companion, Rituals, Rewards, and Accountability Partner systems operate reliably and learn.

## Longevuz Blueprint

The Longevuz Blueprint is the canonical mapping from **Goals → Weekly challenges → Daily Micro Rituals**. The Blueprint is the product’s “playbook” for turning a single 30-day intention into a sequence of daily actions that are small, evidence-based, and stack into real change.

For example, to help a user achieve a step goal, the Blueprint will provide specific cues and framing techniques, such as “Listen to your favourite podcast outside”, “take the stairs instead of the lift”.

Longevuz Blueprint mapping Goals to Rituals stored here:[Longevuz Blueprint](https://docs.google.com/spreadsheets/d/1-gTzWYcdIIwaUKG50ShGw_JajwiUeTXMBVeFlu9XYcM/edit?gid=0#gid=0) 

## Proprietary User Data {#proprietary-user-data}

Our understanding of users is what separates us (over time) from other AI companions. In MVP we need to strike the right balance between capturing enough data for effective [personalisation](#learning-loop-/-personalisation) whilst not creating excessive friction for the user to provide information to us.

**What we collect:**

* **Profile:** WhatsApp ID/number, locale/timezone, language, age (optional), name (optional), gender (optional)  
* **Health Pillar:** Chosen pillar (sleep or movement)  
* **Baseline:**   
  * Movement: Number of active days/week OR  
  * Sleep: Sleep consistency between weekday/weekend  
* **Barrier:**   
  * Mindsets and beliefs (Emotional pressures, limiting beliefs, low self efficacy),   
  * Planning & execution (intention quality & stability, lack of structure),   
  * External factors & distraction (present bias, distractions & competing priorities)  
* **Tone Preferences:** Supportive, Strict  
* **Goal, Milestones:** 30 day goal and interim milestones  
* **Reward:** Motivation Gift (if relevant)  
* **Accountability partner:** Info on partner (if relevant)  
* **Progress**: Rituals completed/missed, milestones achieved/missed,  Discounts unlocked (if relevant), Badges unlocked  
* **Conversational signals:** quick-reply choices, past messages  
* **Activity times:** timing of read, replies  
* **Operational:** delivery success/failure, time-to-response latency

**Where we collect it**

* **Profile:** [Onboarding](#onboarding)  
* **Health Pillar:**  [Onboarding](#onboarding)  
* **Motivation:**  [Onboarding](#onboarding)  
* **Baseline:**  [Onboarding](#onboarding)  
* **Barrier:**  [Onboarding](#onboarding)  
* **Tone Preferences:**  [Onboarding](#onboarding)  
* **Goal, Milestones:** [Initial goal sign-up](#initial-goal-sign-up)  
* **Reward:** [Motivational Gift choice](#reward-and-gift-selection-[ab-tested]) \+ ongoing progress  
* **Progress**: Ongoing logging  
* **Conversational signals:** Ongoing logging  
* **Activity times:** Ongoing logging  
* **Operational:** Ongoing logging

This proprietary data will be used directly to give context to the **AI companion** for tone, wording adjustments, and it will be used to adjust & refine the **Micro Rituals** based on the **Longevuz Blueprin**t.

## Learning Loop / Personalisation {#learning-loop-/-personalisation}

Personalisation in MVP will leverage the **Proprietary Data** to give context to the AI companion as part of system prompts. We will not attempt full reinforcement learning in the MVP but rely on a rules engine for respective products. 

Decision / rules engine (deterministic) to be specified for:

* Micro Rituals progression (e.g. if complete 3 days in a row, move up)  
* Companion tone changes (e.g. if no reply within 24 hours, change tone)

For testing key hypotheses we will implement a AB testing framework that is fast to iterate. See [Summary of AB Tests](#summary-of-ab-tests).

# Summary of AB Tests {#summary-of-ab-tests}

| Test | Control   | Treatment 1 | Design | Success Metrics |
| :---- | :---- | :---- | :---- | :---- |
| Recovery ladder (first 3 days) | Send Nudge \+ Make Progression | Send Nudge \+ Make Progression \+ Surprise Reward | 50% random assignment of users to Control vs Treatment 1 | Daily engagement rate **Guardrail**: Reward costs |
| Reward types | Soft | Soft \+ Hard | 50% random assignment of users to Control vs Treatment 1 | Daily engagement rate **Guardrail**: Reward costs |
| Accountability partner | Solo journey | Option to pair up with partner | 50% random assignment of users to Control vs Treatment 1 | Daily engagement rate **Guardrail**: Onboarding complete rate |

# Product Specs

WhatsApp chat will house all products, which will be presented to the user as natural conversations that feel human and authentic (LLM-powered) \- e.g. no ‘forms’, no single word replies but also not overly verbose. 

Backend services (for Enablers) will support LLM with personalisation & context and will store key user data on progress, preferences etc.

## AI Companion {#ai-companion}

The AI Companion is the primary user-facing persona. It delivers all product experiences (Daily Micro Rituals, Goal updates, Milestones, Rewards, Buddy updates) through a conversational interface inside WhatsApp. 

It is adaptive, responsive, and designed to feel supportive without being verbose or mechanical.

![][image2]![][image3]![][image4]

### P0 Core functions \- Must have for MVP

#### First 3 days Recovery Ladder {#first-3-days-recovery-ladder}

This is critical **for the first 3 day engagement** in particular. Carries out targeted recovery if the user drops off at any step of the journey (e.g. no interaction with Companion, No onboarding, No Micro Ritual completed/skipped). We will use the following ladder

1. **Send Nudge:**   
   1. **Follow-up:** First check-in message after 24 hours or at 8:00am (whichever is later) if no response  
   2. **Change of tone:** Second check-in message after 12 hours or at 8:00am (whichever is later). Move away from current tone (supportive \-\> coach, or vice versa)   
2. **Make progression (default):** Select an option on behalf of the user (e.g. default goal, default pillar, default micro-ritual)  
3. **Surprise Reward:** Automatically issue a [surprise reward](#surprise-vs.-milestone-rewards) to the user

**MVP constraint:** Employ strategy 1+2, or 1+2+3 \[AB Tested\]:

#### Tone variation {#tone-variation}

* Companion can adjust its tone/messaging (whilst delivering the same content to the user)  
* Default tone: supportive  
* Adjust baseline tone: based on [user data](#proprietary-user-data)  
* Tone can shift back dynamically if the user drops off (see [recovery ladder](#first-3-days-recovery-ladder))  
* **MVP constraint:** Companion to adopt 2 different baseline tones via relevant system prompts  
  * Supportive, empathetic  
  * Strict, coach

#### Personalisation {#personalisation}

* **MVP constraint:** No reinforcement learning, personalisation via system prompts.  
* Adapts messaging to  
  * [User data](#proprietary-user-data) (name, age, health pillar, barriers)  
  * User context (time of day, day, past responses, milestone progress, conversational signals)

**Address specific Barriers**

| Barrier Category | AI Tone | Rules (system Prompts) |
| :---- | :---- | :---- |
| Mindset & Beliefs | **Supportive, Empathetic Friend**. Acts as a confidence builder. | Celebrate small wins. Focus on effort and progress, not perfection. Frame nudges as "you can do this." |
| Planning & Execution | **Structured, Action-Oriented Coach**. Acts as a habit architect. | Provide specific, step-by-step instructions (if-then-planing) Prioritise being clear and direct Ask for logistical details. |
| External Factors & Distractions | **Supportive, but firm.** Acts as a personal assistant to combat inertia. | Keep it short and immediate. Use external triggers for nudges.  |

Refer to [Annex](#annex---summary-of-personalisation-rules) for detailed personalisation rules.

#### Responsive

Answers user-initiated questions about:

* Current ritual  
* Upcoming milestones/rewards  
* Purpose/benefits of assigned rituals  
* How to swap or adjust a ritual  
* Buddy progress  
* Motivation, help implementing micro rituals

Fallback for unrelated questions

Does not adhere to strict flow, adjusts based on user messages.

#### Push frequency {#push-frequency}

* **Morning anchor (default):** Nudges are scheduled for 8:00-9:00am local time.  
* **Evening anchor:** For sleep-focused users, evening nudges (8:30-9:00pm) are used.

**If no user response in past 24 hours**

* Max 1 nudge/day.  
* Nudge delivered at the user's preferred time (morning/evening).  
* After 3 missed days → pause nudges

**If user has responded in past 24 hours**

* Limit to contextual follow-ups (encouragement).  
* Max 2 proactive pushes/day (e.g., one for ritual, one for milestone/reward).

**Inactivity beyond 7 days**

* Trigger re-engagement nudge with “fresh start” framing tied to Monday, month start, or other landmark.  
* Max 1 fresh start nudge

Refer to [Annex](#annex---summary-of-frequency-rules) for detailed frequency rules across all Products

### P1 Functions  \- Nice to Have

* Personalised morning and evening anchors based on user activity times    
* Question for smarters: Is this doable? Is there a minimal set of user interaction data needed?

## Goal/Challenge {#goal/challenge}

The **Goal/Challenge** product gives users a **structured 30-day challenge** that translates broad health intentions into a clear, motivating commitment. Instead of vague aspirations (“I should be healthier”), users choose a **specific medium-term goal**, framed as a **goal with rewards**. This helps overcome **low intention quality** and the lack of structure that often undermines behaviour change.

### P0 Core Functions  \- Must have for MVP

#### Goal Bundle self-selection

* Users self select their own goal bundle from a set of options, based on a their chosen pillar and baseline assessment  
* **MVP constraint:** Fixed library of of goals defined in [Longevuz Blueprint](https://docs.google.com/spreadsheets/d/1-gTzWYcdIIwaUKG50ShGw_JajwiUeTXMBVeFlu9XYcM/edit?gid=48291464#gid=48291464)

#### Individual vs. Collective Goal

**Solo users:** 

* Pick an individual 30-day goal   
* Progress tracked individually


**With buddy:** 

* Both users must agree on the same goal.  
* Goal start date syncs across both.  
* Progress updates are shared with both users  
* Milestone celebrations and failures are mirrored  
  * If both users complete a milestone → collective celebration.  
  * If one lags → companion nudges them with light social accountability (e.g. “Your partner is on track \- want to catch up together?”).  
  * The challenge continues regardless of one user’s lapses, but social comparisons remain visible.  
* **MVP constraint:** Buddy sign up happens only at goal sign-up, not mid-way.

### P1 Functions  \- Nice to Have

* **Fully personalised goals** \- Goal broken into smaller sub-goals as per user baseline (e.g. instead of 2x week strength training start with 1x/week)  
* **Streaks**

## Reward {#reward}

The **Rewards** product motivates users to sustain engagement by combining **immediate gratification** with recognition of **longer-term progress**. Instead of abstract future benefits, users experience tangible reinforcement throughout their journey. 

Users **choose a meaningful gift they buy for themselves**, and then **unlock stacking discounts** toward it. This framing emphasises autonomy and self-investment rather than a “free handout.” 

Rewards are seamlessly integrated into Companion conversations so they feel like **celebrations of progress**, not compliance checks.

* **Present Bias & Procrastination:** By providing rewards that are immediate and visible, users overcome the tendency to delay action (“I’ll start tomorrow”) and instead feel a direct benefit for today’s effort.  
* **Low Motivation / Drop-Off Risk:** Early and surprise rewards create momentum and reduce the risk of early churn, while milestone rewards give users meaningful reasons to keep going.  
* **Social Reinforcement (Buddy Path):** When paired, rewards also function as **shared wins**. Unlocking milestones together amplifies accountability, strengthens the social contract, and turns progress into a collective celebration.

### P0 Core functions \- Must have for MVP

Milestones & Reward logic stored here [Longevuz milestones](https://docs.google.com/spreadsheets/d/1ImCbV4Vb2RtxrsJCD70GaJvmvHPxjZZl0QqD8RsyDto/edit?gid=0#gid=0)

#### Milestones

* **MVP constraint:** Same sequence and number of milestones for each user (no personalised sequence)  
* **Default sequence:** 30-day challenge → broken into Day 3, Day 7, Day 14, Day 21, Day 30 checkpoints.

#### Reward types

**MVP constraint:** To test two different types of reward, soft and soft+hard at a user level \[[AB tested](#summary-of-ab-tests)\]

**Soft Rewards** (symbolic, non-monetary):

Users build their own **secret garden** ("Meu Jardim Secreto")

* Day 1: First soil (surprise) 🌱  
  * Day 3: First Leaves 🌿  
  * Day 7: First flower 🌺  
  * Day 14: Living Garden 🦋  
  * Day 21: Almost complete 🌳  
  * Day 30: Dream Garden 🏡  
* Each milestone comes with a PNG image and emoji  
  * Question for Smarters:   
    * To what extent can we reskin the Whatsapp experience at a user-level based on badge (e.g. different colour scheme, different profile pic of the Companion)?  
    * What can we do to gamify this experience and show user progress  
* Celebratory messages at each milestone

**Soft \+ Hard Rewards** (Motivation Gift):

* Companion invites the user to choose their own **Motivation Gift** from a catalogue (e.g., Amazon, MercadoLibre).  
  * Framing: “Pick something you’ve been eyeing—Longevuz will help you earn discounts on it as you stay consistent.”  
* User accumulate **discount vouchers** on this Motivation gift (e.g. Amazon voucher) upon reaching milestones (marketing-funded during MVP).  
* Question for smarters: How do we execute such discount voucher issuance?

#### Reward amount

* At each milestone, a **fixed discount** is unlocked that accumulates toward the user’s chosen gift:  
* Day 1: $1 (surprise)  
* Day 3: \+$1  
* Day 7: \+$0.5  
* Day 14: \+$0.5  
* Day 21: \+$0.5  
* Day 30: \+$1  
* Companion shows a **progress meter** after each milestone: e.g. “You’ve stacked **$2** off your Motivation Gift—keep going to grow it\!”

#### Surprise vs. Milestone Rewards {#surprise-vs.-milestone-rewards}

**Surprise reward**

* These are not communicated to the user ahead of time  
* Issued after completing a first ritual to drive early engagement  
* Used strategically as part of the [recovery ladde](#first-3-days-recovery-ladder)r if user drops off  
* Can be either Soft or Soft+Hard depending on A/B group

**Milestone reward (Expected reward)** 

* Pre-communicated, tied to milestones & **weekly challenges (Day 3, Day 7, 14, 21, 30\)**. Builds anticipation and stability.  
* Can be Soft or Soft \+ Hard depending on A/B group.

**Qualification criteria**

* Each milestone \= completion of a threshold number of **daily rituals**.  
  * **Day 3:** Achieved if ≥2 of 3 rituals completed. Purpose: reduce early churn by creating fast success.  
  * **Day 7:**  Achieved if ≥5 of 7 rituals completed. Unlocks first meaningful reward.  
  * **Day 14:** Achieved if ≥10 of 14 rituals completed. Reinforces medium-term habit formation.  
  * **Day 21:** Achieved if ≥15 of 21 rituals completed. Behavioural science suggests \~3 weeks to start habit integration.  
  * **Day 30:**Achieved if ≥21 of 30 rituals completed (70% rule).   
* Rewards unlocked at milestones (see [Rewards](#reward)).

#### Accountability Partner Flow \[AB tested\]

* In buddy mode, each person can choose their own Motivation Gift   
* Discounts unlock **only when *both* partners hit a milestone**.   
* If both complete a milestone, both unlock and celebrate.  
* If one completes, one misses,  Companion frames positively, nudging lagging partners.  
* **Surprise rewards** are independent, if one unlocks, the other can still get theirs.

#### Expiry

* Surprise small voucher: expiry \= 12–24 hours.  
* Week/milestone vouchers (Day 7+): expiry \= 7 days (1 week) after the challenge end.

#### Fraud rules

* **Duplicate number checks:** Prevent multiple accounts linked to the same WhatsApp number.  
* **Budget checks:** Cap maximum voucher issuance per user (e.g. $10/user during MVP).  
* **Verification of ritual completion:** Out of scope for MVP. We will trust self-report via Companion responses. Can revisit with passive data capture (e.g., wearables) and active data capture (image recognition) in future.

### P1 Functions  \- Nice to Have 

* **Wearables integration** \- for automatic step count and activity detection  
* **Verification steps \-** e.g. image as proof  
* **Health score** as a holistic way to track progress  
* **Further gamification** \- eg. character development, growth, accessories  
* **Personalised milestones**

## Daily Micro Ritual {#daily-micro-ritual}

Daily Micro Rituals are the **“living” delivery of the Longevuz Blueprint**: simple, evidence-based actions that help users turn intentions into practice. They provide the *how* for achieving 30-day goals.

Micro Rituals directly address two of the biggest barriers to habit adoption:

* **Low self-efficacy:** Rituals are deliberately small and achievable (2–5 minutes initially), helping users build confidence through consistent wins.  
* **Forgetfulness:** Rituals are paired with timely nudges, reminders, and if–then anchors (implementation intentions) to make action more automatic and harder to forget.

**MVP constraint:** Fixed mapping. Longevuz Blueprint mapping Goals to Rituals stored here:[Longevuz Blueprint](https://docs.google.com/spreadsheets/d/1-gTzWYcdIIwaUKG50ShGw_JajwiUeTXMBVeFlu9XYcM/edit?gid=0#gid=0)

### P0 Core functions \- Must have for MVP

Proactive daily nudges delivered by Companion in personalised tone. ritual based on behavioural science-backed framing:

* **Habit loops** (Cue → routine → reward).  
* **Temptation bundling** (pair “should” with “want”).  
* **Fresh-start effect** (new week, birthday, Monday cues).

#### Daily Check-in

Sent at specific [anchor times](#annex---summary-of-frequency-rules) (morning or evening)  
If goal activity

* User Actions: **DONE | SKIP | REMIND ME | WHY | SWAP**.  
  * DONE → celebrate \+ reward trigger.  
  * SKIP → supportive reply (“Missing one is normal \- try again tomorrow”).  
  * REMIND ME→  Ask for preferred time, keep user accountable if too far in future  
  * WHY → Every ritual can be explained with a short, science-based rationale to boost buy-in. (“This works because dimming lights cues your body to produce melatonin”).  
  * SWAP → offer alternative   
  * Free-text Feedback → User can reply naturally anytime with context (e.g., “I work night shifts”).

**Tips**  
Micro rituals can offer tips for achieving the goal (based on behavioural science)

* E.g., if goal is “go to bed at a consistent time each day,” rituals may include “dim lights for 5 minutes” or “put your phone outside the bedroom”

If no goal activity scheduled on day

* Check in to see how user is feeling  
* Offer ‘Filler’ ritual 1-2mins

#### Daily Digest

Sent at opposite  [anchor time](#annex---summary-of-frequency-rules) from Daily check-in

* Check-in how user is feeling  
* Partner update (Partner snippet)  
* Milestone update (if relevant)  
* Prepare for upcoming ritual 

**MVP constraint:** [Longevuz Blueprint](https://docs.google.com/spreadsheets/u/0/d/1-gTzWYcdIIwaUKG50ShGw_JajwiUeTXMBVeFlu9XYcM/edit)

### P1 Functions  \- Nice to Have

* TBD

## Accountability Partner {#accountability-partner}

Accountability Partners add a **social contract** layer to habit formation. Signing up with a partner acts as a commitment device as this creates shared momentum, and adds a social “cost” for not following through.

This product addresses:

* **Commitment device:** Users are less likely to fall short if someone they know is tracking their progress.  
* **Relatedness:** Transformation is easier when users feel seen and connected to another human on the same journey.  
* **Social norms:** Seeing a partner’s progress creates upward motivation (“If they can do it, so can I”).

**MVP constraint:** We will enable this product via [\[AB test](#summary-of-ab-tests)\] at a user level.

### P0 Core functions \- Must have for MVP

#### Interplay with AI Companion

Accountability partners are not expected to actively message each other beyond the basic interactions set out above \- that is the role of the AI agent. The AI agent is the empathising ‘coach’ that remains in the background and is always there to add support and timely nudges. The accountability partner in that sense acts more passively but because users have a real world relationship with them their impact on commitment is expected to be strong.

**Companion \= Emotional Coach**

* Handles motivation, framing, emotional support, and belief reframing.  
* Always available for empathetic nudges.

**Accountability Partner \= Social Contract**

* Adds passive, real-world accountability through visibility and light interactions.  
* Not a chatty peer-to-peer channel; instead, structured updates and kudos prompts keep it lightweight.

#### Partner selection

At sign-up partners/friends join a goal/challenge together and work together towards a reward. Enabled via \[AB test\]

#### Partner updates

Partners receive three types of updates:

* **Real-time completion notice**: e.g. “Alex completed today’s ritual.” if inside active window, otherwise: partner snippet  
* **Partner snippet** \- included in the recipient’s daily digest: short summary of partner’s activity.  
* **Milestone / major event alert** \- partner hit a weekly milestone or unlocked a milestone reward.

Delivered according to [frequency rules](#push-frequency).

#### Shared Goal/Rewards

* If both complete → collective celebration \+ mirrored reward.  
* If one completes, one misses → Companion frames positively, encouraging lagging partner

**Reward rules**

* Users can choose their own Motivation Gift  
* To receive **stackable milestone rewards** both users must meet the milestone.   
  * Both users receive the **same** reward (randomly chosen)   
* Soft rewards remain individual.   
* Surprise rewards stay individual. 

### P1 Functions  \- Nice to Have

* **Group-based sign up for a goal**

# User Journeys

To illustrate the user journey combining each product, we break our [L0 Problem](#user-problem) down into sub-problems (L1) with measurable outcomes and success metrics across the **user lifecycle**.

**L1 Problems:**

1. **P0: Set intentions (Day 0):** How might we help users *set intentions* that are motivating and achievable?  
   1. Success Metric/Goal:   
      1. **P0” Activation rate:** % users that complete onboarding  
2. **P0: Get started (Day 1-3):** How might we help users to *start implementing* new behaviours to work towards their intentions?  
   1. Success Metric/Goal:  
      1.  **P0: First action completion rate:** % of onboarded users that complete their first action  
      2. **P0: First 3 days completion rate:** % of onboarded users that complete their first 3 days  
3. **P1: Keep going (Day 7+):** How might we help users *stick with* new behaviours so that they become automatic habits?  
   1. Success Metric/Goal  
      1. **P1: Weekly active rate:** Average number of days active in a week (%)  
      2. **P1: 7D, 30D retention:** % onboarded users active after 7 days, 30 days

## 1\. Set Intentions (Day 0\)

### Onboarding {#onboarding}

Conversational onboarding and mini dialogue for user to provide answers using quick action OR natural language

**Welcome to Longevuz**

* Welcome message with a “get started” CTA


**Collect basics** 

* Companion to ask for user’s name (optional), birth year, (optional), and one-time consent (mandatory, guided by WhatsApp rules)

**Select Pillar**

* Companion lets user choose **sleep or movement** as a focus area

**Assess baseline**

* If user chose **sleep**  
  * “In the last 7 days, on how many days did you do at least 30 minutes of physical activity (e.g., walking, standing, exercise)?”  
    * (A) 0 Days  
    * (B) 1 \- 2 Day  
    * (C) 3- 4 Days  
    * (D) 5 \- 6 Days  
    * (E) 7 Days  
    * (F) I don't know  
* If user chose **movement**   
  * “How much does your wake up and bed time differ between weekends or days off vs. weekdays?”  
    * (A) less than 30 mins difference  
    * (B) 30-90 mins difference  
    * (C) more than 90 mins difference  
    * (D) I don't have a regular sleep schedule  
    * (E) I don't know  
* *Note: Helps us assign Goal to user*

**Identify Barrier:**

* “Think about a time you tried to start a new habit but didn't stick with it. What was the biggest reason it didn't work out?”  
  * (A) I just couldn't get started. I felt like I wasn't the right kind of person for it, or lost motivation.   
  * (B) I had good intentions, but I never had a clear plan for when and how to do it. It was too hard to fit into my daily routine.   
  * (C) Other things always got in the way. I'd forget, get distracted, or put it off until tomorrow.  
  * (D) Others  
* *Note: Helps us classify user barriers into: mindsets & beliefs, planning & execution, external factors in [user data](#proprietary-user-data)*

**Identify Preferences:**

* “Think about a time you successfully stuck with a new routine. What was the most important factor?”  
  * (1) The positive support and encouragement I received.  
  * (2) The firm structure and accountability I had in place.  
  * (3) Both  
* *Note: Helps us classify default user tone preferences into: supportive vs. strict  in [user data](#proprietary-user-data)*

***\=\> ONBOARDING COMPLETE***

### Initial goal sign-up {#initial-goal-sign-up}

**Goal assignment**

* Based on the chosen pillar and baseline assessment at Onboarding, Companion assigns **recommended goal options** for user to choose from a predefined list.  
  * 3-4 recommended 30-day goals, other goals listed below recommended list

* Illustrative example

| 30 day goal: Based on your activity level, here are a few high-impact activities to consider. Pick the one you're most excited to start with\! ⭐Walk 7,000 steps daily: The easiest way to boost your energy and overall health. ⭐2-3x/week Strength training (bodyweight): Builds muscle, improves metabolism, and protects your joints. ⭐2-3x/week Zone 2 cardio: Improves heart health and endurance. 3x/week Dedicated Core Stability Work (15min) 3x/week Ankle & Hip Mobility Routine (5–10 min) Daily Spinal Mobility Flow (2-3mins) |
| :---- |

  * Logic for goal recommendation defined inside [Longevuz Blueprint](https://docs.google.com/spreadsheets/d/1-gTzWYcdIIwaUKG50ShGw_JajwiUeTXMBVeFlu9XYcM/edit?gid=784342799#gid=784342799).  
* Companion frames each option following behavioural principles:  
  * **Autonomy (vs. Control):** “You choose what feels right for your lifestyle.”  
  * **Specific (vs. General):** Clear, concrete goals (e.g., “Take a 10-minute walk daily”) rather than vague intentions (“Be more active”).  
  * **Promotion (vs. Prevention):** Goals are framed as positive actions (“Build energy”) instead of avoidance (“Stop being tired”).  
  * **Learning (vs. Mastery):** Goals emphasise progress, not perfection (“Get better at winding down at night”).  
* User picks **specific goal for 30 days** (can also choose ones not recommended)   
* Follow-up if no response in line with [recovery ladder.](#first-3-days-recovery-ladder)

**Highlight Reward**

* Companion asks user to select Motivation Gift (if relevant)  
* Companion introduces [milestone rewards](#reward) upfront when asking the user to select their goal (e.g., “You’ll unlock rewards at Day 3, Day 7, Day 14, Day 30”).  
* Rewards are framed as **celebrations of progress**, not tests of compliance.

### Buddy Sign up \[AB tested\]

**Ask to buddy up**

* After user selects goal, Companion to ask user if they would like to go on this journey with a partner   
* Companion to highlight and explain the benefits of joining with a partner  
  * Shared accountability, you both share this journey together, you both can get rewards

**Invite buddy**

* If user says yes:  
  * **Invite Link:**   
* System generates a secure invite link (single-use, expires in 48 hours).   
  * Companion sends: “Send this invite to your partner so you can do the same challenge together.”  
* When invitee clicks, their Companion opens the UI and the proposed goal is pre-selected. Invitee can:  
  * Accept the proposed goal → pairing proceeds.  
  * Reject the proposed goals →User proceeds solo  
* ​​If the invitee does not accept within 48 hours, link expires and the inviter is notified.  
* If user says no: proceed solo  
* **MVP restriction:** pairs only  
* **MVP restriction:** Pairing only possible at onboarding (not mid-journey).

### Reward and Gift Selection \[AB tested\] {#reward-and-gift-selection-[ab-tested]}

#### Soft Rewards only

* Companion explains how goals are broken down into milestones over the next 30 days  
* Companion explains how users unlock rewards for each milestone, where they build their own **secret garden.**  
* Companion highlights upcoming milestones

#### Hard \+ Soft Rewards

**Motivation Gift**

* Companion asks user to **choose their own Motivation Gift,** something they will buy for themselves at the end of the challenge.  
* "Pick something you've been eyeing—Longevuz will help you earn discounts on it as you stay consistent. "  
* User either pastes Amazon/Mercadolibre link or writes a message with their chosen gift  
  * Store this in [user data](#proprietary-user-data) /context  
* Companion reflects this and explains how they can unlock savings towards their gift as they hit milestones  
  * "Great choice\! \[Product Name\] for $\[Price\]. As you hit milestones, you'll stack discounts toward this gift. Let's get started\!"  
* Selection is **optional**: users who skip will default to a generic discount on Amazon.

**Discounts**  
Companion introduces the concept of cumulative milestone discounts: e.g. “Every week you’ll unlock discounts at Day 3, Week 1, Week 2, Week 3, and the finish at Day 30.”

Companion offers **“Learn More” flow** (optional):

* Explains voucher amounts (hard discounts to help purchase the user's Motivation Gift).  
* Explains how user progressively unlocks discounts by hitting more milestones  
* Explains qualification criteria

**Buddy path**

* Companion highlights shared reward moments: “You and your partner will unlock rewards together when you hit your milestones”

### Set your plan

**Introduction**

* Companion introduces the concept: e.g. “Your big goal is achieved through small daily rituals — bite-sized steps that fit into your life.”

**First Ritual**

* Companion asks user to set a **plan** for their selected goal (if-then-planning)  
* For each activity ask the user **what day & what time** they plan to complete it, and (if relevant) what they will do  
  * “On \[day/time\], I will \[run/bike/swim\] for 20 min.”  
* Offer tip from [Longevuz Blueprint](https://docs.google.com/spreadsheets/u/0/d/1-gTzWYcdIIwaUKG50ShGw_JajwiUeTXMBVeFlu9XYcM/edit)to achieve first ritual  
* Companion reminds user that they will send a reminder at the stated time

## 2\. Get Started (Day 1-3)

### Daily check-in

**Nudge**

* Sent at relevant goal time as per user’s plan, or default evening or morning anchor depending on chosen pillar (see [Frequency Rules](#annex---summary-of-frequency-rules) for more details).  
* Gentle nudge to complete the first Micro Ritual at relevant time in line with [Longevuz Blueprint](https://docs.google.com/spreadsheets/u/0/d/1-gTzWYcdIIwaUKG50ShGw_JajwiUeTXMBVeFlu9XYcM/edit)  
* Companion delivers:  
  * Instruction (“Tonight, dim your bedroom lights for 5 minutes before bed”).  
  * Why (“This helps signal to your brain it’s time to rest”).  
  * CTA (DONE | SKIP | REMIND ME | WHY| SWAP).


**Encouragement**

* If skipped \-\> framing according to tone &  companion asks to adjust goal or adjust plan, offers tips  
* If completed → Celebration & [Surprise reward](#reward) (if relevant)  
* If no response→ Follow-up if no response in line with [recovery ladder.](#first-3-days-recovery-ladder)

***\=\>FIRST ACTION COMPLETE***

### Early Surprise Reward (Day 1\)

* If user completes their very first ritual, issue a small **surprise reward** (soft or soft \+ hard).   
  * Soft: First soil 🌱   
  * Hard:+ $1  
* If user skips or misses. Companion to trigger a surprise reward tactically: e.g. “Here’s a bonus reward you can unlock today if you complete your ritual — expires in 24 hours.”

### Daily Digest

If user active

* Sent at evening or morning anchor depending on users chosen pillar (see [Frequency Rules](#annex---summary-of-frequency-rules) for more details)  
  * If sleep \- send Daily Digest in morning  
  * If movement \- send Daily Digest in evening  
* Includes:  
  * **Companion Update** (if any)  
* Day 1 surprise reward is not dependent on buddy completion.  
* If one user unlocks a surprise:   
  * “Alex just unlocked a surprise reward \- yours is waiting too.”  
* If both still need to complete, offer encouragement:  
  * “Don’t let your partner down”  
  * **Milestone progress** and upcoming rewards  
    * “You are nearly there, you need 1 more activity to hit your 3 Day Milestone”  
  * **Reminder** of upcoming activity as per the Goal  
  * **Gentle check-in** to see how user is coping and if they want to make any changes

If user inactive

* Follow up in line with [recovery ladder.](#first-3-days-recovery-ladder)

***\=\>DAY 1 COMPLETE***

### Daily check-in

If user active

* Companion issues 2nd Ritual and offers tips as per [Longevuz Blueprint](https://docs.google.com/spreadsheets/u/0/d/1-gTzWYcdIIwaUKG50ShGw_JajwiUeTXMBVeFlu9XYcM/edit)  
  * Consistent structure and CTA

If user inactive

* Follow up in line with [recovery ladder.](#first-3-days-recovery-ladder)

### Daily Digest

If user active

* Send daily update

If user inactive

* Follow up in line with [recovery ladder.](#first-3-days-recovery-ladder)

***\=\>DAY 2 COMPLETE***

### Daily check-in

If user active

* Companion issues 2nd Ritual and offers tips as per [Longevuz Blueprint](https://docs.google.com/spreadsheets/u/0/d/1-gTzWYcdIIwaUKG50ShGw_JajwiUeTXMBVeFlu9XYcM/edit)  
  * Consistent structure and CTA

If user inactive

* Follow up in line with [recovery ladder.](#first-3-days-recovery-ladder)

### Milestone Reward (Day 3\)

If user active

* Trigger: ≥2 of 3 rituals completed.  
* Soft: First Leaves 🌿  
* Hard: \+$1  
* If missed: Companion reframes \- “You didn’t hit the 3-Day challenge, but you still logged rituals — progress counts. Next week is another chance.”

**Accountability partner**

* Reward unlocked if both meet threshold.  
* If one lagging, send nudge to parter

If user inactive

* Follow up in line with [recovery ladder.](#first-3-days-recovery-ladder)

### Daily Digest

If user active

* Send daily update

If user inactive

* Follow up in line with [recovery ladder.](#first-3-days-recovery-ladder)

***\=\>FIRST 3 DAYS COMPLETE***

## 3\. Keep Going (Day 7+)

#### Ongoing Check-in

* Daily nudges adjusted for user progress.  
* Rituals adapt in difficulty over time in line with [Micro Ritual](#daily-micro-ritual).  
* Follow-up if no response in line with [recovery ladder.](#first-3-days-recovery-ladder)

#### Persona shifts

* Reframe set backs \- Companion reduces shame from lapses (“One day doesn’t erase your progress”).  
* Persona shifts in line with [Tone variation](#tone-variation)

**Progressive Rituals:**

* Difficulty and type increase over time  in line with milestones  
* Ensures challenge remains fresh but achievable

**Feedback Handling:**

* If user reports ritual too easy/hard → Companion offers swap:  
  * “Got it — want to try an easier option tomorrow?”  
* If user adds context (e.g., night shifts) \- stored in [Proprietary data](#proprietary-user-data), used to personalise future assignments.

**Recovery Support:**

* If rituals are skipped multiple days → Companion offers reset option or reframes with fresh start effect.

**Buddy path**

* Buddy pairs are encouraged to share kudos when both complete rituals.  
* If one lags, Companion nudges gently (“Your partner logged today’s ritual — want to catch up together?”).

### Weekly digest

xx

### Weekly Goals and rewards (Day 7, 14, 21\)

**Overall**

Delivered every 7 days as a forward-looking goal (“This week’s challenge: complete 5 rituals”).

**Day 7:** Threshold ≥5 rituals.

* Soft:  First flower 🌺  
* Hard: \+0.5$ additional discount

**Day 14:** Threshold ≥10 rituals.

* Soft:Living Garden 🦋  
* Hard:+0.5$ additional discount

**Day 21:** Threshold ≥15 rituals.

* Soft: Almost complete 🌳  
* Hard: \+0.5$ additional discount

**Day 30:** Threshold ≥21 rituals.

* Soft: Dream Garden 🏡  
* Hard: \+1$ additional discount

**Buddy path**

* Joint reward unlocked if both meet threshold.  
* If one completes, one misses: Companion encourages lagging partner without shaming.  
* If both miss, reframe.

### Day 30 completion

* Goal validated if ≥21 rituals done.  
* Companion delivers celebration and major reward.  
* If under threshold, Companion reframes (“You didn’t hit the full 30, but you still built momentum”).  
* Companion offers reset options:  
1. Restart the same challenge.  
2. Level up your challenge.  
3. Try new pillar (sleep ↔ movement).

# ANNEX \- Summary of Frequency Rules {#annex---summary-of-frequency-rules}

These rules are enforced for every proactive message the Companion might send (anything not in direct response to a user message).

## Global Rules

**User session / activity windows**

* **Session window:** user is “in-session” if they have **sent a message in last 30 minutes**.  
* **Active window:** user is “active” if they have **responded in last 24 hours**.  
* **Wake window:** default 07:00–22:00 local time (used to avoid sending at night).

**Daily proactive push budget**

* **If active (responded in last 24h):** max **2 proactive pushes/day**.  
* **If inactive (\>24h):** max **1 proactive push/day**.  
* **If 3 consecutive proactive pushes were sent with NO reply within 72 hours:** pause all proactive pushes until user re-engages.

**Inactivity beyond 7 days**

* Trigger re-engagement nudge with “fresh start” framing tied to Monday, month start, or other landmark.  
* Max 1 fresh start nudge/user

**Session exception**

* If user is **in-session** (last message within 30 mins), **in-session companion messages** (companion replies and partner events triggered by that session) are **delivered immediately** and **do not count** against the daily proactive budget. This allows fluid, in-conversation interactions.

**Wake window enforcement**

* All proactive pushes must be scheduled inside the user’s wake window. If triggered outside wake window, deliver at the next wake window anchor.

**Preferred time anchors**

* Default morning anchor: **08:00–09:00 local**. (for movement daily check-in)  
* Default evening anchor: **20:30–21:00 local**. (for sleep daily check-in)  
* Nudges default to the user’s chosen pillar; system respects timezones.

## Priority Order

When multiple messages want to send at the same time, use this priority order (high → low):

1. Reward issuance (soft and soft+hard)  
2. Milestone completion alert   
3. In-session partner interactions (kudos, completion reactions)  
4. Daily Micro Ritual reminder (scheduled nudge)  
5. Daily digest (includes partner update)  
6. Weekly digest (instead of daily digest)  
7. Recovery / re-engagement nudges

## Daily Micro Ritual

**Daily Nudge:** once per day at user preferred anchor (morning or evening per pillar). This is the highest-importance scheduled push (priority rank 4).

**Behaviour:**

* If user **in-session** → deliver ritual instantly.  
* If user **active but not in-session** → deliver scheduled ritual; counts as one proactive push.  
* If user **inactive \>24h** → scheduled ritual uses the single allowed push for the day.

**Missed ritual recovery ladder** (see Recovery Ladder).

**Daily Digest:** once per day 12 hours after Daily nudge or within the wake window, whichever is later. 

* Partner update   
* Upcoming milestone

**Swap/Feedback interactions** triggered by user do not count against proactive budget (they are responses).

**If more than one product attempts to push at the ritual slot (e.g., partner milestone \+ ritual):** use priority order

## Reward

**Surprise Rewards (issued immediately upon trigger):**

* **If user in-session:** deliver immediately (session-exempt).  
* **If user not in-session:** attempt immediate delivery. If cap is full, schedule delivery at next scheduled nudge but mark voucher expiry appropriately (see expiry rules).  
* **Expiry-critical rule:** the system will prefer immediate delivery. Limit: **1 immediate surprise monetary issuance per user per 72h**.

**Milestone Rewards (expected):**

* Issue immediately at milestone close (priority rank 3). If user inactive and cap full, schedule at next daily nudge (expiry windows for milestone vouchers are typically 7 days \- allows scheduling).

**Expiry reminders:** 24h before expiry send one reminder (counts as a proactive push). For short expiry (≤24h), send reminder at 6–12h if user did not reply

## Partner Updates

* **Real-time completion notice:** deliver in-session if recipient active within 30min; otherwise coalesce into daily digest.  
* **Daily digest / partner snippet:** included inside the daily ritual nudge by default (no extra push). If user opted out of daily nudges, send a single daily digest at preferred time (counts as the 1 push if inactive).  
* **Milestone partner alerts:** high priority; if recipient inactive and cap full, defer to daily nudge unless recipient active.

# ANNEX \- Summary of Personalisation Rules {#annex---summary-of-personalisation-rules}

| User Data |  | Personalisation rules  |
| :---- | :---- | :---- |
| **Profile**  | WhatsApp ID/number, locale/timezone, language, age (optional), name (optional), gender (optional) | **Locale/timezone** for [Frequency rules](#annex---summary-of-frequency-rules) Pass name as **context** to Companion WhatsApp ID/number not used (for analysis, fraud rules) Age not used (for analysis) Gender not used (for analysis)  |
| **Health Pillar**  | Chosen pillar (sleep or movement) | Pass pillar as **context** to Companion |
| **Barriers**  | Mindserts and beliefs (Emotional pressures, limiting beliefs, low self efficacy),  Planning & execution (intention quality & stability, lack of structure),  External factors & distraction (present bias, distractions & competing priorities) | Pass **system prompts** for each barrier as set out in [AI Companion (Personalisation)](#personalisation) |
| **Tone Preferences** | Supportive, Strict | Pass **system prompt** for each tone |
| **Goal, Milestones**  | 30 day goal and interim milestones | Pass **context** on 30 day goals and upcoming milestone  |
| **Reward**  | Motivation Gift (if relevant) | Pass **context** on Motivation Gift to Companion |
| **Progress**  | Rituals completed/missed, milestones achieved/missed,  Discounts unlocked (if relevant), Badges unlocked | Pass **context** on Progress to Companion |
| **Conversational signals**  | quick-reply choices, past messages | Pass **past messages** as context to Companion |
| **Activity times** | Timing of read, replies | If consistent timing (daily variance within threshold) \-\> store and set as user-specific morning/evening anchor times |
| **Operational**  | delivery success/failure, time-to-response latency | Not used (for analysis) |

# ANNEX \- Roles and Responsibilities

BSP:

* AI Companion user experience/UI \- user interactions, tones flows  
  * System prompts co-owned  
  * Frequency rules, Personalization rules co-owned  
* Goals and Rewards user experience  
  * Learn more experience  
  * Soft reward experience  
  * Motivation Gift choice experience  
  * Hard Voucher issuance experience  
* Daily Micro ritual user experience  
  * User interactions  
  * Quick action buttons  
* Accountability partner user experience (sign-up, invite, partner updates)

Longevuz:

* Enablers  
* Backend logic for Goal/Challange  
* Backend logic for Reward/Milestones  
* Backend Logic for Daily Micro Ritual  
* Backend logic for Accountability partner

# ANNEX \- Key Deliverables

1. Day 0 (Set intentions) flow  
2. Day 1-3 (Get started) flow  
3. Day 7+ (Keep going) flow  
4. Functional AB testing   
   1. Feature flags enabled at user-level  
5. User level and aggregate analytics

[^1]:  [https://www.cdc.gov/nchs/data/databriefs/db313.pdf](https://www.cdc.gov/nchs/data/databriefs/db313.pdf)	

[^2]:  [https://doi.org/10.1136/bjsports-2022-106640](https://doi.org/10.1136/bjsports-2022-106640)	

[^3]:  Action: Read message, write message, use quick reply etc

[image1]: <data:image/png;base64,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eaG55547bWt0g+Pwwgsv1A0KHn/88bQtLjvUTFwqqdGgIC45lA8ZZsyYUdue3+/gC1/4QuFoAACqxqCgYgwKAABgplaDgtwHH3yQLb744unYbbfdtra9L4OC1157rfaYV155pXT0h9577726QcFVV12Vti2zzDKFI7ubNm1aw0FByG/IfNRRR9W25ZckinsfAABQXQYFFWNQAAAAM7U7KAj77rtvOjYGBrnioCCGCWXvv/9+uqxRcVAQx02cODFte+qpp0qP+NCbb75ZNyh4+OGH07YYPDTz4x//uOmg4MYbb0z74pJKIc5miI8XWWSRhq8dAIDqMCioGIMCAACYqTeDgt122y0du8Yaa9S2/fa3v60NCuIsgLLi/uI9CtZff/20LRbvG3n00UfrBgVxj4J86PDuu+8Wjp7p5JNPbjoo+Ne//pXNP//8af+TTz6ZziyIfz7ssMPKhwIAUDEGBRVjUAAAADO1Oyh4/fXXswUXXDAde/DBB9e2v/POO7VBwPTp0wuP+NAVV1zRcFDwzW9+M23baqutCkfPdNBBB9UNCsIqq6yStse9Bcri3gdxw+Vmg4KQf95jjjkmW2mlldI/x1kRAABUm0FBxRgUAADATPmgYIEFFkiX+ykW9xL4zW9+k1166aXZ8ssvn46bffbZu10uKBbnl1xyybRviy226Hafgri0T37T4vKgIJ43v3fBueeeW9se7rzzzmzChAkNBwXXXHNN2h6PffDBB7vtmzJlSu1zNRsUPP3002l/XG4o/nettdYqHwIAQAUZFFSMQQEAAMyUDwraKS77c/nll5efIjvjjDNqx8TA4Qtf+EJ65/+ss86arbnmmtmnP/3ptK84KAh333137VJCcSmiQw45JN0oecyYMenyRrG9PCgI+UAg9u24447pcbHgH9vyxzUbFITVVlut9nrPO++88m4AACrIoKBiDAoAAGCmngYF48ePT2cLrLvuutmhhx6avfzyy+WH11xwwQXZPPPMU3vsHHPMke2yyy7ZX/7yl7T432hQEK677rp0c+H8cWPHjs122GGH7O23364NAxo59thju52tMOecc2ZHH310Nm3atPRxT4OCc845p/b1NbvXAQAA1WJQUDEGBQAAMHji5sVxI+K4cXC7Pvjgg3SfgJ///OfZ3/72t/LupuLYuLxR9P7775d3N3XhhRemQcHnP//5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QGcUb3TsrAIAADrFoEDqMigAAKAzDAoAABgODAqkLoMCAAA6Ix8SuPwQAACdZFAgdRkUAAAw9IpnEzirAACATjIokLoMCgAAGHqNBgURAAAMNYMCqcugAACAoVceELj8EAAAnWJQIHUZFAAAMLSanU0QufwQAABDzaBA6jIoAABgaJWHA+UAAGAoGRRIXQYFAAAMnbi0UHkwUM7lhwAAGEoGBVKXQQEAAEOnp8sO5bn8EAAAQ8mgQOoyKAAAYOiUhwLNclYBAABDxaBA6jIoAABgaLRzNoFBAQAAQ82gQOoyKAAAYGj0ZlDg8kMAAAwVg4KP2n333bPNNtusrs033zzbeuuts5122ik75JBDsgceeKDusSOxn/zkJ+nr23PPPev29acXXnihbttIyKAAAIChEGcJlJsyZUq299571213RgEAAEPFoOCjPvnJT2azzDJLW6211lrZyy+/XPccI6mLLroofS2f+tSn6vb1pYcffjjbYIMNshNOOKFu30jIoAAAgE455ZRTsq9//evlzQAAMGQMCj4qHxRss8022fe///1unXvuudnUqVOzjTfeuDYs2HTTTbM//vGPdc8zUopTntdYY43s85//fN2+vhRnJ8T3xaAAAAB65+STT87233//8mYAABgyBgUflQ8KDj/88Lp9ee+++252xBFH1IYFt9xyS90xVc2gAAAA+uakk07KDjjggPJmAAAYMgYFH9XOoCB65ZVXsvHjx6djv/vd79btz4uzDV5//fW67cV+97vfZW+++Wbd9lbFY+Kx5e091c7raVQMR1588cW67eV6Myh49dVXe33ppr6+/nYzKAAAoFOOPvpogwIAADrKoOCj2h0URKuttlo69otf/GJt2ze+8Y1s2WWXzW6++eZ0M7J55503m2OOObJtt902e+aZZ2rH/fKXv0w3Rl5ggQXSc8w222zZCiuskD5vo6HBt771rfS8V199dXbrrbdmn/70p7MJEyakx8ZzHHbYYdkbb7xR97hWr+eaa65J++Pj8mOjyy67LFt77bWzOeecM32u+eabL93Y+cEHH+x2XDx/PM/EiRNrryk+jhs/F4+7/fbb0zBhscUWy2adddZ07Pzzz5+tt9562W233Vb3+Xt6/d/73vfSvg033LDucXlPPPFEOmaVVVZp+P0pZ1AAAECnxBuQDjzwwPJmAAAYMgYFH9XuoCDeYZ8v8n/nO9+pbY9r/ce2r371q7VLE0VzzTVX9tprr6Vjrrjiitoi/9xzz51u/rvyyiunYUFsixsLF4cK0Ve+8pW0L4YL8dhJkyZl22+/fbpHQv5cu+22W93rbPV6mt3MON65/6Uvfal2/PLLL59tscUW2aKLLpo+js951lln1Y6/6aabsqWXXjot4sf+GCjExwcffHDtmBga5MOBeL4tt9yy2xAi9v3whz9s+/U/+eST2ZgxY9LHd911V93XHsW/x9gf37fyvkYZFAAA0CknnnhidtBBB5U3AwDAkDEo+Kh2BwXxbvZ80Tre7Z5vzxe2Y9E7bhJ83XXXZTfeeGN24YUXpv3PP/98eld8HPPlL3+5NjyIHn744fTu99gXi/LFz5cPCqJ43niefN/999+fLbzwwmnfmWee2e1xrV5Ps0HBaaedlrbPM8886fjivrh2agw14tJL8Y794r5mlx565JFH0vZx48al11Dc99vf/jZbddVV0/54539xX6vXH2c3xP699tqr2+OiGOYsueSSaf/1119ft79RBgUAAHRKDArijTYAANApBgUflQ8Kdtlll+zHP/5xty699NI0INhoo41qi/Zbb711t8fnC9vxzvrp06fXPf+uu+6a9scZBLGQXd4fC+pjx45Nx8RlgfLt+aAgFtqffvrpusfFwnnsj3faF5+31etpNCiI+wbkw4xLLrmk7jHRfvvtl/bHWQ3F7c0GBXHWRbz24mWaip1yyinpcfG1F7e3ev1xBkLsjzMY3nrrrW77pk2blvbFECXOkCg/tlEGBQAAdMrUqVMNCgAA6CiDgo/KBwXttOOOO3Z7Z3+UL2yvvvrqdc8dfeITn0j7L7744rp9edttt106Zv/9969tK156qHx8FAvhcRmjOObxxx+vbW/1ehoNCuId+7EtLgnUbIE9LvUTx8TnLG5vNiiIeroR8U9/+tPa97W44N/q9cd9B+IyTHFM3L+huC8uxRTb4z4H5cc1y6AAAIBOid+hjz322PJmAAAYMgYFH5UPChZaaKF0s+JicSZBLNjHu+PvuOOOusdG+cJ2/G95XyyA5/chuO++++r258WNi+OYuIZ/vi0fFBTvh1BupZVWSscUr/Pf0+uJGg0K8nf3xwJ8nFnRqHyYERWHJT0NCqI42+Gxxx7LLr/88uzoo49O90GIsyvyexdExZs5t3r90d57752OKQ5RYoCQD07iLI3yY5plUAAAQKcYFAAA0GkGBR/V7j0KmpUvbDd6F3vcfLfR4nq5fKG+uHifDwrOPffcuuPzNtlkk3TMMcccU9vW0+uJGg0KDjjggNrrbKef/exntcf2NCiI4cByyy1X9/hY0N94441rHzcaFDR7/dG9996bjpl99tmz3//+92lbXCYqtjU7E6FZBgUAAHRKXOa0v4OC+H32gw8+KG8GAIC2GBR81EANCr75zW/W7XvllVdqi+EPPfRQ3f68ww47LB2z3nrr1bblg4Ljjz++7vi8WOyPY2JBPt/W0+uJGg0KYtAQ29Zaa6003GhVvHs/f2yzQUG8pjFjxtQ+V1xWKRbzH3300XRJonvuuaf2vWk0KGj2+vNWXHHFdNx5552XPo57R8THp556at2xPWVQAABAp8Sg4Ljjjitvbukvf/lLts8++6S/y8SZuvEGmjXWWCP7n//5n+w///lPt2Pj9+Sdd96527bhaIMNNsi+9rWvlTcDADDIDAo+ajAHBVFc0ij2X3nllXX78j73uc+lY+IX+HxbPijYd999646P3nnnndqldp555pna9lavp9GgIBb1Y9v8889fd3ze22+/nW56XN7ebFCwwgorpO1f+MIX0mstPy5/HVHxPgatXn9efL447jOf+UwayEyYMCH1u9/9ru7YnjIoAACgU+JNQVOmTClv7lH8Xh6/a0+cODFdkvOMM85Ivzsvv/zy6ffjz372s9m//vWv2vGrrLJKtv766xeeYXhaeumls2222aa8GQCAQWZQ8FGDPSiIX3Zjf1wmqLwvmjFjRnoHUBxz/vnn17bng4IFFlig4Q2Bf/CDH6T98847b7ftrV5Po0HBU089lY0dOzZtv+KKK+oeE8X3J/Yvuuii3c4oiPsqxPb4C06+LRbu83sQXHXVVXXPFeU3Ho7+8Ic/1La3ev15cSmncePGpeHA97///fSYuNl0+bhWGRQAANApfRkUxN8Z4nffyy67rLwr22OPPdK+adOm1bYZFAAA0BODgo8a7EFB3Fg3v6FxcTE9ine/5/cZiHcFFRfM80FBtPvuu6d3DuX74vI9iy++eNoX9zfozetpNCiI4syF2L7IIovU3Xg57kmQfw1xinNxXyzOx/a4SXFxe9wYObY3uilx/IUo/9qi4v0bWr3+Yttuu206Nj9r49prr607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JxkUSF0GBQAAdE4MCk466aTyZgAAGDIGBVKXQQEAAJ1zwAEHGBQAANBRBgUjtCuuuCLbbLPNskMPPbRuX3964YUX6rZVIYMCAAA6Zf/9989OPvnk8mYAABgyBgUjtKlTp2azzDJLtskmm9Tt60sPP/xwtsEGG2QnnHBC3b4qZFAAAECn7P/1r2ennHJKeTMAAAwZg4IR2kAPCuLshHg+gwIAABhaXzcoAACgwwwKRmgGBQObQQEAAJ2y3377GRQAANBRBgUjpD/84Q/Z66+/Xvu43UHBu+++mz3//PPZH//4x7p9xXozKHj77bdH3b0MDAoAAOiUfffdNzv11FPLmwEAYMgYFAzzYuF+iSWWSIv448ePz9Zaa63s2muv7XFQ8Nprr2UHH3xwNnny5GzixIm1x37iE5/IDjjggOzVV1+tHXvzzTdnyy67bO24BRZYIH18yCGHdHvOZ555Jttll13Sc4wbNy4dO+ecc6bPccYZZ6SBRPl1jKQMCgAA6JQYFJx22mnlzQAAMGQMCoZxxxxzTFqQn3XWWdPifdxsOBbnx44dmwYGjQYFjzzySLbUUkulfXPPPXd6zBZbbJEts8wyaVu04oorZu+88046/qabbsqWXnrpbI455kj75ptvvvRxDBry57z88suzueaaK+1fdNFFs0033TTbaKON0lAhf86999677vWPpAwKAADolH322Se74IILypsBAGDIGBQM06677rpszJgxaTBw9dVX17a//PLLaeE/X6AvDwp22mmntH3zzTfPXnnllW77zj333Nrjis8ZNbv0UFxmKIYDse/www+vDRiiN998M9ttt93SvgkTJozoyxEZFAAA0CnxphuDAgAAOsmgYJi23HLLpQX4I444om5f3K9g0qRJdYOCGCLEu/zjDIQnn3yy7nGxyJ+fBXDkkUd229dsUBCXJoqzDRZffPGGlxf6xS9+URs+TJs2rW7/SMmgAACATtlrr72y008/vbwZAACGjEHBMOyNN95IlxeKxfe4EXF5fxT3GigPCvJikFDeFsWgID8b4dBDD+22r9mgIK98dkJevNa4xFE8Ni5jVN4/UjIoAACgU2JQEPf9AgCATjEoGIbdc889aeE9LjtU3pd31llnNR0URHF2wR133JH+wrH//vtnW265ZTbPPPPU3v1fvllxq0FBNGPGjOyGG25Ix+yxxx7Z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>

[image2]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAMMAAAFSCAYAAABPMmv4AABA+klEQVR4Xu2d97cd1Z3l+U96+jdPu3tm1nhCz+phuqfbBmNs3NgGZNNywFiNWQSDJSRBg4AmY/CAyUHkIEAIEYUlEEkEoQAoIQESQRIGEQy2RKbmfeq9XfrefU/dd+/Te0/33Xv2Wt91cqhT313nVJ1Qe3z55ZdFlC+++KJBPv/880o+++yzUj799NNKPvnkk0o+/vjjSj766KMG2bFjR1uyffv2LD0ofp/rxPUGiXolXYs6KL2Muup67Hqewh7tEMFJ4MqfUvjYEH/+859r5U9/+lOWPhTXA5cUkZwcTgwnhevzcISoyOAJIxFSJIgESCm9LvrDDz+s5IMPPsiSpVairqSIE8mRIkYkRbuEiKQoyeAJ6ojQigSu/PEi//jHP1by/vvvt5T33nsvSw+K3+eURD1xkkRi1JHCCSFSuH7XkqGOBCKC9wYiQewBpPxR4dUI7777boO88847tbJt27YsPSx+v6O4nkQSRYKkiCFSeC/RatiUIkRFhuF6g0gCJ8Bf//VfF3vssUeWLGMu6JoTI0UK7yXaIUQDGbxHaEUEKvTyyy83VTZLlvGQKVOmlDrYDiHaHTKVZGhFBCcBjKTr8splybI7RMMoJ4UTIvYQtWTw4VEdETQkYhznFcqSZXfKrbfe2jB0qiPEcMOlkgytiBB7A15svCJRpvz7rOIrk3+QJcuoC7rl+hYF3URH2yFEXQ+xh78w6x2hkx7hG9/ap6nyWbKMhaBrrn8SfX1CZzVkiu8Qww2XKjLUEUGfSQ899NCmwhGvbJYs4yGuhwg6GnsIJ0Sr94eSDKnhUfxipLkBLxj5b1N+3FTJLFnGS1wfEeYz0Fm9Q6DL+srkwyV/fyjJED+hxvcEegSI8PbbbzcVmodGWXa3pIZMX/3qV0udRXf1lanu/aGJDOoVNJcQh0cwLEUExCuWJcvuENdLBJ3VLLYPl1K9QwMZ/OuRiECX84c//KGpsP/wl3/ZVKksWXaHoIuun+ishkvosuYgYu+Q+rK0h4ZI8aVZa4pg2JtvvtlU2Nd+MbmpUlmy7A5BF10/0Vl0V8Ol+LnVh0oNZPB3Bb00q1fYsmVLU2FeoU5l70umFt++5vhi39nHF9+66oRinytOKL55+QnFf/3Vz5riZskynLh+orPoroZLeplOfVlqIoO/K+ilGYa98cYbTYV5ZdqR/znjkOK7N88s9rtxZvGd6wfkuuMDIY6vCPHNS/+t+Kfzpzelz5KlTlw/0Vl096233ip1OX5q9aFSJERFhvgFiV6BjLZu3Vq8/vrrTYV5ZYaTfzj3l8U/3zpjgAwziv1umlF854YZJSG+fe3MYt9rZhbfunqADFcOEeKyE4q9Lz2h2OviE5ryyZIlJa6f6Cy6q3eH+GWp1WfWPVJDJPUKmzdvLl577bWmwrwyreS7N/26+N4d04v9b5s+QIjpFSHUQ0RCVD1EJkSWDsT1E51Fd/XuEF+kWw2VKjLEIRK9goZIr776alNhXpk6+cFdxxU/mDe9+P7c6YEQgz3EdxOEaBgydUAIsGDpU03+3ShvDTylgNzfmXlsgztL5+L6ic6iu/QOGirpRTrOOTSRIb4vaIikF2e6m40bNzYV5pWpkwPuPq44YH6KEANyiwjROGTaSYjjdxLiktaEqCPDsvXrigeeebJyX3LX7aW5YsOLDfFIO+mU46tw5PK77yzWvbaptP/3f/1xQ5jsv7tzTpMfpuSb045sKAcR5M5k2HVx/URn0V16h/iZtdWcQwMZtBiPhPQKkIHu5pVXXmkqzCuTkoPuO6448N4BKQkx3Qgxo9h/zowBQsxMv1TbkImXas8/SooM4LOBC4zK56jzu+fJx0v7lm1vV34yoz3lRxqlm/KbMxrqNOPyi0r/jz75uPhPP/th6ZfJsOvi+onOxqFSXKJRRwZ6hz18oi2+L9DdjJQMkx6YVhLioBpC7Pj042L7gJQ9BO8REOKG+q9Me7foHUCKDG7vxO+6BfeVIr9PBxpLYa++ubU2LaL18XLHOIeec1pD/EyGXRfXT3RWQ6U45+DvDW2RgbGW3hdSWzu9Mi5/M+Wg4ocPThsgxHHFpPsjIXYOmYTBHgJCDPUQKUJcOUgIL0cCRpsMXob8U/Gj/d+vv6rskTyt4hCmHgu/TIZdF9dPdBbd1VelOjL4e0NJBn95Fhk2bdpUvPTSS02FeWVc9r70sOKHv59aTFoAIeghphUH3nNc+Q7BS/X37zyuVAAQvzI1vVTPjl+Zjm8qRwLeePut4qr75pfy1Z8cWPodc9H5xX1PPVEpm8xod+CHsn4w0C6pNO7+1nFHN/gDhkDIX/34gCoudWF4FNMyTs1k2HVx/URn0V2RAZ1mqJSab0iSQStUSaiX55GS4UcLfz0gUwcIMW2ohxAhplWEENIv1WlCeDnDCQr4/ROPa/KPcuDJMyt7VEpemk+8+rKm+C6nXndVk1+W8RXXT5GB9wZ0WWSIC/d88i1JBv+StGHDhqbCvDIukx44pjj4oaklIX5UQwjh+3OP20kIDZmqr0wzGuYhvJzRkPlLHq3qMufhhU3hWbpfXD/RWXRXZIiTb22TQZ9VeXneFTLsc+Vhxb8snlr8y0PTioMXTRsixHHlO4S+MgnlO8Sdgy/V37u99VcmLydLFsT1M5JBn1d5bxiWDKk5Bs0881Y+EjIgkx+dWkyGEA9HQgy+VEOIFL5/x4xAiJ0v1fsNvVR7GVmyIK6f6Gz8vNoxGeJK1UiG9evXNxXmlUnJjx+fOkiIR6btJMTCnYSovjLxYj302fUHAz1EihDfvWlm8Q/nHNFUhmT1pldK86gLf9MUNhpy9s3XlabKydJd4vqJzurzaiRDnHhriwxxTdKukOEnj/+6+PFjg4RgyFS+QywafKne+ZVpcMikl+rmmeqdSzc8/yj/6/CfFc++uLZSVkyEl+AYD79fnn9WaS5a9kzpd+zFvy3+z5G/KGeccf/NzyY15IHbyfD8yxtKu+YMFBc7fqs2vtxUl1iP3z/7dIO/x1m+fl3pfvyFlZX/dQvubYjHJ9zoXrLq+dJO2bgXDM28p8rx+kx0cf10MsQ1SsOSIe5hGC0yIElCpL4yDRGi1dINz9uFCTLM//jjA4pL588t7X7TcUMGTysFeXjFs5UyobBSWifDcwNkiO4Yl3o8s3Z18Vc/ObCKc9LsyxvKUxnI5NNPKiXmJzn/tpsqO2SQXfGYKZedT8gxDDLE/LgGuX9+9r83lDPRxfWzFRnivui40WfMybDPlVOKnzyRIMQiSNFMiMEhUzMhPN+URIWTsunmH/H/zqncdWTgM6xIgR89BuYdjzzURIblG9Y1uL857agq7g2/v7+0o6j/5ec/qsrYd/qvGsrDfP6VlwbzW9+YnyRFhn/81WENPYau9a7HH2nIAzIsW7+2Sk8Pp7CfnnlKQzkTXVw/u5IMyNeO/VGSEI0v1YOE2PkOASGOKwnh+bUrKI37dSoHzGq/fA2vkINO2fmyj796iSgsDIxuH9K5iAz/+ZDBNU3IXr+uf4+SxHr1qrh+di0ZkH2u/NcBQkxtIETLl+qhIZPn088Sh0lZGsX1c1TIELd6igwvvvhiU2FemXbl4EXHVISY/EgzIX64YJAQni5Lllbi+onOphbrdRUZovzf3/x8QPmPHSDE1GK/G48oF/d5nCxZ2hHXzwlHhixZRktcPzMZsvStuH5mMmTpW3H9zGTI0rfi+pnJkKVvxfUzkyFL34rrZyZDlr4V189Mhix9K66f40oG4mfJ0i3i+pnJkKVvxfUzkyFL34rrZyZDlr4V189Mhix9K66fmQxZ+lZcPycMGTjiL0sWF9eTTsT1s6vJwMVyZo3+Ipoli4v0YyTkcP3sSjKIBLrYjIxWiLrSCSFcP7uODFwMebKvOiOjE6Cs6E67hHD97CoyiAgUkpExEqA77RLC9bNryKChEXllZOwKpMDDEcL1s2vIoKPtMzJGAzpK3vWs68mg4RE/h8jIGA208/7g+tk1ZIDJFJaRMVrQL6hc37qaDHpX4F9lExWfbX+7eG/pzIEG+qy89ozdD3Sq1VDJ9bNryDDcEOnUU09tcH/ta19rcLeDdevWleZI0kak0q++7jvFH1dfXuxYdlCxcdNrxWOPPVb8adkRDXGULpW+Dvfff7979S06aTeATrWae3D9nPBk4Nx87NOnD/4WNzaY26My7rfffsU3vvGNZDg44ogjKvekSZOa8op4e82i4qPnJhdv3LVv8cqDFxYfLTuw+OKLL4pX5/xTQzyl22effSo3Mnny5GLGjBlN+QInw8KFC0tz1qxZ5c0gzSGHHNKQdsqUKcm8hMcfH/x5O0oiEP+0004r7Vxv9JfpeXKN+MV7g1vXx69kn3nmmYY89txzz4a4MU/lN2fOnNJ97bXXlu65c+dW8TtBT5PhqquuqiQ2MDj88MMb3BdccEHxwgsvDCYewooVK0pTca6++uripptuKu67777yRxQxTCakufvuu0u7bmTqprz+xOzig2d+Uny85vDioxU/Lj5e9fPixZv3bYijdDRkdGPSwLTZkUceWcUHdWQ48cQTKzII1O+hhx4qr13uFPwa47XeeOONtWRweBjpAQSgbP6eecUVVzTEQTeiGwWjTKD0CtPDystpFxOWDPwyqBXqegZMCT+nA9Qj1XBOBsBTOeahsEguD/O8H3tsSbHtwW8Wa+48ZYAMRwz0Ej8vPnlxevH2gr0b4nk6uc8+++zKzxW4EzJg19M11tfh1+F5tEsGFCEilotABoG4sU5eJvjyyy8b3DGv6N8u0Km+IwPg53QxjKeT47zzzivN2KiQgSc/1xHDRAa6fD25FMawJOJ3v/tdcdFFFxVv3LlX8fGLxxUfrz2m+HDJ94oXr/i7hnh+M+XuhAyxd0qRgfryqyW5AW3s8OEK4El8++23F7Nnz24K87pHP5kaHomQkQyKgyJFN/eeMoGTgV47ulN1aIWeJcPpp5/e4FbDUDnshx56aBXmCiWkhjlSbMKifxyu+Bg8dVP0lPzjw/sW25dOKtZf87cWozmd3Oeee27l53UnjgToXebkk08u/ymWqhfmtGnTGtwO98N94YUXNrghR6s8UF78zz///MoPt65BQyKguN7rxOt1Muy///6lvVUdWqFnydAuUOJOG63X4Z+saR/v3UYCKW+3ou/JkJEhZDJkZAwhkyEjYwh9T4bly5eXZpxQm6jYlXefHTt2NJjDQV95xgO6R60wGvev78mwZMmS0twVReoFdPoFRp9jdxX+sp6C7lErtFvvVuhZMqhxNEsJ+BR46aWXNnx+czIoLDau3HwPj+7DDjuswc31RMifpRBAnx7jJ1sJ39xlguuvv76hHiif3HyV4Vu73Mx9KL+Yb/SPeaUQ08p04WYK1Ofggw8u/fVUfuqppxrKkZ1Pnt7uQvTjc3cqDvdIn7L1SZy2x+2z0ErvebSDniVDVFTW8WzZsqVyC9QjRQZh/vz5De5UHL7d8w3fofIFZrNnzpxZ2pkQpNyYj5aXyE9LJBw06jHHHFNNPIFYL5aMCHFNk8BMdAquPHKjyILWc4HYM3i7LF68uJz5TrUdoN2F2DPEOQQmJYXYM5APaUTAAw44oPKPptvbQc+SAVAOSy5olFRjgVZkuOuuu5riC6+//npDmBYACkx2RTz33HOVMkGeuCANcF1AfnFiKvpTTisyxNlgX6sDxoMM7u/2iDoyXHLJJZW9FRmifzTd3g56mgxqDJQvNtZZZ51VNeZwZOCC8Fu0aFEVxk1jyTVuGoLhF09+Zp4jCGchXMw79gixLCcD5q233trgZvUoZisyyHz00Ueb/AFk4GZHP1Dn7pQM8+bNK02tLYpx6C1ciQHDLeD1FpwMMlNticlyFYV3gp4mw0TG888/714ZbcCJ1AkyGTIyhpDJkJExhEyGjIwhZDJkZAwhkyGBdl7C/CuGwD7e+HkzwuMOh3a+hniebJvU5GAn8M1Qo41dzd+vs85vV9CzZKASbldah6+zUSPHPdFMrgF9F1ee8YY8++yzTWQgnvYCqByldbfbRQbaJ4KZXoHyWU+k+gnkw5yEkNrJR1qVh7KuWrWqIVwTlYC8Yt2A3NqnsHLlyhjccOKhyBDTLF26tAqP0HbbCLUzeiKgWAL64PXrFD1LhqikKDWz0DwxtYMKUA/g374J943pzE0AZqWjf8r0nkGz0T4jfO+99za4/VACyPDggw82xYlumZdffnmZf1RgEVdxtDxDiG0ku+/u09bX1BqiWAcRm81SpGG+AEydOrU0IQPxUAjugw5NiHUAqYlCuUUehTFLfd111zXNQo8UPUsGQP6ugNHeigxub0UGrkFPPq6jXTJEUFf3r5tskkR/2VNkWLBgQUMaIbpVf07+AFoLpDityOB7slGAVD3VDieccEJTuNDK3+2QIeU/UvQ0GfxmRH+g84C8EXH7U1WzpHHNU8pkz66TQU+uVmTAz5dKOBlo0OiOpmZ8Ixm4qUDDJV9DFevhZFCY9lt3QoaYr+zqGTiYLQ6Dtm7dWtkBM/3A2yiVJ2RgQaMv1hspepoM3Bg/cSE2mI59SfUMjJ9jXD3NfGgjk5uKnbVQdN0RWmnZ6qb5xn4Qx/mxvHgdsivv2C6Kw34A7Oecc04VBrTUBJxxxhmlqWEZQx3C4hjd6y136oACwlim4vnLrUMTuJ8RvqlfwE3doj8rYQXemzxNp+hZMkykjf4Tqa7dCJHHe75O0bNkyMjoFJkMGRlDyGTIyBhCX5EhfmmJX2bGE3EiLKO70Bdk0Msp2xGj2+3jAZ+lHSuM5LqUZiRpW4EJz4mAniaDvjLEm6xN+VEeeeSRaoO54rKrCzs71SgrhsUJqThXgWg+IpYTIXcsPxUe7Yq3adOmBv84W4vET5wxf80Oy00behy5UYTox5m10S2k0no8uY899tjKr5vRs2Twm5IyU34axsQtjgpjEowZ6DgnQNiyZcuqU7i19VPf/X2xnZe3Zs2ahs3/LFVA2GPNt/lWda1buuB+1Jc92eTpYdHtJtCZRZ5GuOyyy0ozhrMllnvrBwN3OzIZgh+Ki1B5J4PCUHwnAxNUvhAOUihNhNeBBvKZZ8I8XrTL9HVEEZ4uXoPqhB+9ouc7XH5yMwmmb/sxnL3j/CBG0Ax8t6NnycAeYhaJaSYVuOl+F198ceWOZOBm6hwjLtzJIFPnBskNcVJKFM0UGcifGW9AuzFTfsMNN1Sb80nL9XleEX6NWqCoQwXkr18/xTSYDz/8cJU+hkU3/4LwtAAyyC+2f7ejZ8kwkRH/SZAxfshk6EL4mUsZ44NMhoyMIWQyZGQMIZMhI2MIPUsG3+I4UkyULyEZu46eJwOb9CPiHmPOC2UHl68XihvuuRiZlKvZXEB66hPBBQvUMbozuhs9TYaf/vSnDd/6Mfn/c3SfeeaZDTvd8Esd2ovJSdpyn3LKKeXSC2aepfDYmU1mPoCZ2bVr15bubv/LZcYgepoMghSY2VatGYr+wGdJ9dP0VFy5ycvzY3IOsCAvujO6H31FBt9sHhV8zpw5pTl37tzS1OKyVFx386MRLjKGxaFX/PFGRveir8iAKUm5QTzGxNNGcGiXp5Wbla4aaimcJRZazJfRnehZMrQDV/CM/gY9fN+SISMjIpMhI2MAUmR0y/UtkyGjr8D++G3bttX2Cl1NBv0qNiNjV8EOQPQR3ZywZEid/5mR0QnQQY4GpVdoNUTqejJs3rzZry0jo22gh+gQujRcr9C1ZKDSMJk8MDMyOgHDIoT3hHaJ0NVkIB+IQBdHPlwceWXJUifoCLoCCfgAg/60SwTE9bMryIBEQnBh5JclSytBT+gJ0D9+sdVqTiElrp9dQwaEC+GCyDNLlnYEfREJOiEC4vrZVWRAOJ+HY004AkUXSH784wz7008/XS6lRhQuUZxW9iy9Ja4/nYjrZ9eRQYICy86+A0iCnVWonDHk8SEJh2DJzQ/3ZOfcH4+fJYvrZ9eRARJIor/IwK41levp2AWndPx+CjtLudn34OVkyeL62XVkuOeee8rzSjndLfqLDLfccktpciJdDKcOMRwy8LXh6quvzmTIkhTXz64jQ5Ys4yWun5kMWfpWXD8zGbL0rbh+ZjJk6Vtx/cxkyNK34vo5Ycjgky1ZsiCuJ52I62dXk4GL1XQ75WTJ4tLTyzEQXZguNiOjFfSw7KmFeohIkPc1ZHQKlBXdaZcQrp9dRQYRgUIyMkYCdKddQrh+dg0Z9H5AXhkZuwIp8HCEcP3sGjJABDZoZGSMBibsgQAaHuXjYjJGC+28P7h+dg0ZYDKFZWSMFibsIWLkkc9NyhhNoFOthkqun11DhuGGSKeeemq5R0HYHSdu85sr6tEK7dTr5ptvdq9Rxbp16yp7O/XZHfBfA/B3pNHGhD14uB0y0HAoJFAj8hMR7P6nHsAPShQvfqU666yzGsK5OKD/L5x22mnVPMchhxxShYkM2F9++eXBzIbC9tlnn8oe/TA5xQGT9gH6xxwNi/8zzzxTutmEhJujT9jaKtxxxx2lO+YtO1i4cGFpzpo1qylc5hdffFHa9RMXhZ1//vkN7phvBNeLEM6mKaB/VtBeDvz5h4XXI4bL9H9fjBZ6mgzAG1cme6Pj/MSMGTOa/tYTFRucfPLJDe54MyCXFEhhkMHjykShPT6AVIceemiD35IlS0rT6yfz6KOPLvd9C7fffntDHG5ujC8ynHjiiaW5YsWK0oxx9ttvvwa3TH7btX79+sq9Y8eO8jocL730Urm7EHgeylvAn/iyR1Nwfw8fDUxYMgx3CnccnvCjQzVe9Jdygdi4scF5LznmmGOKefPmlW5JKg1y3nnnlW62ocZhUkwj0V+CYjjgGqOfyCDIPz61nQzqKbyOoB0y6KeMqXrzBI9+KUi5geLQgwl1Q7NUe6T8PVx+Kf920bN/7olKz5PTG/G6664rf0Ul8NQ/7LDDGuLQKLFx657M4Le//W3llrLUkQHwNOUfc+4P2iUDJteB2YoMGvJ5/eROKWaKDGD+/PnF2Wef3VBf8ledhRQZZMa/qwIeINQJcnpcHmTR7eZoomfJcPrppze41Xh069inTJnSEA74na03cnTrZm3atKkpDOgf07GsM844o8FPdlfIGK6fI8pP7whCjCuli+8MDAHj/67jWBwcccQRpVvDPuD1cDLIrt5Ebh9OCdxTQWHLly8v7RdeeGEVJujLoOIuWLCgtMf3s2jGIeZooWfJ0A9AGSS7G7tSB16wdR3xw8V4I5MhI2MImQwZGUPIZMjIGELPkiE1qdYuqDAvv0ici2gH/qVkrLArY3RBX2rqwAuvo93rS6UdDu3mDfz+dpK2Dj1Lhk7AkZIR+sQ61hivcuqgWfA6+CfdiOHI2CptHYbLM0Jf44RO0tahZ8mgJ0VspDijjFCx1NcYueu+bEyfPr1Kp2UPSiOTWeSUP1i6dGlTue4WIAz+s2fPTuan8OiP0M6yp/IFWv6h8MmTJze4UWh9lo35axkIUteGdWmjG+XwcMDnaOZoWIbiecudIoMEXfM07aDvyMD3d28c7xkIp56yA46vR6gnZBD8O7tMlb948eIGfwAZgE/yuT3C88ekYVNKITDfIKBc/MNC1wEUl+UVEdw4EJ/uRx55ZGl6PZj0u/fee6t4Qiqt4HlEf8TnHACz5prd9zB3y6620VzFcOg7Mgh829bKRyfDFVdcUdm90UEkw6RJk0rTb/Dhhx9emhx7H/1BKzLUwfPHTE08RTcz0QLvPw4Nk7RMQmk16RcVmom6GMfLZRLz3HPPrdyptL7myvPAzSRiXTiz/IKHRXdM7/FaoS/IwI1B8SEDywl4Yjz22GPFlVdeWcWJIC7C2h9/qoGRkkEL6EQGxaVOrIylzsyCp+D5R5Prc3/ZtcIzhRQZ6D0UX/lec801Tflj0obMSKtN40tzXVraQ26e9KyCxc39lz/k0fCLBZQM33Arj7hsQ8DNGrILLrigXPMF4oLCdtCzZOikETJ6E+hIJxvAepYMGf0N9SSdIJMhI2MImQwZGUPIZMjIGELfkoHPp6ntiqMBtg/yAh/loosuatjpBepe8uv8U1D+GbuOniYDp2NEhSetNq1EkJ9PzFCfiLh5BmzYsKHMrxWikooMcaOODiugoWJ5MZ0Tlk32W7duLe00NHFj3TWfwE/ggW8MWr16dYNbUF0E5hrIPyK6oz3uavN2VLzh2qob0LNkkEJpwzrfnuPMpp7SbMuEIHqag7rtnXyX14kPgAuL+5AdToa63W0pk1ni1MZ5wfNyf5DKF2hTv6CZXdp06tSpxZlnnlmFcdKGECcjmX8hnxtvvLF0K2/VGQWR/+bNmwcTdTl6lgyAG+GKIMSJpigRdWlbpYmIYXGY5Plqgi76p/KNfp6HEMmgY108XyTGUw8Ty62rA1tFtfwiVZ8UGSYKepYMWlIAtGhMYOmAKybQ8ENwhVu2bFnx0EMPNaRpdWRNjNcpGWgXV6SU8nmc4cgg0I6C/DnIGXtsO2Z/IwiP+WkY52VoiYvXr5vRs2QA3Ig41MCtZRoxfbzBEdEPe9zIHtOgPPHYGSGmv/TSS6syXXHqFsHRZiwviPC6er0jGZTW48dN/dE/rvb0cgSGRXE5CkSO8S6++OLSrYPDUnl0K3qaDBmji9SK315CJkNGxhAyGTIyhpDJkJExhEyGUQLX1ClooIzuQSbDLiAe2NvpBnj/ZAlGSg72Rw+H1HIQRzyjtR208/+JiYSeJQMH8cbPg9qRBuR3/fXXN8SJG/3jlsxUHM03yB9TO+fkjunjMoi777678mcpg3ZuoVjxfxLKAyW97LLLSrdIFDfzRzLEEy/ip1XIwAwydvn7oQUs3dB/JuTPzYuQP+fNxv9PAGbN4zmxOqBY4TLBmjVrittuu60hfHejZ8ngDZwig87eoXwQv58rDlsJgX42EuOkjnKPm+2vvfbaUvFjuCA3ZNBciMgQ4zIvAhl0kLIrFktMIhlEpvjjFa4BMlx11VWl2/MAbPcU2vlTEGlFBogqP+p73333lcruUHn+n4tuQc+SAXBT1eApMkhRAU+0FBnivl6GGcORQUoC2EeNkjGEisqmeAAysE8YRDKQRuJHzANtrgc+TOLJTzx6EREtNQMeTyL34Y5OzI4nbDDhhiJrf3McJtF+qaNhSC9iQFwmGCMJ1Ft1A3qWDDQw3T4LzwB2LZaLN+vWW2+t3BoCxf8PYN55550NcYQ486xwFu7Fm4td5yRFyJ0igw4IgMwcEJAiA6Y2+zsZ8NM7jOKnyBDziKB8FD8emgBYwEed2KRPmtT/J7inMX+fqMOuf+1hZ/jo5e8u9CwZ2oG/LEZFzxgbdIvip9DXZNCaf0E/FskYG0AEXpq7FX1NhoyMiEyGjIwhZDL0GD7/svPzgjIGkclgoOI33XSTew8LxsMjSdcuhvv/wLyXjiqOn/f3xbS5f+tBGW2iZ8mgjfE615T4vuk9TgyhzFTcwe62CI5Jd5CO9Nr1pQk6oAMIYlmxHNlT9QMK1yHJjs8+H/x97+m/3684+cE9i08+HdmSjoweJgPzCcwwa9kE38OZeNPyAvz4nh6/iUth45IIP9RX/yaIp1aQTmTCZOZZaXSqdCSRwgD/guZbvOrHP6sjFNf/svPF50Vx0t1/X8ya94/FafP+uXhn++DOsoyRo6fJIETlw44CClp6EOP4EzoqtuBHuChO/BsPs7UxjcC6HraQHnzwwaXb6xcht5Pk13P+R3H64r8vPv98sB6vf7Dzp+gZI0PfkYEnLJWjHiD1H4c6Msgk7zoyyGR4RG+QIgMgnqeJdhrSw1rh96/s/DdCxsjQF2TQOhtXOkRk0CpQUEcGzhDCzsXVkYEneCyrjgycXBGXfSsNDRbdymc4UjyyceeZRhkjAyed9CQZxgIoJAvPhlPM4cAaoV3Nw/Fl0f5/CDLSyGTIyBhCJkNGxgA4AhO9RLdc3zIZMvoKDF3Z5VfXK3Q1GVod65iR0QnQQx6u6OaEJUPqd64ZGZ2AYzDRRXqFVkOkriYDeQx32kNGRiugxOiQFLhVr9C1ZKDSnBhN1waztcQiI6MVUEh0RsrLqet6aR6OCF1NBi6Aro2Lg918DSC/LFnqBB1BV6S0PFDbJQLi+tkVZEBECC6I/HiHgBhZsqQE/UDQFR6i6GEnREBcP7uGDAgXIlJkydKuSG9cn4YT18+uIgNCekzO38HkIrFzYBbuxYsXN6WRXH755cPas2SRuH52HRkkrsAiA7vPCOP8nxiOP0upqQduXRh29ix4/lmyuH52HRn4ayXnH9WRoU6IL8HNwVZyZzJkSYnrZ9eRQQrMS1H0Fxn4XzMHDDtZJJy0hwkZMCFCJkOWlLh+dh0ZsmQZL3H9zGTI0rfi+pnJkKVvxfUzkyFL34rrZyZDlr4V189Mhix9K66fmQxZ+lZcPzMZxkm2bl9bvPbRs1nGSLy92xHXz0yGcRC/cVnGTrztW4nrZybDGMrW7S823awsYy9+H+rE9TOTYQzFb1KW8ZH3P3in6V6kxPUzk2GMxG9QlvEVvx8pcf3MZBgj8ZuTZXxly/bVTffExfUzk2GMxG9OltGR9zfMavKrE78nLq6fmQxjJH5jsoyOfPLizOK1Pz/V5J8Svycurp+ZDGMkfmOiPLtxQZPf7pCjpk1p8htN8fzPu+zU4oGnbyntnFru8dtpl0/Wz2zyqxO/Jy6un5kMYyR+Y6Kce8nJ1b8acC9/7fcN7qgohx31s8q+8o1FDfEUF7nl/stKt8xjjz+8NP/3nn9XxbnzodkNaX75q0NK9+U3/6YpX+SVD5+q/GPdPG6dW/m7f10+3i4uHz49qewZ3vr9t4u3XzqzeOPNOU1xovg9cXH9zGQYI/EbE+U3l51SmlExMOctvqaYfccFxT9+/R9K99Mv3d+QzpVk8iEHNYWlyBDjPPPy/cWrO5Y2pPF8Pc9of2jF7aWpp77HSeUvqesZTjprWml6u0g+efHo4uN1R5ZE+HjtUcX7j+w3YB5ZvLvw2w3xXPyeuLh+ZjKMkfiNiaLhwF77fL00ufkQAbnvyZtKv4XLb2tSCuSauReW/mvefrRJETFFhl/N+GVpOhmkcMg/f3+nMumpHMvy/J/f8lDlFik8Tl3+SB0ZZPd2kXz84nEDRJgxYM4oPlzy/eLdRd8qPn7h58WOJfs3xHPxe+Li+pnJMEbiNyaK33SU5sLZZ5RK8eT6e0s/7FJoCfFvfeCK4qwLTyzWv/dE+QTG78ipUyqFwly4bCeRnAwyb3vwygb3ouW3N5Fh45+fKf0kinvHwqsr9/V3XVTMOOXospwrbjkvmb9k7sAwLebDEJBeUD2Jt4tkx7KDi7cX7F188MT3io+W/WjAvlfx0XM/Lrbev29DPBe/Jy6un5kMYyR+Y4aT4YZEkuc2L2pwo7Brtz3a4Pf4mvlN6aK8un1psXTjAw1+T6y7uylerFOsz6Or5jXEe2Hrw5VC1+Uvob7Rvf79J5riNMnmW4p1r8wb0Kvri403/l2x7cG9iu1LJzXHM/F74uL6mckwRuI3phNB8Va+vrDJf3cIdTnksH9p8p8I4vfExfUzk2GMxG9MlvEXvycurp+ZDGMkfmOyjL/4PXFx/cxkGEPxm5NlfMXvh4vrZybDGErez7B7xe+Hi+tnJsM4iN+kLOMjfh9cXD8zGcZJ/EZlGVvx9k+J62cmQ5a+FdfPTIYsfSuun5kMWfpWXD8zGbLsVpk/f35xzTXXNPnfcMMNlZ1/c/BXJo8T/9HBPztkf+KJJ8rf4Hp8F9fPTIYsXSH+Dz79nObqq68uzdmzZzel0Y9pUunRQ4/v4vqZyZBlt8pTTz1V6pD/iSn+tiz1K7K77rqrNPUjzNtuu60hj0yGLBNW6sgg/xUrVjT83hb/e+65pwqHDBBG5MhkyDLhBOV1IiAaHiGEP/DAA5U72iW33357Q9jrr7/eFMfF9TOTIUvfiutnJkOWvhXXz0yGLH0rrp+ZDFn6Vlw/Mxmy9K24fnY9GficJnnvvfeyZKkk6obrTTvi+tmVZIjKT/4IhWZkRKATH3zwQakfkRyuT3Xi+tl1ZIgk4EIzMtqBk8L1KiWun11FBhFh27Ztfq0ZGW0B3WmXEK6fXUOGTISM0UK7hHD97CoykNfHAwVlZOwKUNZ33nlnYpJBvQL5ZGSMBt56661hewfXz64hA0zmAjIyRgvD9Q6un11DBsZ5O3bs8OvJyBgx0KkJR4Z2hkiffvqpe40I3/jGNxrMscLy5cvdqyVozwgeDFFAJ3Xmho0XOr1W4ZhjjnGvUQU6hW65vnU9GYYbIp166qnuVa55r0NdGKdKR3NXcNhhh7lXle+SJUsspBmxDnX1+fzzzyt7XZwINsGATogzUnRyrSlMnjzZvUYVw703uH5OWDKsWbOm8ps+fXpx7bXXljdn2bJlVRgbPOS3//77l3GdDG4Kp512WnHppZcWe+65Z0OcVatWleYXX3xRTJo0qSxL4BoIww8Fwb5+/fqG9Gxsj26l9/IFJ8Pq1auruDfddFNxxx13lHWkvcmLHV/ck8MPP7yMc9lllxVr164t03z55ZdVXtzUqVOnlu3yu9/9rmwr6k+9iUeeZ599dnHkkUdWaciDjTaYGzdubLhWhQOURO0NYtufc845pX379u0lGX76058Wxx57bBl28sknV2nq2qMTTFgy/OEPf/BraYCTAejpHxtOdu8ZtJwjKmLKFDzPqJQHHHBAabbbM9Tl7WWk4GRIgRujIYd6BuGII45IPrlTZWN6GZAehff2BH6tKEv0FzRkU/733Xdf6Y49g9LwsAHPPfdcFTZSoFOZDDVh0R39mcpfunRp5QaeZ1RKoVMy1Jmt0IoMclP/OjII++yzT/HQQw9Vbs9Lfqm6QYbrrruucgt115rK+8ILLyyJNWXK4C+3QIoMmAcffHDlvyvoKzKoAVEYvwnY6eLlz02IaTxuCvgvXLiwIU0sZ8OGDU1pFe4KEsPknjlzZrI+Ea3IwPAGv4svvrgiA+6ouI8+OvgjRE8L5P/YY4+VwxWBfCEPYbx7xKEccsghhzS4U9fqiP4MwUCKDOeff35tHp2iZ8kwlkg1vvxEtIz2sKttxXvYli1b3HtEyGToENS7DnTrGe2Dl+JuQiZDRsYQMhkyMoaQyZCRMYSeJUPqa9LuBEsQmCxqB3qpjOaDDz5Y2WmvXcV+++3nXhWYQGyFWbNmudeYQPML44W+I8NLL71U2fUCFz9HUifARQjxW3z05yKjmwslT/wQXx+liTzqTsM4KJs5AJGAPIiHW3lykrTyxS6oHswMAz7jClqrxMw6oI7KM4UUGTjwV+BTqafl2lAiQLtwn2NY3f2K9QTx/ogMsaw4K672BPFzbYyPEraLviEDCn/jjTeWdn/yalqf2VfF9TjDmYClBwJLEyL4/HfRRRc1PJGjIsyYMaP6GuV5xzI04yo/zh6V25c5aIkF3+lF+FSeDieDZtCVptXkoUzut9pR18lyDgEd8LkczSfIDRnifIagSTYv002gOY520DdkOOGEEyr7ueeeW5pqND2lYyPGhpUAHTqQaniRAaWOT1IgMoCYn1BXtodFMkjuvPPOpvQS1gRJyRQWzRQiGbQ2KtY5RQZ+IAJivjzlY1ov0/2ZCMSu9U2pNPIHkGnevHlVD8KM+c0339yQJpOhaCYDCiplVWPJFBkYYtB4TOR4nLgoLKVcKDv5MyRJ3UCRIYYtWrSosp944om1T++YxnsG2pX2jHFk1xM5VV+ZkJvFgRHeM6g3U5rUu08rMmjdUAw75ZRTmhYdqmeWGyVnSHj00UcPJhoC9z/Wwa9JJkqYyTCA008/vWwUCWDYgN0XiMWxvT/5GZdjZzWnEG8qJMPNjeMfAbHMs846q4pHfVnVCgiLCip4fd0EUiDGzvi7ogJuAO5DDz20dKfIwHsQ9hdeeKFpHZHXQySO7yixPKA8or9e9FmF6vEBSzfig4dhFHa9t8WPBo7ot3nz5tKNUsZwHk4airWDniXDSCElmDNnjgdldAm4P48//rh77zIyGTIyhpDJkJExhEyGjIwh9CwZ9G18pKDy1G0kqNtPXOc/2uCfxmOBTut/wQUXuFdXo2fJwBk47cK3KHLT2UjD1wg2u3QKzQI7Ul9FRgtjmbfQThkxjn/e7nb0LBn0FIs3x3dcUTHZ6+A9jHZ0sbEesvBpUFA+0UTqZkwFbXCHlNTxt7/9bRWmuEx0YdenVPKMdY92LTORn3aIya143IfoHg6ePvqxwy+6wbRp05riA2bno7/sTIbqOj3NeKDvyMB3dW9o7xkEjwf0zZ6lHa3IkMoT/7r5BcAcQooMTMbpeuLSiDg/EusKGWL5EBgoDu3HJF/d5n8+W/KNX9/5hViGK2y8dkEkrPtMrbVFMU2nQ7HRRN+RAWiibO7cuaU7pbhsSKeuEVyMJrJQolZkOO+88yp/wRUo+gMaLkUGhnyYlLl48eKycQGzuCklhAxacgI0g6s4XAdkAHfffXfpH/9twb1hqOfDvViGX0uqHhom+epT4tD2PgMtO9eJ6DrHC31BBhqWWVAUbf78+eXTmU3tV155ZRUnAjfrY1D2uPhOYdo0TxizsszQXn/99U0KgckapZR/BG6ewpjUkbZiiCFFVRyuI7pZ4hHdZ5xxRmmPwyQ2/3u5IoNOwLjkkkva2oJJel6KWUPE/dIsOG0ay5DytyJD7KFlyh7rPJ7oWTKMdWNSbyfKaKCTtTQZo4ueJUNGRqfIZMjIGEImQ0bGEDIZMjKGkMlgiBNUncDju7sTpNKm/CIUzjbJ4eKOFbS3ejh4nPgZWqduAz6/anfgeKBnycB3cyoi8M1ckzz6ni9QvuBkaHVKHlsqBcXnopkMU9mY1EX5aEO7dqwJ8ah65aUN/NEP+JZSoPKIF6872uPn05hHjKM2AqqrHzwQN+XHfPgcHfOK10S76HqcDHJrZhpwfD4QGfx+P/vss6WJovk1jxQ9S4bUAbyUoRukfbwKY3kDCutkcFOQO8bnOqQ4nk4zvmyF9A32KbNuC6i2n9bVx/05MEAbYZRv3cEI3NT4ubhVXYGHacM/8woeFtN5HWMcTwcZ9LCSn9aLpfLeFfQVGYAm4+Kmdq3zgSidkAHhuqI7hkdT9ngUipYp8KRFCerSyGSCjPojqfpEMwI/eif2NsdTO7SPWGlSZBBUV8VlVtzrIjLg9jCd1KHwCCYctb0WZdGWXRCHSfKD4DFvz2+k6DsyMNsK/AnEDHWKDFSepzEXHKHlC/FJzUVz5Ivc0SQ+M98omJTMl4y46X7kryUKtF9EKq0Q/ybE5vy6I2lYluJkqKsr0BObewpEBh40CtNy8kiGFMhXwy/sCxYsKO1OBg2P5I7mrqJnyQBcqeKZRVpjxB8eCePJRx10To+ndXBCHv564VMchkN+ugailasoF42Nn8bbWpoQn6zkk6qD/DnCJSKWlwK/7hL8YASt1eK9ikMNhFRdY/5+UEAsw08C8d9bOaJfPJ1DhyiAeI0SoN+P7Sp6mgyjAY5z2ZWG9rRx6DEeoIcc6RKP8a7r7kYmQ0bGEDIZMjKGkMmQkTGEviAD5WVkDIeeJUP8tJra2thr4OsNm33iHzFHA6lDhh2+eacV4qdn0vkHht2JniVD/PSW+iQnoR4xjPwj5K/5iejnx85rzoEdaiCWA1JbRAVtqNd2TE8rUxNjWgeE8H3eyaD4fDb1fdeeN7v+otvjAW5mKg7g82cM4954XLn90OJUfrsLPUuG1KSbzHiqM4qi05+B3xwdqKszgPQ/BOBxvRz9a/nll18uzU7JECG3zxIDjrVxMigfJsviWqLUIcQyqaf/YNyXrbgdKE/uLYjhbAnlPscJNYE6zp49u3LvbvQlGeITXbOz2oTuQyouAOhGM1MtuFKglECnUTAxJ6Co7ZAh/kcC4nndmWyDDNSbJzJlQDonA4j7soWUUqf8hHbIECfG1q1b19CeLM6LE3nx6J3deRJGCj1LBlB3XpGTgacWs9MsaPMbjVub9QXSsPne4wJXmvgjER0eEJdHxLhxgg9z9erVDW6WImBCBkzqi0LVkYE48aEQ/SWA+qievkpXcdjcz4khuONqVMWJbYfCM9HHw0HLWAhjqbbiyK+b0NNkaOfEBwGl8fVHAnWLgDzqKRx+g7m2CBq6Dlp3JHhar4e7HV4XoHckEMO9rBTeeust96rg6bn5kVjYnWj8V6Gb0NNkGG+klG93gbVA+mOOQ6cCZjQikyEjYwiZDBkZQ8hkyMgYQiZDRsYQMhkyMoaQyZCRMYRxIwMBo02GuMxASPk5iEP5lDtawlIG9xsLqSuH66HB69BOu3SKkeY50nRjjXEjAz0DhRCRyZvRIEM7oOHV+JSjC627YEkMHy5uu0I+nlf087CRCHloLVQrxHZJ+XnYSFGXj/u7e3dg3MhAAIVwxEgkAxlx81qRwZWlFRnizZSdSlDpmF8U9/dG8DjuVycxbiqP6E7F8Xh1kopH+2pdVV27RP/oTsXxeHVoJ14sY6TljAXGjQzqGVJkqOsZXDlkj2RI3eRockRLKp+UAkaJ8bz8dtJ4OjdjvFb1qMu/rhyPy/Wn2iWasqcUtA6eR6r9BS+nlen2lF8qHKTieNxUHGHcyODvDJynwxEfww2TXFGwkwcF64L8AiUcA9Ou4rhfKszjeX6pcE/vaVNlpfLxNJ7e6xCFdojtonaKbeaI8VNxU37u9jw8rZt1qIvn7hTq0grRf1zJQCHqGSIZGCax9NcLq7vpw5FBoJKuGFFinnJ7HA/zuni455uK72lTfu4eLu+6+Aht7MrgyhnF/dzdqs2jX0pimMdN2aMZ4XlGvxRa5SVABnQLQqTa1vVz1MnQapjklZECUNlIBjcRDY9iOleSlHh57u91kbvOHKnE8lJlpvJ3v1gXDZdGIo6UfypNyu3+LnXhMb2jLrxV2uiWHZ1Ct+p6B9fPXSIDESAD3TYJRYa6F2i/sbq5IgMXwbJgbzhEL8yuMClFifG2rTu/Ka5LTIP59nvbijPXXdAULxU/JTEM+1vvvtUUp068Lh4uoY1dASSxDWMYSLVvys/zjvkovpcT4Xl5/OhW/FZpPZ6HeThoNUzCz/Vz/fr1FRlYjt4RGSgIMsR3BpEhNUzSjVQFJRRGem8sROvmYaorRBTPU/LHDUdV3STuX6w8tjh05TGlXPLS7GQ6wt569+0m/1blSB7dvKRMr7i/eO7Y4t9Wn9Hg105+8q8Lp61T7aU2k1K44qo9o5+3tefjZircw1yiAiv+cHXxtPF6UnnHMpBWZEBcP9UzbNq0aeRkYJjEriyRgWMMUz1D3Q3WO4M3UmwoyiFdSlx5ov/2135d/GnzA5X70BXHVOEoqEzJM1uXVXbFV7xbNs4tfv38SaXfk1uWDsZbsVPJkVfe3lQs27qy9Lv+5TnFUc/PHCxjqNxYFu5Za84uZq0+u3Rf+tI1DWFqn9S10WbeVrG9hvOTv8T9Y7jbXdr1r8sj1sPLc79WYUgkDDoV3xnUnsORYUQ9AxkzREqRoa5n8BurPNQzuOhidVGe3pWmyX/9CcUfX76y8kMpT137m+KXz00rFVUKf+Mrt5dKSDmV4kbiDNghw0kDiiv3Da/cVty48fZiyeanG8pd/uZzpXnSgKJftP6qwfgDeW97d1sDebBDhjtevbt0n7rmN1VczHjNKalrK4Sdfu4nf/lFeyoPT+d+MY2nS9XFw1N18bgxH9nr/BABu8ggAgxHBg2TNg31DOikk4HdlkkycEMiGfjKQUaQYe3atU2F6QZHUR6RDDRIbBTs5C8liGkRLhD3O2/tfGHC/dmHJxfvLv9JQ3xXcPwPX3lcFe5kUFqR4cw1FzTkE+sh97ItK0v71nferPKo8lzeWD69wvxX7y/jnLL63CquX6OXRXuojVqZrlzRry6e3C51+Xhe0fRw9/P8U/m6O5LPiVHXM0QSiBSun5CBIb7IQHp0mzz4YMHcWiQDf3QqyUCmFIIiMzYTGTZu3Fhs2LAh2TPoBkdRHqQn41QjIeTpaV12vHpS8fEfphfvvzK1+Oj1U4s3lx5SvPn4dxriHLr8V4OCcr9y56DfgB0ljYqrukX/m1++oyQD9me2LBsMGxCGcLGMZ7esqJRX5c1adfbOsoYE90mrztpJhjVDZFi+kwwS5SehPbyNENrQ3XVtisQwT1snqfxSaVN+qbR1YXJHIrhfJIMLyhyH195DuH76CzR6Tc9AHi3JoK5ei/RQZn1W5UalegYyleJEBSIPkaFOeIH29FGUV+necGOxddUlxTtvDz4ZmsItnYd7XE83XJjnFf1/vuxXyXCP634u+qcdiqE2ivaUpOJK8eSvG5ySdvOPeXqZnoeHu11pokRyRHcUSMJog/ZLESE1TEJvnQz0DKRvSQYy46ZojoHEZELPAMM4fsQLoweIQnoNs1B2Mk7dDPlBGKVx5fB86/zc3+vi7lQ5bno8z8f96uKn8nV/hPaO7YIZJbZbyp+xLm5MjXs9Tav8Y15+j1JphvN3SeWLOMGcIJEYkQwiBNJuzxDnGYYlA5lxY5wMrXoGVwiEwsiD9Lo5sWHkh/C272lT+bmfiyubp1V4XV74e5i7Yz4uqbh14nXBpB1iu3i7RWV3RXO/VB6pOB4/VY7Xw/OoC4txUu5IDhGkVS8iYujhGXsHjWhSZEBveZgz3I/DJNJDoloy+PsCTOLFQz1DigwUIEUSCTA1YUcBEhoimhLeRSiXtFKOVJ5RUvHcT+k8vftHM9bB86uTVDz3U96pMiFCql3kF8X9PV3K7qbnn3K7v/xS4bF+KUnFiWSSW6SQpHoN9JK2jT2DBJ1z/RQZ0EWRgfTeM+zYsaMkREUGCuAGkUATbpCBngEycHqcF4ZwQzUWk5AeNtIQYp3sUeQHIbjQmEcr8fJahbnb/evCh5NO0xPP40IEb5PYLm5vpy29zaOk8vP07va6tBMvFRalFUlcYg8iMtA7OBlcLyMZ0EV0kvYnLb2I/kMOEZBIyj30NNPLM2QgIy3FqCODbjLpZNfLtxpFzJM9JZCRT7jkE/MaicT0yi8qJILby/GyPbwd8XI8P4SbRLu20y4e7m75ebron0qjJ2JdPI/fjp+XE/NyQtRJihjqNTQSUe8Q3x9cLxF9VkWX9bAVGTThRv1UbkUG9QrcLArVZ1XNPkOG559/vqlAzhKFdbrR2Lds3lJWgganQEzJcG4Yy8s65WFKcHcinsbdLh7u5cY6eVpP18qPsSrX7Nc9nJubJj/sMSyVztPXSTt1cWm3LjE8mpE4KfFeQ6RIkQEi7L333k16+ZWvfKUkAw9lyIBeigzcAw2TkmTQE40CtalHcwy8L3AjOQ7RC0X23XffknkSCmd4RWEuYmT0czdxPJ3HaeUf/VJ5xTBP7+6U1MVJ+csPcyLVxf1S+bkQxyX6O1EiOZwkqd4CvURPNVTSy7TrI1L3JSm+PFMnJwPvJnuoV5Ay82SHWVqKsWrVqrJnOOigg5oKRiCRiER60tKoUdTQIxWlh9Uehp/7uzuVV0pahbnUlet+raRVea3CXFLlpvxaSavyWoXViRNGSigypEhSN7RCryADSi0yuB4inO4uMjDCQSdTSzEoO/ZEFRkiEdQrQATNMUAGegb+N+CFS77+9a9X6elRNF0eJTVZws0aLo6HSXSzZa/LMyWpcurS6aUrulN1Gc5eJxOlLl5Oqi4xPmaUVkTxHsR7CxSbhzZKvddeezXpn4RhffyShF6TTl+SqBflUQb5xiFSSQbNLVCg5hciGV544YWSDPzcgv8YeAVciO9v/KlPYu4X3R5GQ3tc+cUxZCqtSypcfjFPD6uTTuoynDv6dUNdJKn2rwsXkSKxUmSqI0gkhgiBgrueuTCchwzx5Tm+L4i8yjv2DBUZIIKe6hoiQQQyhgwMkVY+t7LsGZ55+uniySefbKpIliy7U3gAo6v6WqdlGE4GDZFEsqaeASLEXkFk0MszZFixYkXVMzz11FPl32C8Qlmy7A5BPxnKp4ZIenmmx6I3cjL4nMYeIoLmFvTiDBn0vgAZ+FUTZKBngAyPPvpocddddzVVLkuW8ZADDzywWLlyZUkGeoXUEIn3hThEggwafjFEEhm09GMPzTaTEcyiV4AMel+gQIZI6hkgwxNPPFGSYfHixcXDDz9c/gTwL/7iL5oqnCXLaMvTTz1dPph5QPOgRk95cMeVqvqkyhBJ71HeK4gMGiJBhv8PkLBIgo5VAogAAAAASUVORK5CYII=>

[image3]: <data:image/png;base64,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>

[image4]: <data:image/png;base64,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>