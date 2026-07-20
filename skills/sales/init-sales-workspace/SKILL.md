---
name: init-sales-workspace
description: Create a .sales/ workspace with scaffolded files. Run once per product, at the root of your product folder.
disable-model-invocation: true
---

# Initialize Sales Workspace

Creates `.sales/` in the current directory — the persistent store every sales skill reads from and writes to. Run this once per product.

---

## Flow

### 1. Check if `.sales/` already exists

If `.sales/context.md` exists, tell the founder:
> "Your workspace is already initialized. Run `/sales-navigator` to see your status."

If `.sales/` exists but `context.md` doesn't, ask the founder to resolve or delete `.sales/` so you can start fresh.

If neither exists, proceed.

### 2. Collect what you need

Work through every question below. **Before asking any question, check the workspace for an existing answer** — if `context.md` already has it, skip the question. Only ask what's missing.

**About the product:**
- What is the product called?
- What does it do? One sentence.
- Who did you build it for? Initial guess, raw and unrefined.
- What problem does it solve? The pain, not the feature.
- How is it different from alternatives? The founder's gut feeling.
- What format is it? (SaaS, API, digital product, physical, service, etc.)
- Rough monthly price range?

**About the founder:**
- What's your background? (developer, designer, domain expert?)
- Why did you build this? (personal need, saw a gap, etc.)
- What channels are you comfortable with? (cold email, LinkedIn DMs, Twitter/X, content, community, in-person)
- How many hours per week can you spend on sales/marketing?

**About the market (current state):**
- Do you have any customers yet? (free trials, beta users, paying?)
- Have you tried selling before? What happened?
- Who do you *think* would pay for this?

Ask one question at a time. Wait for the answer before moving to the next.

### 3. Create the workspace

Create this directory structure:

```
.sales/
├── context.md
├── icp.md
├── value-proposition.md
├── competitors.md
├── pricing.md
├── outreach/
│   ├── sequence-01.md
│   ├── results.md
│   └── templates/
├── pipeline.md
├── content-calendar.md
├── calls/
├── workspace-status.md
└── voice-examples.md
```

### 4. Write `context.md`

Write the full interview into `.sales/context.md`. Use this format:

```markdown
# Sales Context: <Product Name>

Last updated: <date>

## Product
- Name:
- One-liner:
- Format:
- Rough price:

## Founder
- Background:
- Comfort channels:
- Weekly hours available:

## Current State
- Existing customers?:
- Previous sales attempts?:
- Initial ICP guess:

## Raw Interview
<full Q&A from the interview>
```

### 5. Summary

```
✅ Sales workspace initialized at .sales/

Next steps:
  1. Run /icp-definer — find your Ideal Customer Profile
  2. Run /value-prop-crafter — craft your value proposition
  3. Run /cold-email-writer — draft your first outreach
```

---

## Completion criterion

`.sales/context.md` exists with populated product, founder, and market state. The founder knows what to run next.
