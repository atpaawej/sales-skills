---
name: outreach-auditor
description: Review past outreach and get 3 actionable changes. Analyzes what's working, what isn't, and where to iterate — based on data, not guesses.
disable-model-invocation: true
---

# Outreach Auditor

Most founders don't track their outreach. They send a few emails, get silence, and conclude "cold outreach doesn't work." But the problem isn't cold outreach — it's not knowing what's broken.

This skill reviews your past efforts and gives you exactly 3 things to change. Not a list. Just 3.

Use `_engine` procedures for all workspace I/O.

## Prerequisites

- `.sales/context.md` exists.

## Flow

### 1. Gather data

Ask the founder:

- "What outreach have you sent? Paste emails, DMs, call notes — anything."
- "How many prospects have you contacted total?"
- "How many replied? How many led to calls? How many led to deals?"
- "What did prospects say when they said no? (exact quotes if possible)"
- "What feels like it's working? What feels like it isn't?"
- "What channel performed best? (email, LinkedIn, Twitter, other?)"

Read `.sales/outreach/results.md` if it exists.

### 2. Analyze: quantitative

Calculate their numbers and compare to benchmarks:

| Metric | Yours | Benchmark | Verdict |
|---|---|---|---|
| Open rate | | 40-60% (cold email) | ✅/⚠️/❌ |
| Reply rate | | 5-15% | ✅/⚠️/❌ |
| Call booking rate | | 2-5% of sent | ✅/⚠️/❌ |
| Follow-ups sent | | 80% of sales happen after touch 5 | ✅/⚠️/❌ |

### 3. Analyze: qualitative

Read every email/DM they sent. Diagnose:

- **Too much about you?** — Count "I/we/my" vs "you/your". If it's 50/50 or worse, that's the problem.
- **Generic or specific?** — Does the email mention something real about the prospect, or could it be sent to anyone?
- **Ask too big too soon?** — "15-minute demo" is high friction. "Quick question" or "Thought you'd find this useful" is low.
- **No follow-up?** — Most replies come after touch 2 or 3. One email and done is not outreach.
- **Same objection every time?** — "Too expensive" = value unclear. "Not right now" = pain not acute. "Using competitor" = not differentiated.

### 4. Identify the ONE bottleneck

Most outreach funnels have ONE bottleneck. Find it:

```
Sent → Opened → Replied → Called → Closed
       ↑         ↑         ↑        ↑
    Low open?  Low reply? Low call? Low close?
```

- Low opens → subject line or sender reputation
- Low replies → personalization, ask too big, or wrong ICP
- Low calls → ask too vague, no clear next step
- Low close → product-market fit or pricing, not outreach

### 5. Give exactly 3 recommendations

Not 10. Not 5. Three.

```
Here are 3 things to change starting today:

1. [Immediate — change this before your next send]
   Example: "Your subject lines are generic. Open rate is 20% — should be 40%+.
   Change 'Introduction to [Product]' to 'Quick question about [their specific situation]'."

2. [Medium — change this week]
   Example: "You're only sending one email. Add a day-3 follow-up with a new angle.
   80% of replies come after touch 2. You're leaving money on the table."

3. [Strategic — change this month]
   Example: "Every 'not right now' objection points to ICP misalignment.
   Your ICP says [X], but the people who reply are [Y]. Refine your ICP based on who actually engages."
```

### 6. Update `.sales/outreach/results.md`

Use `_engine` write procedures:

```markdown
# Outreach Results & Analysis

Last updated: <date>

## Stats
- Total prospects contacted:
- Reply rate:
- Call booking rate:
- Close rate (if applicable):

## Bottleneck
<one-sentence: what's the weakest point in the funnel>

## What's Working
<keep doing this>

## What's Not Working
<stop doing this>

## 3 Actions
1. [Immediate]
2. [Medium]
3. [Strategic]

## Objection Patterns
<objection → root cause → fix>
```

### 7. The verdict

Deliver concisely:

"Your bottleneck is [X]. Your reply rate is [Y] — it should be [Z]. The #1 change you can make today: [one specific change]. Do that, send 10 more, and come back. If it improves, great. If not, we'll find the next bottleneck."

## Completion criterion

`.sales/outreach/results.md` is updated. Founder has 3 specific, actionable changes — not a list, not general advice. They know exactly what to do next.
