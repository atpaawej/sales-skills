---
name: icp-definer
description: Define the Ideal Customer Profile for the product. Reads product context from .sales/context.md and produces a structured ICP document.
disable-model-invocation: true
---

# ICP Definer

Defines who the product is for — specifically, precisely, narrowly enough that the founder can name companies and people to reach out to.

## Prerequisites

- `.sales/context.md` must exist (run `/init-sales-workspace` first)

## Flow

### 1. Read context

Read `.sales/context.md`. Understand the product, the problem, and the founder's initial ICP guess.

If `.sales/icp.md` already exists, read it too. Ask: "Your current ICP says [summary]. Has anything changed since you last defined it?"

### 2. Research and reason

Do the following analysis in your response (use web research if useful):

**A. Who has this problem?**
Based on the product and problem described, who experiences this pain?
- What role or title?
- What industry or niche?
- What company size?
- What specific situation makes the pain acute?

**B. Who gets the most value?**
This is more important than "who has the problem." A small agency might have the problem, but a 50-person company might feel it 10x more.
- Who would pay the most to solve this?
- Who would churn the least?
- Who would implement fastest?

**C. The narrow starting point**
For a pre-revenue founder, recommend ONE narrow segment to start with. Not "SaaS companies" but "B2B SaaS companies in the fintech space, 10-50 employees, who have a dedicated engineering team but no dedicated QA."

**D. Where to find them**
- What communities are they in? (specific Slack groups, subreddits, forums, newsletters)
- What events do they attend? (virtual or in-person)
- What content do they consume?
- What keywords would they search for?

### 3. Write `.sales/icp.md`

Use this structure:

```markdown
# Ideal Customer Profile: <Segment Name>

Last updated: <date>

## Primary ICP (Start Here)
- **Role/Title:**
- **Company size:**
- **Industry:**
- **Specific situation** (the trigger that makes them need this now):

## Why This Segment
- **Problem they feel:** (their words, not your features)
- **Value they'd get:** (quantified if possible)
- **Why they'd pay:** (urgency, budget, ROI clarity)

## Where To Find Them
- **Communities:**
- **Content they consume:**
- **Search terms they use:**

## Outreach Angle
- **The hook:** (one sentence that would grab their attention)
- **The pain they'd admit to:** (what they'd say in a conversation)

## Secondary ICPs (Future)
- <segment 2>
- <segment 3>
```

### 4. Validate with the founder

Show the ICP and ask:
- "Does this feel right? What's inaccurate?"
- "Do you know 5 companies that match this profile?"
- "Would you be comfortable reaching out to someone in this segment today?"

If the founder disagrees, refine. Iterate until they say "yes, that's my target."

## Completion criterion

`.sales/icp.md` is written and the founder has confirmed it's accurate enough to start outreach. They know 3-5 companies or people who match the profile.
