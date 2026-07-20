---
name: call-prepper
description: Prepare for a sales call — research the prospect, build a discovery question set, and create a call flow.
disable-model-invocation: true
---

# Call Prepper

Prepares the founder for a sales call. Turns anxiety into structure by giving them a clear plan before they dial.

## Prerequisites

- `.sales/context.md` exists (for product context)
- `.sales/icp.md` exists (to tailor questions)

## Flow

### 1. Gather prospect info

Ask the founder:
- "Who is the prospect? (name, company, role)"
- "What do you know about them so far?"
- "What's their relationship to your product? (cold, inbound, trial user?)"
- "What's your goal for this call? (discovery, demo, close?)"

Use web search to research the prospect: LinkedIn, company website, recent news, posts.

### 2. Write the call flow

```
## Pre-Call Research Summary

**Prospect:** [Name], [Role] at [Company]
**Company:** [Industry, size, relevant context]

## Call Structure

### 1. Rapport (2-3 min)
- Reference something specific about their work/company
- Keep it genuine

### 2. Discovery Questions (10-15 min — 70% listening)
Open-ended questions to ask:
1. "What happened that made you take this call? What's the trigger?"
2. "How is [problem] affecting your team/company today?"
3. "What have you tried so far? Why didn't it work?"
4. "What would ideal look like for you?"
5. "Who else is involved in this decision?"
6. "What's your timeline and budget?"

### 3. Solution Presentation (5 min)
- Connect their pain to your solution using the value proposition
- Don't list features — show outcomes

### 4. Objection Handling (5 min)
<Pre-write top 3 objections and responses>

### 5. Next Steps (2 min)
- Clear ask: "Based on what you've shared, I think [next step]. Does that make sense?"
- If yes: set date and time right there
- If no: ask what's missing
```

### 3. Pre-write objection responses

Based on the product and prospect, write responses to likely objections:
- "It's too expensive" → value reframe + ROI calculation
- "We need to think about it" → "what specifically needs thinking through?"
- "We're happy with current solution" → "what would you improve?"
- "Not the right time" → "when would be the right time?"

Use the **Feel-Felt-Found** method from the course:
1. "I understand how you feel..."
2. "Other customers have felt the same way..."
3. "What they found was..."

### 4. Save to `.sales/calls/<prospect-name>.md`

```markdown
# Call Prep: <Prospect Name>

Last updated: <date>

## Pre-Call Research
<Summary>

## Call Flow
<Structured flow>

## Discovery Questions
<List>

## Objection Scripts
<Objection → Response>

## Next Steps
<Desired outcome>
```

### 5. Send prep to founder

"Here's your call prep. Read it in 5 minutes before the call. During the call: listen 70%, talk 30%. After the call: send a summary within 2 hours."

## Completion criterion

`.sales/calls/<prospect-name>.md` exists with prospect research, call flow, discovery questions, and objection scripts. Founder feels prepared.
