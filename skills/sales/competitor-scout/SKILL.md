---
name: competitor-scout
description: Research the competitive landscape and find your real differentiator. Produces a positioning map and scripts for every prospect objection.
disable-model-invocation: true
---

# Competitor Scout

Most founders either ignore competitors ("we have no competition") or obsess over them ("they have 10x our funding"). Both are wrong.

The right question: **what does our ICP do today to solve this problem, and how do we beat that?**

---

## Prerequisites

`.sales/context.md` and `.sales/icp.md` must exist.

---

## Flow

### 1. Read workspace

Read `.sales/context.md` and `.sales/icp.md`. Check if `.sales/competitors.md` already exists — if so, offer to update or start fresh.

### 2. Gather founder intel

Ask:
- "Who do you see as your competitors right now?"
- "What alternatives have prospects mentioned to you?"
- "What products do you admire in this space (even if not direct competitors)?"
- "What's the closest someone could get to your product's outcome without using you?"

**Before asking, check the workspace** — if `.sales/competitors.md` already has a "Direct Competitors" section, use that instead of re-asking.

### 3. Research the landscape (web research)

For each competitor the founder named, and for broader alternatives you discover:

**For each competitor/alternative:**
- What is their positioning and tagline?
- What's their pricing (public or estimated)?
- Who is their ideal customer?
- What do they do well? (from reviews, testimonials, case studies)
- Where do they fall short? (from complaints, negative reviews, G2, Reddit, HN)
- Visit their website and pricing page (MCP browser if available, else search + fetch)

**Beyond named competitors, search:**
- "Alternatives to [product category]" — what comes up?
- "[Problem] solution" — what's the landscape?
- "Best [category] tools" — who's listed?
- Search for complaints about the alternatives — what do users wish was better?

### 4. Build the positioning map

```markdown
## The Landscape

### Direct Competitors

| | Them | You |
|---|---|---|
| Positioning | | |
| Target customer | | |
| Pricing | | |
| Key strength | | |
| Key weakness | | |
| Your advantage | — | |

### Indirect Alternatives
[What people do instead of buying any product — manual process, spreadsheets, workarounds]

### The Gap
[What none of them do well that you do]
```

### 5. Present + push back

> "I mapped the landscape. **[Competitor]** is closest to you, but their target customer is different — [explain]. The gap I see is [gap]."

Then grill:
- "You said [competitor] is your real competition. My research shows they target a completely different customer. Are you sure, or are you looking at the wrong mirror?"
- "Every competitor claims to be faster/cheaper/better. What's the ONE thing you can say that none of them can?"
- "If a prospect said 'we use [competitor]' tomorrow, what would you say?"
- "The research shows [gap]. Is that a gap you can own, or is it a gap because nobody wants it?"

If the founder can't articulate a differentiator, push harder — reference the unique capability from value-prop-crafter if it exists.

### 6. Write competitive scripts

For each real scenario:

```
**When prospect says "we use [Competitor A]":**
<specific response — acknowledge the competitor's strength, then differentiate>

**When prospect says "we do it manually":**
<response — frame the cost of manual vs your solution>

**When prospect says "we'll build it ourselves":**
<build-vs-buy argument — for technical founders selling to technical teams>

**When prospect says "how are you different from [Competitor B]?":**
<short, punchy differentiator>
```

### 7. Write `.sales/competitors.md`

```markdown
# Competitive Landscape

Last updated: <date>

## Research Sources
<searches, sites consulted>

## Direct Competitors
<detailed analysis for each>

## Indirect Alternatives
<what people do instead>

## Positioning Map
<table comparing them vs you>

## Your Strongest Differentiator
<one-sentence summary>

## Competitive Scripts
<ready-to-use responses>
```

### 8. Close

> "Your strongest differentiator is: **[one sentence]**. Memorize that. When a prospect mentions [top competitor], say [specific script]. When they say 'we'll build it ourselves,' say [specific script].
>
> Run `/pricing-advisor` next if you haven't yet, or `/outreach` to start reaching out."

---

## Completion criterion

`.sales/competitors.md` exists with at least 3 competitors/alternatives analyzed, research cited, and competitive scripts the founder can use in real conversations.
