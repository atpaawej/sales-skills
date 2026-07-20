---
name: follow-up-sequencer
description: Design a multi-touch follow-up sequence for prospects who haven't replied. Builds persistence without being annoying.
disable-model-invocation: true
---

# Follow-Up Sequencer

Designs a complete follow-up sequence. Most sales happen after the 5th touch; most salespeople quit after the 1st. This skill makes persistence systematic.

## Prerequisites

- `.sales/context.md` exists
- `.sales/outreach/sequence-01.md` or comparable initial outreach exists

## Flow

### 1. Read workspace and ask

Read `.sales/context.md`. Ask the founder:
- "What channel was the initial outreach? (email, LinkedIn, DM, etc.)"
- "What was the initial message about?"
- "How many prospects are you following up with?" (batch size)
- "What other channels can you reach them on?" (LinkedIn + email = higher conversion)
- "Do you have any content (case study, blog post, tweet) you can share as a follow-up touch?"

### 2. Build the sequence

Use the course's recommended rhythm:

| Touch | Timing | Content | Channel |
|---|---|---|---|
| 1 | Day 0 | Initial message | Primary channel |
| 2 | Day 3 | New angle or value add ("wanted to share this resource") | Same channel |
| 3 | Day 7 | Social proof (case study, testimonial, customer story) | Same or cross-channel |
| 4 | Day 14 | Break-up email ("I'll stop following up, but door is open") | Same channel |
| 5 | Day 30-45 | Re-engagement ("saw [trigger] and thought of you") | Cross-channel |

### 3. Generate each touch

For each touch number, write the actual message.

**Day 3 Follow-up**
```
Subject: Re: [Original subject]

Hi [Name],

Following up on my last email — I know you're busy.

I wanted to share [specific resource: blog post, case study, framework] that might be useful regardless of whether our product fits.

[1-2 sentence description of the resource, with link]

No need to reply if this isn't relevant right now.

Best,
[Your name]
```

**Day 7 Social Proof**
```
Subject: Re: [Original subject]

Hi [Name],

Thought you might find this interesting — [similar company] was dealing with [same problem] and they [specific result] after implementing [solution].

[1-2 sentence story].

Worth a quick chat to see if you'd see similar results?

Best,
[Your name]
```

**Day 14 Break-up**
```
Subject: Re: [Original subject]

Hi [Name],

I've sent a few emails and haven't heard back — no worries at all.

I'll stop following up for now. If [specific problem] ever becomes a priority, I'd be happy to help. No catch, just wanted you to know the door is open.

Best,
[Your name]
```

**Day 30-45 Re-engagement**
```
Subject: [trigger event]

Hi [Name],

Saw that [trigger event — new funding, product launch, role change, post about pain]. Made me think of our conversation earlier.

If the timing is better now, I'd be happy to pick it up where we left off.

Best,
[Your name]
```

### 4. Write `.sales/outreach/templates/follow-up-sequence.md`

Save the complete sequence with timing and channel recommendations.

### 5. Reminder

"44% of salespeople give up after one follow-up. 80% of sales require 5+ touches. This sequence is your competitive advantage — the only way it fails is if you don't send it."

## Completion criterion

`.sales/outreach/templates/follow-up-sequence.md` exists with 5 touches. Founder understands the persistence strategy.
