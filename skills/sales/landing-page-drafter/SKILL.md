---
name: landing-page-drafter
description: Draft landing page copy that sells — hero, problem, solution, social proof, FAQ, CTA. Backed by research, written for your ICP.
disable-model-invocation: true
---

# Landing Page Drafter

Most landing pages list features. The best ones sell outcomes. This skill writes copy that leads with emotion, backs with logic, and gives the visitor one clear thing to do.

Not design — just the words that sell. Write them, then hand them to a designer.

---

## Prerequisites

`.sales/value-proposition.md`, `.sales/icp.md`, and `.sales/competitors.md` must exist.

---

## Flow

### 1. Read workspace

Read `.sales/value-proposition.md`, `.sales/icp.md`, `.sales/competitors.md`. Check if `.sales/landing-page-copy.md` already exists — if so, offer to refine or start fresh.

Read `.sales/voice-examples.md` if it exists — match the founder's natural tone.

### 2. Research competitor landing pages

Do not ask the founder anything yet. Research:

- What landing pages do competitors use? Search for them, visit them
- What does their hero say? Their headline? Subheadline? CTA?
- What language do top landing pages in this space use?
- What social proof exists? (testimonials, usage stats, logos)
- Visit pages directly (MCP browser if available, else fetch)
- Collect 3-5 strong headline examples from this space

### 3. Ask the founder

- "What page are we writing? (homepage, product page, pricing page, campaign landing page)"
- "What's the single action you want visitors to take?"
- "Do you have any existing copy to improve?"
- "Who do you consider the gold standard of landing pages in any industry?"

### 4. Write the psychological structure

Every landing page follows this order. Write full copy for each section.

**1. Hero** — 3 seconds to capture them
- Headline: Name the emotional problem your ICP feels. Not "Cloud-based project management" but "Stop losing track of your projects"
- Subheadline: Who it's for + what happens next
- CTA button: Specific, action-oriented
- Visual hint: What sits next to this copy? (screenshot, demo GIF, illustration)

**2. Problem** — make them feel seen
- Name the pain in the ICP's own language (from your research)
- Show you understand their specific situation
- End with: "Sound familiar?"

**3. Solution** — features as evidence
- Lead with the outcome ("You'll never manually update a status report again")
- Features exist to prove the outcome is real
- Write 3-5 specific benefits, not feature names

**4. Social proof** — they need to know others chose this
- Specific testimonials (numbers, names, contexts)
- If no customers yet: founder story, personal guarantee, or problem authenticity
- "Used by [X] teams" or "Built by a founder who had this exact problem"

**5. Objection handling (FAQ)** — close their doubts
- "Is this for me?" — define exactly who should (and shouldn't) buy
- "How is this different from [competitor]?" — from competitive scripts
- "What if it doesn't work?" — guarantee if you have one

**6. CTA** — one thing, no distractions
- Restate the offer
- Remove friction ("No credit card required" / "5-minute setup")
- One button. Not two.

### 5. Validate

Push the founder hard on the headline:
- "If your ICP read this headline, would they think 'that IS me' or 'that's not me'?"
- "If they read nothing else, does the hero make them want to scroll?"
- "Read the problem section. Does it sound like you understand their world, or like generic copy?"

Iterate the headline until the founder says "yes, that would stop me from scrolling."

### 6. Write `.sales/landing-page-copy.md`

```markdown
# Landing Page Copy: <Page Name>

Last updated: <date>

## Research Summary
<competitor landing pages reviewed, language patterns found>

## Hero
**Headline:** <emotional hook, problem-first>
**Subheadline:** <clarifies who and what>
**CTA button:** <text>

## Problem
<2-3 paragraphs, ICP's language, emotional anchors>

## Solution
<benefits, not features — how life changes after>

## Social Proof
<testimonials, stats, founder story>

## Objections (FAQ)
- Q: <common doubt> → A: <specific, honest answer>

## CTA
<final ask, friction removed>

## Voice & Tone Notes
<how does this page sound? technical? warm? direct?>
```

### 7. Close

> "Your landing page copy is written. The headline is your most important sentence — if you change nothing else, get that right.
>
> Run `/outreach` next to draft emails that use the same messaging, or `/content-planner` to build a launch content calendar."

---

## Completion criterion

Draft copy exists for hero, problem, solution, and CTA sections. The founder has approved the headline and confirmed the copy matches their voice.
