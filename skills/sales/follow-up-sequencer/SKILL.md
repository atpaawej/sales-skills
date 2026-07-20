---
name: follow-up-sequencer
description: Design a multi-touch follow-up sequence. 80% of sales require 5+ touches, but 44% of salespeople quit after one.
disable-model-invocation: true
---

# Follow-Up Sequencer

Most sales happen after the 5th touch. Most salespeople quit after the 1st. This skill builds the persistence strategy that becomes your competitive advantage.

Not "send more emails" — **send the right messages at the right time on the right channel.**

Use `_engine` procedures for all workspace I/O.

## Prerequisites

- `.sales/context.md` exists. Initial outreach was written (run `/cold-email-writer` or `/linkedin-dm-writer` first).

## Flow

### 1. Read workspace and calibrate

Read `.sales/context.md` using `_engine` procedures. Read `.sales/outreach/sequence-01.md` if it exists — build on the existing emails rather than starting from scratch.

Ask:
- "What channel was the initial outreach on? (email, LinkedIn?)"
- "What about your prospects? Are they busy execs? Indie founders? Developers?"
- "Do you have any content you can share as follow-up? (blog posts, case studies, tweets, frameworks?)"
- "Can you reach them on another channel? (email + LinkedIn > either alone)"

### 2. Design the touch sequence

Build a 5-touch sequence with actual message text:

**Touch 1 (Day 0): Initial message**
Already written by `/cold-email-writer` or `/linkedin-dm-writer`.

**Touch 2 (Day 3): New angle / value add**
```
Subject: Re: [original subject]

Hi [Name],

Following up on my last email — I know you're busy.

I wanted to share [specific resource] that might be useful regardless of fit.

[1-2 sentences on what the resource is and why it's relevant to their situation]

No need to reply if this isn't the right time.

Best,
[Your name]
```

**Touch 3 (Day 7): Social proof**
```
Subject: Re: [original subject]

Hi [Name],

Thought this might interest you — [similar company/person] was dealing with [same problem] and they [specific result] after [action].

[1-2 sentence story linking their situation to the outcome]

Worth a quick chat to see if you'd see similar results?

Best,
[Your name]
```

**Touch 4 (Day 14): Break-up**
```
Subject: Re: [original subject]

Hi [Name],

I've sent a few emails and haven't heard back — completely understand.

I'll stop following up for now. But if [specific problem] ever becomes a priority, the door is open. No catch, just wanted you to know.

Best,
[Your name]
```

**Touch 5 (Day 30-45): Re-engagement**
Trigger-based: reference something new that happened.
```
Subject: [trigger event — funding, product launch, role change, post about pain]

Hi [Name],

Saw that [specific trigger event]. Made me think of our conversation earlier — might be worth revisiting if the timing is better now.

Let me know if you'd like to pick it up where we left off.

Best,
[Your name]
```

### 3. Cross-channel strategy

If the founder has access to multiple channels:

| Touch | Channel | Content |
|---|---|---|
| 1 | Email | Initial message |
| 2 | Email | Resource share |
| 3 | LinkedIn | Like/comment on their post, then DM |
| 4 | Email | Break-up |
| 5 | Email or LinkedIn | Re-engagement based on trigger |

### 4. Write `.sales/outreach/templates/follow-up-sequence.md`

Use `_engine` write procedures.

### 5. The rule

"44% of salespeople give up after one follow-up. 80% of sales require 5+ touches. This sequence is a competitive advantage. The only way it fails: if you don't send it."

## Completion criterion

`.sales/outreach/templates/follow-up-sequence.md` exists with 5 complete touches (text written, not placeholders). Founder knows when to send each one.
