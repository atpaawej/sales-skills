---
name: landing-page-drafter
description: Draft landing page copy that sells. Uses the ICP, value proposition, and competitive research to write copy that triggers emotion and drives action.
disable-model-invocation: true
---

# Landing Page Drafter

Most landing pages list features. The best ones sell outcomes. This skill writes copy that leads with emotion, backs with logic, and gives the visitor one clear thing to do.

Not design — just the words that sell. Write them, then hand them to a designer.

Use `_engine` procedures for all workspace I/O.

## Prerequisites

- `.sales/value-proposition.md`, `.sales/icp.md`, and `.sales/competitors.md` exist.

## Flow

### 1. Read workspace and research

Read `.sales/value-proposition.md`, `.sales/icp.md`, `.sales/competitors.md` using `_engine` procedures.

Then research:
- What landing pages do competitors use? Visit them. What does their hero say?
- What language do top landing pages in this space use?
- What social proof exists in this market? (testimonials, usage stats, logos)

Ask the founder:
- "What page are we writing? (homepage, product page, pricing page, campaign landing page)"
- "What's the single action you want visitors to take?"
- "Do you have any existing copy to improve?"
- "Who do you consider your gold-standard example of a great landing page in any industry?"

### 2. Write the psychological structure

Every landing page follows this order. Write full copy for each section.

**1. Hero section** — 3 seconds to capture them
- Headline: Name the emotional problem your ICP feels
  - Bad: "Cloud-based project management software"
  - Good: "Stop losing track of your projects"
  - Better: "Your team's projects shouldn't be a black hole"
- Subheadline: Who it's for + what happens next
- CTA button: Specific, action-oriented ("Start free trial" > "Submit")
- Visual hint: What would sit next to this copy? (screenshot, demo GIF, illustration)

**2. Problem section** — make them feel seen
- Name the pain in the ICP's own language (from the research)
- Show you understand their specific situation
- Trigger: "Sound familiar?"

**3. Solution section** — features as evidence
- Lead with the outcome ("You'll never manually update a status report again")
- Features exist to prove the outcome is real
- Write 3-5 specific benefits, not feature names

**4. Social proof** — they need to know others chose this
- Specific testimonials (numbers, names, contexts)
- If no customers yet: founder story, personal guarantee, or problem authenticity
- Badge: "Used by [X] teams" or "Built by a founder who had this exact problem"

**5. Objection handling** — FAQ that closes
- "Is this for me?" — define exactly who should (and shouldn't) buy
- "How is this different from [competitor]?" — from competitive scripts
- "What if it doesn't work?" — guarantee if you have one

**6. CTA** — one thing, no distractions
- Restate the offer
- Remove friction ("No credit card required" / "5-minute setup")
- One button. Not two.

### 3. Write `.sales/landing-page-copy.md`

Use `_engine` write procedures:

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
- Q: <common doubt> → A: <specific, honest answer>

## CTA
<final ask, friction removed>

## Voice & Tone Notes
<how does this page sound? technical? warm? direct?>
```

### 4. Validate

Read the headline to the founder:

- "If your ICP read this headline, would they think 'that's not me' or 'that IS me'?"
- "If they read nothing else, does the hero section make them want to scroll?"
- "Read the problem section. Does it sound like you understand their world, or like generic copy?"

Iterate the headline until the founder says "yes, that would stop me from scrolling."

### 5. Write the.landing-page-copy.md

Write to `.sales/landing-page-copy.md` using `_engine` write procedures.

## Completion criterion

Draft copy exists for hero, problem, solution, and CTA sections. Founder has approved the headline and confirmed the copy matches their voice.
