---
name: pricing-advisor
description: Design a pricing strategy using value-based principles, psychology, and market research. Produces tiered pricing with anchoring and positioning.
disable-model-invocation: true
---

# Pricing Advisor

Technical founders underprice. They calculate their costs, add a margin, and set a number. That's cost-plus pricing — and it ignores the most important variable: **what is the problem worth to the customer?**

This skill doesn't just help you pick a number. It helps you understand the value you deliver, structure tiers that make the middle one feel obvious, and handle the "it's too expensive" objection before it comes.

Use `_engine` procedures for all workspace I/O.

## Prerequisites

- `.sales/context.md`, `.sales/value-proposition.md`, and `.sales/competitors.md` exist.

## Flow

### 1. Read workspace and research pricing benchmarks

Read `.sales/context.md`, `.sales/value-proposition.md`, `.sales/competitors.md` using `_engine` procedures.

Then research:

- What do competitors charge? (from competitor-scout output, plus fresh search)
- What is the range in this category? (lowest to highest alternatives)
- What pricing models dominate in this space? (monthly, annual, usage-based, flat)

### 2. Calculate the value ceiling

Ask the founder — push for real numbers:

- "What does this problem cost your customer? In time, money, missed revenue, or risk?"
- "If your product works perfectly, how much does the customer save or earn per month?"
- "What's the cheapest way to solve this without your product? (manual, competitor, workaround)"
- "If your price was 10x higher, which customers would still buy? (that's your real value ceiling)"

The formula:

```
Customer's cost of problem: $X/month
Your solution's impact: Y% of problem eliminated
Value delivered: $X * Y% = $Z/month
Your capture (10-30%): $Z * 20% = recommended price
```

### 3. Design the tier structure

Based on the value ceiling and competitive research, build three tiers:

**Premium** (anchor — shown first):
- Price: near the value ceiling
- Includes everything
- Makes the middle tier feel reasonable

**Recommended** (where you want them):
- Price: 40-60% of premium
- The best value for most customers
- Mark as "Most Popular" or "Recommended"

**Entry** (for price-sensitive):
- Price: 20-30% of premium
- Limited features or usage
- Gets them in the door

**Optional: Decoy tier**
If it helps, add a tier between Entry and Recommended that's clearly worse than Recommended at a similar price. This makes Recommended feel like a steal.

### 4. Score against pricing psychology

For each tier:

| Principle | Applied? |
|---|---|
| Value-based (not cost-plus) | Price is fraction of value, not cost to build |
| Anchoring | Premium shown first, sets the frame |
| Decoy effect | Middle tier looks best next to the decoy (if used) |
| Charm pricing ($.99) | For consumer; round numbers for B2B |
| Grand slam offer | Clear transformation + guarantee + bonuses |
| Discount discipline | Annual prepay 15-20% off, early adopter pricing, no other discounts |

### 5. Practice the "too expensive" response

Write a specific script for the founder:

```
When prospect says "it's too expensive":
1. Don't defend the price. Don't discount.
2. Say: "I hear you. Is it the price itself, or is the value not clear enough yet?"
3. If they say "the value isn't clear": walk through the ROI calculation again.
4. If they say "the price is too high": "What would make the full price worth it to you?"
```

### 6. Write `.sales/pricing.md`

Use `_engine` write procedures:

```markdown
# Pricing Strategy: <Product Name>

Last updated: <date>

## Value Analysis
- Problem cost to customer: $X/month
- Value delivered: $X/month
- Recommended capture rate: X%
- Recommended price: $X/month

## Tier Structure
### Premium ($X/mo) — <Name>
<what they get>
<psychological rationale>

### Recommended ($X/mo) — <Name>
<what they get>
<psychological rationale>

### Entry ($X/mo) — <Name>
<what they get>
<psychological rationale>

## Psychology Applied
<anchoring, decoy, charm — specific tactics>

## "Too Expensive" Script
<full response script>

## Discount Policy
- Annual prepay: 15-20% off
- Founder pricing (first X customers): Y% off
- No other discounts — ever
```

### 7. Final check

- "If your ICP doesn't flinch at this price, it's too low."
- "If you're scared to say this number, it's probably right."
- "Would you pay this if you were your customer? If no, fix the value, not the price."

## Completion criterion

`.sales/pricing.md` exists with tiered pricing, value analysis, anchoring strategy, discount policy, and a "too expensive" script. Founder has said the price out loud and confirmed they can defend it.
