---
name: value-prop-crafter
description: Find the one thing only you can do, position it where it wins, and produce messaging you can use everywhere — cold email, landing page, sales call.
disable-model-invocation: true
---

# Value Proposition Crafter

Founders describe their product as "a CRM for dentists" or "an analytics platform for SaaS." Those aren't wrong — they're useless. They tell the prospect what the product does, not why they should care.

This skill finds the positioning that makes your strengths look like strengths, and gives you words you can use today.

Based on April Dunford's positioning framework (Obviously Awesome).

---

## Prerequisites

`.sales/context.md` and `.sales/icp.md` must exist.

---

## Flow

### 1. Read workspace

Read `.sales/context.md` and `.sales/icp.md`. Check if `.sales/value-proposition.md` already exists — if so, offer to refine or start fresh.

Check for `.sales/competitors.md` and `.sales/voice-examples.md` — use them for research direction and tone.

### 2. Research the competitive landscape (web research)

Do not ask the founder anything yet. Research:

- What categories does this product fit into? Search each one. Who wins in each?
- Who talks about solving this problem? What language do they use?
- What positioning do competitors use? Their tagline? Their "why us?"
- Find at least one competitor or adjacent player for each potential category
- Visit competitor landing pages (MCP browser if available, else fetch). What does their hero say? What do they lead with?
- Search for "[problem] solution", "best [category]", "alternatives to [product]"

### 3. Present the landscape

> "I researched the market positioning landscape. Here are the categories this product could play in and who owns each:
>
> 1. **[Category A]** — owned by [leader]. They position as [their positioning].
> 2. **[Category B]** — owned by [leader]. They position as [their positioning].
> 3. **[Category C]** — no clear leader yet. This is interesting.
>
> Does one of these feel like the right neighborhood? If not, what category would you add?"

### 4. Extract the unique capability (grilling)

This is the core of the skill. The agent can't *know* what's unique — it must be extracted from the founder through questioning. Push for specificity:

- "What does your ICP do TODAY to solve this problem?" — Score each: Nothing / Manual process / Competitor / Hated workaround
- "What can your product do that no alternative can?" — Reject "faster" and "cheaper." Push for the defensible thing. "We're the only one that works offline" ✓ — "We're the fastest" ✗
- "You said 'better DX' — what specifically? The API design? The docs? The onboarding?"
- "If you had to pick the one competitor that keeps you up at night, who is it?"
- "What do customers say when they try to explain what you do to a colleague?"
- "What's the one thing your product does that, if I heard it, I'd immediately say 'oh, that's different'?"

If the founder struggles, push harder. A vague product description means the founder hasn't articulated their differentiator yet. Your job is to help them find it.

### 5. Choose the category

Ask: "What category makes your strengths look like strengths?"

Examples:
- If your strength is automation, don't compete in "project management" — compete in "workflow automation"
- If your strength is simplicity, don't compete in "BI tools" — compete in "analytics for non-analysts"
- The category determines who your competitor is. Pick wisely.

If the founder picks a category that contradicts your research, push back: "You said [category], but my research shows [leader owns it]. Are you sure you want to compete there, or is there a subcategory where you win?"

### 6. Generate 3 positioning options

Write 3 distinct options:

```markdown
## Option 1: [Category-focused]

**One-liner:** "We help [ICP] [solve problem] by [unique mechanism], unlike [alternatives]."

**Why it works:** [psychological hook — emotion, curiosity, social proof]

**Where to use:** [cold email, landing page hero, pitch]

## Option 2: [Outcome-focused]

**One-liner:** "Get [specific outcome] in [timeframe] without [pain of alternative]."

**Why it works:** [psychological hook]

**Where to use:** [cold email, landing page hero, pitch]

## Option 3: [Contrarian / underdog]

**One-liner:** "Most [alternatives] do X. We do Y. Here's why Y matters for [ICP]."

**Why it works:** [psychological hook]

**Where to use:** [cold email, landing page hero, pitch]
```

Score each:

| Criterion | Option 1 | Option 2 | Option 3 |
|---|---|---|---|
| Triggers emotion, not just logic? | | | |
| Creates curiosity? | | | |
| Differentiates from alternatives? | | | |
| Can the founder say it naturally? | | | |

### 7. Present + validate

> "Here are 3 positioning options. Option [X] is my recommendation because [reason].
>
> Which one feels closest to the truth? Which one would your ICP read and say 'tell me more'?"

If the founder hesitates, refine. If the founder picks one that scores poorly, push back: "Option [X] scored lowest on differentiation. I'd recommend [Y] instead — here's why."

If the founder can't decide, recommend one: "Let's test Option [Y]. It's the most differentiated, and we can always adjust based on real replies."

### 8. Write `.sales/value-proposition.md`

```markdown
# Value Proposition: <Product Name>

Last updated: <date>

## The Winner
[the one-liner the founder chose or you recommended]

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
[How should the founder sound? Technical? Empathetic? Direct? If voice-examples.md exists, reference it.]

## Research Sources
<sites and searches consulted>
```

### 9. Close

> "Your positioning is: **[one-liner]**. Test this in your next cold email and on your landing page. If prospects say 'tell me more,' it's working. If they say 'so what,' come back and we'll refine.
>
> Run `/cold-email-writer` next to draft emails that use this positioning."

---

## Completion criterion

`.sales/value-proposition.md` exists with a winning positioning option the founder feels confident enough to test in real outreach. The founder has said the one-liner out loud and it felt true, not clever.
