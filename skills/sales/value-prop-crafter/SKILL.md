---
name: value-prop-crafter
description: Craft a clear, differentiated value proposition by researching the market and grilling the founder on their real differentiators.
disable-model-invocation: true
---

# Value Proposition Crafter

Founders describe their product as "a CRM for dentists" or "an analytics platform for SaaS." These aren't wrong — they're useless. They tell the prospect what the product does, not why they should care.

This skill finds the one thing only you can do, positions it in a category where it wins, and produces messaging you can use everywhere — landing page, cold email, sales call, pitch deck.

Based on April Dunford's positioning framework (Obviously Awesome) and Geoffrey Moore's category-creation playbook (Crossing the Chasm).

## Prerequisites

- `.sales/context.md` exists. Use `_engine` procedures for all workspace I/O.

## Flow

### 1. Research the competitive landscape

Before asking the founder anything, do web research:

- What categories does this product fit into? Search each one. Who wins in each category?
- Who talks about solving this problem? What language do they use?
- What positioning do competitors use? What's their tagline? Their "why us?"
- Find at least one competitor or adjacent player for each potential category.

### 2. Present the landscape and grill

Report your findings:

```
I researched the market positioning landscape. Here are the categories this product
could play in and who owns each:

1. [Category A] — owned by [leader]. They position as [their positioning].
2. [Category B] — owned by [leader]. They position as [their positioning].
3. [Category C] — no clear leader yet. This is interesting.
```

Then ask:

- "Which of these categories feels like the right neighborhood for your product?"
- "If you had to pick the one competitor that keeps you up at night, who is it?"
- "What do customers say when they try to explain what you do to a colleague?"
- "What's the one thing your product does that, if you told me, I'd immediately say 'oh, that's different'?"

### 3. Run the positioning exercise

Walk through each dimension with the founder, pushing for specificity:

**A. Competitive alternatives**
Ask: "What does your ICP do TODAY to solve this problem?"
- Score each alternative: "Nothing" (0 pain), "Manual process" (some pain), "Competitor" (switching cost), "Hated workaround" (best case for you)

**B. Unique capability**
Ask: "What can your product do that no alternative can?"
- Reject "faster" and "cheaper" — push for the defensible thing
- "We're the only one that works offline" ✓ — "We're the fastest" ✗
- Dig: "You said 'better DX' — what specifically about the DX? The API design? The docs? The onboarding?"

**C. Category choice**
Ask: "What category makes your strengths look like strengths?"
- If your strength is automation, don't compete in "project management" — compete in "workflow automation"
- If your strength is simplicity, don't compete in "BI tools" — compete in "analytics for non-analysts"
- The category determines who your competitor is. Pick wisely.

### 4. Generate value proposition options

Write 3 distinct positioning options. Each must include:

```
Option 1: [Category-focused]
One-liner: "We help [ICP] [solve problem] by [unique mechanism], unlike [alternatives]."
Why it works: [psychological hook — emotion, curiosity, social proof]
Where to use: [cold email, landing page hero, pitch]

Option 2: [Outcome-focused]
One-liner: "Get [specific outcome] in [timeframe] without [pain of alternative]."
Why it works: [psychological hook]
Where to use: [cold email, landing page hero, pitch]

Option 3: [Contrarian / underdog]
One-liner: "Most [alternatives] do X. We do Y. Here's why Y matters for [ICP]."
Why it works: [psychological hook]
Where to use: [cold email, landing page hero, pitch]
```

### 5. Test each option against real psychology

For each option, score it:

| Criterion | Option 1 | Option 2 | Option 3 |
|---|---|---|---|
| Does it trigger emotion, not just logic? (System 1) | | | |
| Does it create curiosity? (would they read more?) | | | |
| Does it imply social proof? ("used by companies like yours") | | | |
| Can the founder say it naturally? (not corporate-speak) | | | |
| Does it differentiate from the alternatives found in research? | | | |

### 6. Write `.sales/value-proposition.md`

Use `_engine` write procedures:

```markdown
# Value Proposition: <Product Name>

Last updated: <date>

## The Winner
[one-liner that the founder chose]

## Competitive Alternatives
[what the ICP does today — from research + founder input]

## Unique Capability
[the defensible differentiator]

## Category
[the category where this product wins]

## All Options
<all 3 with rationale and scores>

## Tagline Candidates
<3-5 short taglines>

## Voice & Tone Notes
[How should the founder sound? Technical? Empathetic? Direct?]

## Research Sources
<sites and searches consulted>
```

### 7. Validation

Ask:
- "If a prospect in your ICP read Option 2, would they say 'tell me more' or 'so what'?"
- "Read the winning option out loud. Does it sound like you?"
- "Where will you test this first — cold email or landing page?"

If the founder hesitates on any question, refine. The winning option should feel true, not clever.

## Completion criterion

`.sales/value-proposition.md` exists with at least one positioning option the founder feels confident enough to test in real outreach this week.
