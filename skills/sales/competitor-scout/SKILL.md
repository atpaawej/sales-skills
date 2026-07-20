---
name: competitor-scout
description: Research the competitive landscape and find your real differentiator. Produces a positioning map and competitive scripts.
disable-model-invocation: true
---

# Competitor Scout

Most founders either ignore competitors ("we have no competition") or obsess over them ("they have 10x our funding"). Both are wrong.

The right question isn't "who are our competitors?" — it's **"what does our ICP do today to solve this problem, and how do we beat that?"**

Use `_engine` procedures for all workspace I/O.

## Prerequisites

- `.sales/context.md` exists.
- `.sales/icp.md` exists (so you know whose alternatives to evaluate).

## Flow

### 1. Read workspace and gather founder intel

Read `.sales/context.md` and `.sales/icp.md` using `_engine` procedures.

Ask:
- "Who do you see as your competitors right now?"
- "What alternatives have prospects mentioned to you?"
- "What products do you admire in this space (even if not direct competitors)?"
- "What's the closest someone could get to your product's outcome without using you?"

### 2. Research the landscape (web search required)

For each competitor the founder named, and for broader alternatives you discover:

**For each competitor/alternative:**
- What is their positioning and tagline?
- What's their pricing (public or estimated)?
- Who is their ideal customer?
- What do they do well? (from reviews, testimonials, case studies)
- Where do they fall short? (from complaints, negative reviews, G2, Reddit, HN)
- What's their origin story? (this tells you how they think)

**Beyond named competitors, search for:**
- "Alternatives to [product category]" — what comes up?
- "[Problem] solution" — what's the landscape?
- "Best [category] tools" — who's listed?

### 3. Build the positioning map

Organize findings into a clear comparative structure:

```
## The Landscape

### Direct competitors
| | Them | You |
|---|---|---|
| Positioning | | |
| Target customer | | |
| Pricing | | |
| Key strength | | |
| Key weakness | | |
| Your advantage | — | |

### Indirect alternatives
[What people do instead of buying any product — manual process, spreadsheets, workarounds]

### The gap
[What none of them do well that you do]
```

### 4. Push the founder on differentiation

After presenting your research, grill:

- "You said [competitor] is your real competition. My research shows they target a completely different customer. Are you sure, or are you looking at the wrong mirror?"
- "Every competitor claims to be faster/cheaper/better. What's the ONE thing you can say that none of them can?"
- "If a prospect said 'we use [competitor]' tomorrow, what would you say that actually changes their mind?"
- "The research shows [gap in the market]. Is that a gap you can own, or is it a gap because nobody wants it?"

### 5. Write competitive scripts

For each scenario the founder will face:

```
**When prospect says "we use [Competitor A]":**
<specific, honest response — acknowledge the competitor's strength, then differentiate>

**When prospect says "we do it manually":**
<specific response — frame the cost of manual vs your solution>

**When prospect says "we'll build it ourselves":**
<for technical founders selling to technical teams — the build-vs-buy argument>

**When prospect says "how are you different from [Competitor B]?":**
<short, punchy differentiator>
```

### 6. Write `.sales/competitors.md`

Use `_engine` write procedures:

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
<table comparing them vs you on key dimensions>

## Your Strongest Differentiator
<one-sentence summary>

## Competitive Scripts
<ready-to-use responses>
```

### 7. Deliver the verdict

"Your strongest differentiator is: [one sentence]. If a prospect mentions [top competitor], lead with [specific script]. If they say 'we'll build it ourselves,' say [specific response]."

## Completion criterion

`.sales/competitors.md` exists with at least 3 competitors/alternatives analyzed. Research is cited. The founder has a one-sentence differentiator they can say without thinking.
