---
name: linkedin-dm-writer
description: Generate LinkedIn DM scripts — connection requests and gate-question messages that get replies.
disable-model-invocation: true
---

# LinkedIn DM Writer

LinkedIn is the best cold channel for B2B founders. But most DMs sound like spam: "Hi, I saw your profile and think we should connect." This skill writes messages that get replies.

Based on Alex Berman's gate-question technique: ask something easy to answer, build rapport first, pitch later.

Use `_engine` procedures for all workspace I/O.

## Prerequisites

- `.sales/context.md`, `.sales/icp.md`, `.sales/value-proposition.md` exist.

## Flow

### 1. Read workspace and research

Read `.sales/context.md`, `.sales/icp.md`, `.sales/value-proposition.md` using `_engine` procedures.

Then research the prospect the founder wants to reach:
- Use web search to find their LinkedIn activity, posts, comments
- What are they posting about? What's relevant to them right now?
- What's their role and what problems would they likely feel?

Ask the founder:
- "Who are you reaching out to? (specific person, or profile type?)"
- "Do they have recent activity we can reference?"
- "What's your goal? (reply, call, trial signup)"

### 2. Write the 3-message pipeline

**Message 1: Connection Request (300 characters max)**

```
Hi [Name], [specific compliment about their work]. Would love to connect.
```

Rules:
- Reference something specific — a post, comment, article, or mutual connection
- Zero self-promotion
- 300 characters max (LinkedIn's limit)

**Message 2: First DM (gate question)**

After they accept, wait 24-48 hours. Then:

```
Thanks for connecting, [Name]. I really liked your take on [specific insight].

Quick question — are you still dealing with [specific pain] at [company]?
```

The gate question must be:
- Easy to answer (yes/no or quick clarification)
- Relevant to their world (not your product)
- Low-friction: no pitch, no call request

**Message 3: If they engage**

Only introduce your product after they've replied to the gate question:

```
Since you mentioned [pain], this might be relevant — I built [product] to [specific outcome]. No pressure, but if you're curious: [link or 5-min call ask].
```

### 3. Write `.sales/outreach/templates/linkedin-dm.md`

Use `_engine` write procedures:

```markdown
# LinkedIn DM Template: <Segment>

Last updated: <date>

## Connection Request
<template — 300 characters max>

## First DM (Gate Question)
<template — with placeholder for their specific activity>

## Follow-up (if they engage)
<template — introduces product naturally>

## Reminders
- Wait 24-48 hours after connection accept before DMing
- Pitch only after they reply to the gate question
- The gate question filters: a reply = warm lead, no reply = not acute pain
```

### 4. Coach the founder

- "Alex Berman got 40%+ reply rates using this method. His secret: ask a question, don't make a pitch."
- "Connection request is 300 chars max. No links. No pitches."
- "If they accept but don't reply to the gate question — follow up once in 5-7 days, then move on."

## Completion criterion

`.sales/outreach/templates/linkedin-dm.md` exists with a complete 3-message pipeline. Founder understands the gate-question technique and has the templates ready to send.
