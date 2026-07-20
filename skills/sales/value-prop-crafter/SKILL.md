---
name: value-prop-crafter
description: Craft a clear, differentiated value proposition from the product and ICP. Reads .sales/context.md and .sales/icp.md.
disable-model-invocation: true
---

# Value Proposition Crafter

Turns the product's features into a message that resonates with the ICP. Based on positioning frameworks from April Dunford (Obviously Awesome) and Geoffrey Moore (Crossing the Chasm).

## Prerequisites

- `.sales/context.md` exists
- `.sales/icp.md` exists

## Flow

### 1. Read workspace

Read `.sales/context.md` and `.sales/icp.md`.

### 2. Run the positioning exercise

Work through each step with the founder:

**Step A: Competitive alternatives**
Ask: "What does your ICP do TODAY to solve this problem?"
- "Nothing" = they don't feel the pain enough
- "Spreadsheets / manual process" = pain is real but bearable
- "Competitor X" = switching cost, need differentiator
- "A workaround they hate" = best case

Write down the answer.

**Step B: The unique capability**
Ask: "What can your product do that no alternative can?"
- Not "faster" or "cheaper" — those aren't defensible
- "Only one that works offline" / "Only one that integrates with X"
- "Only one designed for [specific use case]"

**Step C: The category**
Ask: "What category makes your strengths look like strengths?"
- If your strength is automation, don't compete in "project management" — compete in "workflow automation"
- What category does your ICP already search for?
- Can you name a category they'd recognize?

### 3. Generate value proposition options

Write 3 distinct positioning options:

```
Option 1: [Category-focused]
"We help [ICP] [solve problem] by [unique mechanism], unlike [alternatives]."

Option 2: [Outcome-focused]
"Get [specific outcome] in [timeframe] without [pain of alternative]."

Option 3: [Underdog / contrarian]
"Most [alternatives] do X. We do Y. Here's why Y matters for [ICP]."
```

### 4. Test against the course's psychological principles

Check each option against Cialdini's principles:
- Does it trigger an *emotional* reaction (System 1), not just logic?
- Does it imply social proof ("used by companies like yours")?
- Does it create curiosity?

### 5. Write `.sales/value-proposition.md`

```markdown
# Value Proposition: <Product Name>

Last updated: <date>

## One-Liner
<The winning option>

## Competitive Alternatives
<What they do today>

## Unique Capability
<Only we can...>

## Category
<We compete in...>

## Positioning Options
<All 3 options with rationale>

## Tagline Candidates
<3-5 short taglines>

## Voice & Tone Notes
<How should the founder sound? Technical? Empathetic? Direct?>
```

### 6. Founder validation

Ask:
- "Which option feels most true to your product?"
- "If a prospect read Option 2, would they say 'tell me more' or 'so what'?"
- Refine based on feedback.

## Completion criterion

`.sales/value-proposition.md` exists with at least one positioning option the founder feels confident using in outreach.
