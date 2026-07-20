---
name: init-sales-workspace
description: Initialize a sales workspace for a product — creates the .sales/ directory with scaffolded files. Run this first, once per product.
disable-model-invocation: true
---

# Initialize Sales Workspace

Creates a `.sales/` workspace in the current directory — the persistent data layer that every sales skill reads from and writes to. Run this once per product, at the root of the founder's working folder.

## Flow

### 1. Interview the founder

Ask every question below. Capture the answers in a structured document you'll write to `.sales/context.md`.

**About the product:**
- What is the product called? (name)
- What does it do? (one sentence)
- Who did you build it for? (initial guess — raw, unrefined)
- What problem does it solve? (the pain, not the feature)
- How is it different from alternatives? (your gut feeling)
- What format is it? (SaaS, API, digital product, physical, service, etc.)
- Monthly price you're thinking? (rough range)

**About the founder:**
- What's your background? (developer, designer, domain expert?)
- Why did you build this? (personal need, saw a gap, etc.)
- What channels are you comfortable with? (cold email, LinkedIn DMs, Twitter/X, content, community, in-person)
- How many hours per week can you spend on sales/marketing?

**About the market (current state):**
- Do you have any customers yet? (free trials, beta users, paying?)
- Have you tried selling before? (what happened?)
- Who do you *think* would pay for this?

### 2. Create the workspace

Create the following file structure:

```
.sales/
├── context.md              # The interview answers, always kept current
├── icp.md                  # Ideal Customer Profile (created by /icp-definer)
├── value-proposition.md    # Positioning & messaging (created by /value-prop-crafter)
├── competitors.md          # Competitive landscape (created by /competitor-scout)
├── pricing.md              # Pricing tiers & strategy (created by /pricing-advisor)
├── outreach/
│   ├── sequence-01.md      # Active outreach sequence
│   ├── results.md          # Track replies, conversions
│   └── templates/          # Generated email/DM templates
├── pipeline.md             # Deal pipeline / prospect tracker
├── content-calendar.md     # Content plan (created by /content-planner)
├── calls/                  # Call preps and notes
└── workspace-status.md     # Auto-generated status summary
```

Each file gets a header with `# Title` and `Last updated: <date>`.

### 3. Write `context.md`

Write the full interview into `.sales/context.md` in a clean format. Include a section at the top:

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

### 4. Summary

Print a summary:

```
✅ Sales workspace initialized at .sales/

Next steps:
  1. Run /icp-definer  — define your Ideal Customer Profile
  2. Run /value-prop-crafter — craft your value proposition
  3. Run /cold-email-writer — draft your first outreach
```

## Completion criterion

The `.sales/` directory exists with at least a populated `context.md`. The founder has seen their summary and knows what to run next.
