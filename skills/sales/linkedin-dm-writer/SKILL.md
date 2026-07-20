---
name: linkedin-dm-writer
description: Generate LinkedIn DM scripts for outreach — connection requests and follow-up messages.
disable-model-invocation: true
---

# LinkedIn DM Writer

Generates LinkedIn outreach scripts — from the connection request to the first conversation. Based on Alex Berman's gate-question technique from the course.

## Prerequisites

- `.sales/context.md` exists
- `.sales/icp.md` exists
- `.sales/value-proposition.md` exists

## Flow

### 1. Read workspace and ask

Read `.sales/context.md`, `.sales/icp.md`, `.sales/value-proposition.md`.

Ask the founder:
- "Who are you reaching out to? (specific person or profile type)"
- "Do they have a recent post or activity we can reference?"
- "What's your goal? (book a call, get a reply, send them to your product)"

### 2. Write the 3-message pipeline

**Message 1: Connection Request (300 chars max)**
```
Hi [Name], admired your post about [specific topic]. I work on [related area] and would love to connect.
```
Must be:
- Referencing something specific
- Low pressure
- Not self-promotional

**Message 2: First DM After Connection**
```
Thanks for connecting, [Name]. I really liked your take on [specific insight from their content].

Quick question — are you still dealing with [specific pain] at [company]?

[Only mention product if they ask or conversation goes there naturally]
```
- Acknowledge their expertise
- Ask the **gate question** (simple, easy to answer)
- No pitch yet

**Message 3: If they engage**
Only pitch after rapport is built. Use the value proposition naturally:
```
Since you mentioned [pain], this might be relevant — I built [product] to [specific outcome]. No pressure, but if you're curious: [link or 5-min call ask].
```

### 3. Write `.sales/outreach/templates/linkedin-dm.md`

```markdown
# LinkedIn DM Template: <Segment>

Last updated: <date>

## Connection Request
<template>

## First DM (Gate Question)
<template>

## Follow-up (if they engage)
<template>

## Notes
- Best times to post/send for this segment:
- Content they engage with:
- Common objections on LinkedIn:
```

### 4. Coach the founder

Summarize:
- "Connect requests must be <300 characters — short and specific"
- "Don't pitch in the first 3 messages"
- "The gate question filters out non-leads; a reply to that question = warm lead"
- Alex Berman's data: 40%+ reply rate using this method

## Completion criterion

`.sales/outreach/templates/linkedin-dm.md` exists with a complete 3-message pipeline. Founder understands the gate-question technique.
