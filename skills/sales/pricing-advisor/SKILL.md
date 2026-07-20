---
name: pricing-advisor
description: Design value-based pricing with anchoring, decoys, and psychology. Produces tiered pricing and a script for the 'too expensive' objection.
disable-model-invocation: true
---

# Pricing Advisor

Technical founders underprice. They calculate costs, add a margin, and set a number. That's cost-plus pricing — and it ignores the most important variable: **what is the problem worth to the customer?**

This skill helps you find that number, structure tiers that make the middle one feel obvious, and handle "it's too expensive" before it comes.

---

## Prerequisites

`.sales/context.md`, `.sales/value-proposition.md`, and `.sales/competitors.md` must exist.

---

## Flow

### 1. Read workspace

Read `.sales/context.md`, `.sales/value-proposition.md`, `.sales/competitors.md`. Check if `.sales/pricing.md` exists — if so, offer to refine or start fresh.

### 2. Research pricing benchmarks (web research)

Search for competitor pricing:
- What do competitors charge? (from competitor-scout output, plus fresh search on pricing pages)
- What is the range in this category? (lowest to highest alternatives)
- What pricing models dominate? (monthly, annual, usage-based, flat)
- Visit pricing pages directly (MCP browser if available, else search + fetch)

Present your findings before extracting the founder's numbers:
> "Here's what the market looks like. [Competitor A] charges $X, [Competitor B] charges $Y. The range is $Z to $W in this category. Does that match your expectations?"

### 3. Calculate the value ceiling

This is the hard part. The agent doesn't know the customer's numbers — the founder does. Push for real answers:

- "What does this problem cost your customer per month? In time, money, missed revenue, or risk?"
- "If your product works perfectly, how much do they save or earn per month?"
- "What's the cheapest way to solve this without your product? (manual, competitor, workaround)"

If the founder gives vague answers, push harder:
- "10 hours a week at $50/hr is $2,000/month. Does that sound right?"
- "If they lose one deal a month worth $5,000 because of this problem, that's $60k/year."

**The formula:**

```
Customer's cost of problem: $X/month
Your solution's impact: Y% of problem eliminated
Value delivered: $X × Y% = $Z/month
Your capture (10-30%): $Z × 20% = recommended price
```

Present the calculation and say: "Based on this, your price should be in the range of [$low] to [$high]."

If the founder flinches at the high end, push back:
> "If you're not scared to say the price, it's too low. Your job isn't to be cheap — it's to deliver value worth more than you charge."

### 4. Design the tier structure

Build three tiers:

**Premium** (anchor — shown first):
- Price: near the value ceiling
- Includes everything
- Makes the middle tier feel reasonable

**Recommended** (where you want them):
- Price: 40-60% of premium
- Best value for most customers
- Mark as "Most Popular"

**Entry** (for price-sensitive):
- Price: 20-30% of premium
- Limited features or usage
- Gets them in the door

**Optional decoy** — a tier between Entry and Recommended that's clearly worse than Recommended at a similar price.

### 5. Score against pricing psychology

| Principle | Applied? |
|---|---|
| Value-based (not cost-plus) | |
| Anchoring — premium shown first | |
| Decoy effect (if used) | |
| Charm pricing ($.99) — B2B uses round numbers | |
| Discount discipline — annual prepay, no other discounts | |

### 6. Write the "too expensive" script

```
When prospect says "it's too expensive":
1. Don't defend. Don't discount.
2. "I hear you. Is it the price itself, or is the value not clear yet?"
3. If "value not clear": walk through the ROI calculation again.
4. If "price too high": "What would make the full price worth it to you?"
```

### 7. Write `.sales/pricing.md`

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
<what they get, psychological rationale>

### Recommended ($X/mo) — <Name>
<what they get, psychological rationale>

### Entry ($X/mo) — <Name>
<what they get, psychological rationale>

## Psychology Applied
<specific tactics used>

## "Too Expensive" Script
<full response script>

## Discount Policy
- Annual prepay: 15-20% off
- No other discounts — ever
```

### 8. Close

> "Your pricing is: **[Entry $X | Recommended $X | Premium $X]**.
>
> Say '$[recommended price]' out loud. Does it feel too low? Too high? If you're not nervous, it's probably too low.
>
> Run `/outreach` next to start reaching out, or `/landing-page-drafter` to update your pricing page."

---

## Completion criterion

`.sales/pricing.md` exists with tiered pricing, value analysis, anchoring strategy, and a "too expensive" script. The founder has said the price out loud and confirmed they can defend it.
