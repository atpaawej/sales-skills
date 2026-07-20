---
name: outreach-auditor
description: Review past outreach attempts and suggest improvements. Analyzes what's working, what's not, and how to iterate.
disable-model-invocation: true
---

# Outreach Auditor

Reviews the founder's past outreach efforts — cold emails, DMs, calls — and suggests data-driven improvements.

## Prerequisites

- `.sales/context.md` exists

## Flow

### 1. Read workspace and gather data

Read `.sales/context.md`. Ask the founder:
- "What outreach have you sent so far? (paste emails, DMs, call notes)"
- "What were the results? (opens, replies, calls booked, deals closed?)"
- "What feels like it's working?"
- "What feels like it isn't?"
- "How many prospects have you reached out to total?"

If they have `.sales/outreach/results.md`, read that too.

### 2. Analyze the data

**Quantitative (if they have numbers):**
| Metric | Founder's number | Benchmark |
|---|---|---|
| Open rate | | 40-60% (good cold email) |
| Reply rate | | 5-15% (good cold email) |
| Call booking rate | | 2-5% (good from cold) |
| Close rate | | Varies |

**Qualitative:**
- Is the email about them or about you? (should be mostly them)
- Is it personalized or templated? (specific references = higher replies)
- Is the ask low-friction? (5-min call > demo > "buy now")
- Is the follow-up sequence working? (most sales happen after touch 3+)
- What objections are you hearing repeatedly? (that's a positioning problem, not a pricing problem)

### 3. Provide specific recommendations

- "Your subject line is too generic — try [specific suggestion]"
- "You're pitching too early — move the ask to message 4, not message 1"
- "Your reply rate is low — here's what's missing in the personalization"
- "Everyone says 'too expensive' — that means your value isn't clear enough. Strengthen the ROI statement before defending the price."
- "You're not following up enough — here's a 5-touch sequence"

### 4. Update `.sales/outreach/results.md`

```markdown
# Outreach Results & Analysis

Last updated: <date>

## Stats
- Total prospects contacted: 
- Reply rate: 
- Call booking rate: 
- Close rate: 

## What's Working
<Keep doing this>

## What's Not Working
<Stop doing this>

## Recommendations
<Actionable changes>

## Objections Heard
<Pattern → Root cause → Fix>
```

### 5. Give the founder 3 actions

"Here are 3 things you can do differently starting today:
1. [Immediate change — e.g., rewrite subject line]
2. [Medium change — e.g., add follow-up sequence]
3. [Strategic change — e.g., refine ICP based on who replied]"

## Completion criterion

`.sales/outreach/results.md` is updated. Founder has 3 actionable recommendations they can apply today.
