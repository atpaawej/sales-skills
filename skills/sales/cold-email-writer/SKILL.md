---
name: cold-email-writer
description: Generate cold email variations that get replies — research-backed, personalized to the ICP, built on the 4-sentence formula.
disable-model-invocation: true
---

# Cold Email Writer

Most cold outreach fails because it's about the sender, not the receiver. "Hi, I'm John, my company does X, we're the best at Y, would you like a demo?" — delete.

This skill writes emails that sound like one thoughtful human to another. Not templates — **variations tailored to your ICP's specific situation**, backed by research and psychological principles.

Use `_engine` procedures for all workspace I/O.

## Prerequisites

- `.sales/context.md`, `.sales/icp.md`, and `.sales/value-proposition.md` exist.

## Flow

### 1. Read workspace and research

Read `.sales/context.md`, `.sales/icp.md`, `.sales/value-proposition.md` using `_engine` procedures.

Then **research your ICP's world** using web search:
- What are they talking about right now? (Twitter, LinkedIn, Reddit, blogs)
- What's the #1 problem they're complaining about in their niche?
- What recent news/trend is affecting them?
- What language do they use when describing the pain? (their words, not yours)

### 2. Present the research and calibrate

Share what you found:

```
I researched [ICP segment] to understand what's on their mind right now.
Here's what I found:

- They're talking about: [topic 1], [topic 2]
- The language they use: [specific phrases, words]
- The mood: [frustrated? overwhelmed? curious?]
```

Then ask:

- "Who specifically are you emailing? (name + company, or profile type)"
- "What's the trigger for this outreach? (they posted something, launched a feature, got funding, or just cold)"
- "What's your goal? (reply, call, trial signup)"
- "Have you tried emailing this type of prospect before? What happened?"

### 3. Build the 4-sentence email

Every email follows this exact structure — no exceptions:

| # | Sentence | Purpose | Check |
|---|---|---|---|
| 1 | Who you are | Plain English intro | "I'm a solo developer building tools for fintech teams." |
| 2 | Why them | Specific to their situation | Must reference something real about them |
| 3 | What you offer | Value, not features | "I built a tool that handles compliance checks in CI/CD so your team doesn't manually audit every deploy." |
| 4 | The ask | Lowest possible commitment | Reply? 5-min call? Link? |

### 4. Generate 3 distinct variations

Each variation uses a different psychological hook:

**Option A: Curiosity hook**
- Subject: "Quick question about [their specific situation]"
- Sentence 2 creates a gap they want to close
- Sentence 4 asks a low-friction question

**Option B: Pain-first hook**
- Subject: "Still dealing with [specific pain]?"
- Sentence 2 names the pain in their language (from your research)
- Sentence 4 offers a way out

**Option C: Social proof hook**
- Subject: "[Similar company/name reference]"
- Sentence 2 references a similar situation or company
- Sentence 4 implies "others like you found this useful"

For each option, score it:

| Check | Option A | Option B | Option C |
|---|---|---|---|
| **P**ersonalized — references something specific? | | | |
| **A**udience-aware — sounds like you understand their world? | | | |
| **I**mmediate — scannable in 5 seconds? | | | |
| **N**ext step — clear what to do? | | | |

### 5. Write the follow-up sequence

Each email needs a follow-up strategy:

```
Email sent: Day 0
Follow-up 1 (Day 3): New angle — "wanted to share [specific resource]"
Follow-up 2 (Day 7): Social proof — "here's how [similar company] solved [problem]"
Follow-up 3 (Day 14): Break-up — "I'll stop here, but door's always open"
```

Write the actual text for each follow-up.

### 6. Write `.sales/outreach/sequence-01.md`

Use `_engine` write procedures:

```markdown
# Outreach Sequence 01: <Target Segment>

Last updated: <date>

## Research Summary
<What you found about the ICP's current situation>

## Email Option A (Curiosity)
**Subject:** <subject>
**Body:**
<4 sentences>

## Email Option B (Pain-first)
**Subject:** <subject>
**Body:**
<4 sentences>

## Email Option C (Social Proof)
**Subject:** <subject>
**Body:**
<4 sentences>

## Follow-up Sequence
**Day 3:** <full text>
**Day 7:** <full text>
**Day 14:** <break-up text>

## Best Practices
- Recommended send time:
- Personalization level needed:
- Expected reply rate benchmark:
```

### 7. The reminder

Close with:

"Here are your emails. Pick the best variation, personalize it for 5 prospects in your ICP, and send them today. Don't wait for perfect — perfect doesn't send. If you get replies, I can help you prepare for the call. If you don't, I can help you iterate.

The agent writes. Only you send."

## Completion criterion

`.sales/outreach/sequence-01.md` exists with 3 email variations, follow-up sequence text, and subject lines. Research was done — the emails reference real things happening in the ICP's world.
