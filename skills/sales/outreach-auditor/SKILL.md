---
name: outreach-auditor
description: Review your past outreach and get exactly 3 actionable changes. Analyzes what's working, what isn't, and what to change — based on data, not guesses.
disable-model-invocation: true
---

# Outreach Auditor

Most founders don't track their outreach. They send a few emails, get silence, and conclude "cold outreach doesn't work." The problem isn't cold outreach — it's not knowing what's broken.

This skill reviews your past efforts and gives you exactly 3 things to change. Not a list. Just 3.

---

## Prerequisites

`.sales/context.md` must exist.

---

## Flow

### 1. Gather data

Ask:
- "What outreach have you sent? Paste emails, DMs, call notes — anything."
- "How many prospects have you contacted total?"
- "How many replied? How many led to calls? How many led to deals?"
- "What did prospects say when they said no? (exact quotes if possible)"
- "What feels like it's working? What feels like it isn't?"
- "What channel performed best? (email, LinkedIn, Twitter, other?)"

Read `.sales/outreach/results.md` if it exists — don't re-ask what's already tracked.

### 2. Analyze: quantitative

Calculate their numbers vs benchmarks:

| Metric | Yours | Benchmark | Verdict |
|---|---|---|---|
| Open rate | | 40-60% (cold email) | ✅/⚠️/❌ |
| Reply rate | | 5-15% | ✅/⚠️/❌ |
| Call booking rate | | 2-5% of sent | ✅/⚠️/❌ |
| Follow-ups sent | | 80% of sales after touch 5 | ✅/⚠️/❌ |

### 3. Analyze: qualitative

Read every email/DM they sent. Diagnose:

- **Too much about you?** — Count "I/we/my" vs "you/your". If it's 50/50 or worse, that's the problem.
- **Generic or specific?** — Does it mention something real about the prospect, or could it be sent to anyone?
- **Ask too big too soon?** — "15-min demo" is high friction. "Quick question" is low.
- **No follow-up?** — Most replies come after touch 2 or 3.
- **Same objection every time?** — "Too expensive" = value unclear. "Not right now" = pain not acute. "Using competitor" = not differentiated.

### 4. Find the ONE bottleneck

```
Sent → Opened → Replied → Called → Closed
       ↑         ↑         ↑        ↑
    Low open?  Low reply? Low call? Low close?
```

- Low opens → subject line or sender reputation
- Low replies → personalization, ask too big, or wrong ICP
- Low calls → ask too vague, no clear next step
- Low close → product-market fit or pricing

### 5. Give exactly 3 recommendations

Not 10. Not 5. Three.

```
Here are 3 things to change starting today:

1. [Immediate — change before your next send]
2. [Medium — change this week]
3. [Strategic — change this month]
```

If the founder pushes back on a recommendation, defend it with evidence from the analysis. If they have a valid reason, adjust.

### 6. Write `.sales/outreach/results.md`

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

### 7. Close

> "Your bottleneck is **[X]**. Your reply rate is **[Y]** — it should be **[Z]**. The #1 change today: **[one specific change]**. Do that, send 10 more, and come back. If it improves, great. If not, we'll find the next bottleneck.
>
> Run `/outreach` to implement the changes, or `/icp-definer` if the data suggests your ICP is wrong."

---

## Completion criterion

`.sales/outreach/results.md` is updated. The founder has 3 specific, actionable changes — not general advice — and knows exactly what to do next.
