---
name: call-prepper
description: Research a prospect and prepare a structured call flow — discovery questions, objection scripts, and next steps.
disable-model-invocation: true
---

# Call Prepper

The thought of a sales call makes most technical founders anxious. "They'll ask something I don't know. They'll see through me."

Reframe: a sales call is just a structured conversation. Your job is not to pitch — it's to discover whether you can help them.

This skill researches the prospect, writes a call flow, and preps objection responses so you walk into every call with a plan.

Use `_engine` procedures for all workspace I/O.

## Prerequisites

- `.sales/context.md` and `.sales/icp.md` exist.

## Flow

### 1. Gather prospect info and research

Ask:
- "Who is the prospect? (name, company, role)"
- "What do you already know about them?"
- "What's their relationship to you? (cold reply, inbound, trial user, referral?)"
- "What's your goal for this call? (qualify, demo, close?)"

Then research using web search:
- Their LinkedIn profile — recent posts, activity, background
- Their company — what they do, recent news, funding, challenges
- Their role — what they care about, what metrics they're measured on
- Any common ground — mutual connections, shared interests, similar background

### 2. Write the call flow

```
## Pre-Call Research
**Prospect:** [Name], [Role] at [Company]
**Company:** [what they do, size, relevant context]
**Triggers:** [what made them take this call/reply]

## Call Flow

### 1. Rapport (2-3 min)
- Reference something specific: their recent post, company news, mutual connection
- Keep it genuine — not transactional

### 2. Discovery (15 min — 70% listening)
Goal: Understand their situation deeply.

Questions to ask:
1. "What happened that made you take this call? What's the trigger?"
2. "How is [problem] affecting you/your team today?"
3. "What have you tried so far? What didn't work?"
4. "If this problem disappeared tomorrow, what would change for you?"
5. "Who else is involved in the decision? What do they care about?"
6. "What's your timeline? What's the budget range?"

### 3. Offer (5 min)
- Connect their specific situation to your solution
- Don't list features — describe how their life changes
- "Based on what you told me, I think [specific outcome] is achievable. Here's how."

### 4. Handle objections (5 min)
<Pre-written responses for likely objections>

### 5. Next steps (2 min)
- Clear ask: "Based on what you've shared, does [next step] make sense?"
- If yes: set date and time immediately
- If no: ask what's missing
```

### 3. Pre-write objection scripts

Write 3-4 specific objections this prospect is likely to raise:

| Likely objection | Your response |
|---|---|
| "It's too expensive" | Acknowledge → Value reframe → "What would it cost you not to solve this?" |
| "We need to think about it" | "What specifically needs thinking through? I might be able to help right now." |
| "Happy with current solution" | "What would you improve if you could? Where does it fall short?" |
| "Not the right time" | "What needs to change for it to be the right time?" |
| "Send me some info" | "Happy to — but what specifically are you evaluating? I'll tailor it." |

Use Feel-Felt-Found for each:
1. "I understand how you feel..."
2. "Other customers have felt the same way..."
3. "What they found was..."

### 4. Write `.sales/calls/<prospect-name>.md`

Use `_engine` write procedures.

### 5. Send prep to founder

Deliver:

"Here's your call prep for [prospect]. Read this 5 minutes before the call.

During the call: listen 70%, talk 30%. Your discovery questions are more important than your pitch. If they bring up an objection, use the script — and if the objection is valid, say so. Trust beats winning.

After the call: send a summary within 2 hours. I can help you draft it."

## Completion criterion

`.sales/calls/<prospect-name>.md` exists with prospect research, call flow, discovery questions, and 3-4 objection scripts. Founder can review in 5 minutes before the call.
