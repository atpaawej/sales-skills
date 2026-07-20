---
name: landing-page-drafter
description: Draft landing page copy based on value proposition and ICP. Covers hero, problem, solution, social proof, and CTA.
disable-model-invocation: true
---

# Landing Page Drafter

Drafts copy for the founder's landing page or website. Not design — just the words that sell.

## Prerequisites

- `.sales/value-proposition.md` exists
- `.sales/icp.md` exists

## Flow

### 1. Read workspace

Read `.sales/value-proposition.md`, `.sales/icp.md`, `.sales/competitors.md` (if exists).

Ask the founder:
- "What page specifically needs copy? (homepage, product page, pricing page, landing page for a specific campaign?)"
- "Do you have an existing page you want me to rewrite?"
- "What's the primary action you want visitors to take?"

### 2. Apply the psychological structure

Every landing page should lead with emotion, back with logic. Use this structure:

**1. Hero section**
- Headline: The single most important line. Solve the emotional problem.
  - Bad: "Cloud-based project management software"
  - Good: "Stop losing track of your projects"
- Subheadline: Clarify who it's for and what happens next.
- CTA button: Specific action ("Start your free trial" vs "Submit")

**2. Problem section**
- Name the pain the ICP feels
- Show you understand their world
- Trigger the emotional hook: "If this is you, keep reading"

**3. Solution section**
- How the product solves the problem
- Features as *evidence*, not the sell
- Screenshots/demo — show, don't tell

**4. Social proof**
- Testimonials (specific results, not "it's great")
- Logos (if any)
- Usage stats (X customers, Y problems solved)
- "Join [number] founders who've switched"

**5. Objection handling**
- FAQ that pre-emptively answers objections
- "Is this for me?" — define exactly who should (and shouldn't) buy

**6. CTA**
- One clear action
- Reduce friction: "No credit card required" / "5 minute setup"
- Scarcity/urgency if genuine

### 3. Write the copy

Write full copy for each section. Use the voice defined in `.sales/value-proposition.md`.

```markdown
# Landing Page Copy: <Page>

## Hero
- **Headline:** <emotional hook>
- **Subheadline:** <clarify>
- **CTA:** <action>

## Problem
<2-3 paragraphs naming the pain>

## Solution
<2-3 paragraphs showing how it works>

## Social Proof
<testimonial 1>
<testimonial 2>
<stat>

## Objections (FAQ)
- Q: <common objection> → A: <response>

## CTA
<Final call to action>
```

### 4. Show the founder

- Highlight the emotional hooks
- Explain why each section uses that approach
- Ask: "Does your ICP feel seen when they read this?"
- Iterate on the headline specifically — it's the most important line

## Completion criterion

Draft copy exists for at least 3 sections (hero, problem, solution, CTA). Founder has approved the headline.
