---
name: competitor-scout
description: Research and map the competitive landscape. Uses web research to find alternatives and position against them.
disable-model-invocation: true
---

# Competitor Scout

Researches the competitive landscape so the founder knows who they're up against, what the alternatives are, and how to differentiate.

## Prerequisites

- `.sales/context.md` exists

## Flow

### 1. Read context and ask

Read `.sales/context.md`. Ask the founder:
- "Who do you see as your competitors?"
- "What alternatives do prospects mention?"
- "What products do you *admire* in this space (even if not direct competitors)?"

### 2. Research (use web search)

Research the named competitors and discover ones the founder didn't mention. For each competitor, find:
- What they offer (features, positioning)
- Their pricing (public or estimated)
- Their target customer
- Their key messaging/thesis
- Their strengths (from reviews)
- Their weaknesses (from reviews, complaints)

### 3. Write `.sales/competitors.md`

```markdown
# Competitive Landscape: <Category>

Last updated: <date>

## Direct Competitors

### <Competitor 1>
- **Positioning:**
- **Target customer:**
- **Pricing:**
- **Strengths:**
- **Weaknesses:**
- **Our advantage:**

### <Competitor 2>
...

## Indirect Alternatives
<What people do instead of buying any product>

## Positioning Map

| Dimension | Them | Us |
|---|---|---|
| <Dimension 1> | | |
| <Dimension 2> | | |
| <Dimension 3> | | |

Our strongest differentiator: <one thing none of them have>

## Competitive Response Scripts

**When prospect says "we use Competitor X":**
<1-2 sentence response>

**When prospect says "we do it manually":**
<1-2 sentence response>
```

### 4. Brief the founder

Summarize:
- "Here are the 3 competitors you need to know about"
- "Your strongest differentiator is: ______"
- "If a prospect mentions [competitor], here's what to say"

## Completion criterion

`.sales/competitors.md` exists with at least 3 competitors analyzed. Founder knows their top differentiator and has a competitive response script.
