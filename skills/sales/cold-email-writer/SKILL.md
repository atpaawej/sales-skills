---
name: cold-email-writer
description: Generate personalized cold email variations based on the ICP and value proposition. Uses the 4-sentence formula and P.A.I.N. framework.
disable-model-invocation: true
---

# Cold Email Writer

Generates cold email templates personalized to the founder's product and ICP. Based on the 4-sentence formula from the course and the P.A.I.N. framework.

## Prerequisites

- `.sales/context.md` exists
- `.sales/icp.md` exists
- `.sales/value-proposition.md` exists

## Flow

### 1. Read workspace

Read `.sales/context.md`, `.sales/icp.md`, and `.sales/value-proposition.md`.

### 2. Ask for context

Ask the founder:
- "What's your target prospect's name and company?" (if specific)
- "Do you have a specific trigger event? (they posted something, launched a feature, got funding, etc.)"
- "What channel are you sending through? (email, LinkedIn, Twitter/X DM)"
- "What's your goal for this outreach? (book a call, get a reply, get a trial signup)"

If they want a *batch* of emails for cold outreach (no specific prospect), proceed with the generic template approach below.

### 3. Apply the 4-Sentence Formula

Every cold email follows this structure:

| Sentence | What it does | Example |
|---|---|---|
| 1. Who you are | One sentence, plain English | "I'm a solo developer building tools for fintech teams." |
| 2. Why them | Specific to their situation | "I saw your post about PCI compliance headaches." |
| 3. What you offer | Value, not features | "I built a tool that handles compliance checks in CI/CD so your team doesn't manually audit every deploy." |
| 4. The ask | Low commitment | "Would you be open to a 5-minute call to see if this fits?" |

### 4. Check against P.A.I.N.

| Letter | Check |
|---|---|
| **P**ersonalized | Does it reference something specific to them? |
| **A**udience-aware | Does it sound like you understand their world? |
| **I**mmediate | Can they scan it in 5 seconds? |
| **N**ext step | Is it clear what to do? |

### 5. Generate options

Generate 3 distinct cold email variations:

- **Option A: Curiosity hook** — "Quick question about [their specific situation]"
- **Option B: Pain-first** — "Still dealing with [specific pain]?"
- **Option C: Social proof** — "We helped [similar company] achieve [outcome]"

Also generate 3 subject line options with rationale.

### 6. Write the sequence

Save to `.sales/outreach/sequence-01.md`:

```markdown
# Outreach Sequence 01: <Target Segment>

Last updated: <date>

## Email Variation A (Curiosity)
**Subject:** <subject>
**Body:**
<4-sentence email>

## Email Variation B (Pain-first)
**Subject:** <subject>
**Body:**
<4-sentence email>

## Email Variation C (Social Proof)
**Subject:** <subject>
**Body:**
<4-sentence email>

## Follow-up Sequence
**Day 3 follow-up:** <new angle>
**Day 7 follow-up:** <case study / social proof>
**Day 14 break-up:** <break-up email>

## Best Practices for This Segment
- Send times
- Personalization tips
- Length recommendations
```

### 7. Remind the founder

"Reminder: The agent can write the email. Only *you* can send it. Pick one variation, personalize it for 5 prospects, and send them today. Come back after you get replies."

## Completion criterion

`.sales/outreach/sequence-01.md` exists with 3 email variations, follow-up sequence, and subject lines. Founder has been reminded that sending is their job.
