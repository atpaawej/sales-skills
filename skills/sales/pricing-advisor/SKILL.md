---
name: pricing-advisor
description: Generate pricing options and strategy. Based on value-based pricing, anchoring, decoy effect, and Hormozi's grand slam offer framework.
disable-model-invocation: true
---

# Pricing Advisor

Helps the founder design a pricing strategy. Covers value-based pricing, tier structure, anchoring, and the psychology behind price perception.

## Prerequisites

- `.sales/context.md` exists
- `.sales/value-proposition.md` exists

## Flow

### 1. Read workspace

Read `.sales/context.md` and `.sales/value-proposition.md`.

### 2. Calculate the value

Ask the founder these questions to establish the value ceiling:

**Quantified value questions:**
- "What problem does your product solve, and what does that problem cost the customer in time/money?"
- "If your product delivers its promised outcome, how much is that worth to the customer per month?"
- "What's the cheapest alternative? (manual process, competitor, etc.)"
- "What's the most expensive alternative?"
- "Who gets the most value from your product? (this determines the ceiling)"

### 3. Build the tier structure

Based on the course's pricing psychology:

**Three tiers:**
| Tier | Position | Price | Target |
|---|---|---|---|
| Entry | Basic / Starter | Lower | Price-sensitive, small customers |
| Recommended | Most Popular | Middle (where you want them) | Most customers — the default |
| Premium | Enterprise / Pro | High (anchors the others) | Power users — makes middle look cheap |

**The Decoy Effect:**
If it makes sense, add a decoy tier that's clearly worse than Recommended at a similar price. This makes Recommended feel like the smart choice.

**Anchoring:**
Always present Premium first. The first price the prospect sees anchors their entire perception.

### 4. Check against pricing principles

From the course:

| Principle | Applied? |
|---|---|
| Value-based, not cost-plus | Price = fraction of value delivered, not cost to build |
| Anchoring | Premium price anchors the conversation |
| Decoy if needed | Middle tier looks better next to a decoy |
| Charm pricing ($.99) | For consumer; round numbers for B2B |
| Grand slam offer | Clear transformation + guarantee + bonuses |
| No discounts without reason | Annual prepay or early adopter only |
| Raise every 6 months | If nobody complains, you're too cheap |

### 5. Write `.sales/pricing.md`

```markdown
# Pricing Strategy: <Product Name>

Last updated: <date>

## Value Analysis
- Problem cost to customer: $X/month
- Value delivered: $X/month
- Recommended value capture: 10-30% → $X/month

## Tier Structure

### Premium (<Name>) — $X/mo
<What they get>
<Why this price>

### Recommended (<Name>) — $X/mo
<What they get>
<Why this price>

### Entry (<Name>) — $X/mo
<What they get>
<Why this price>

## Anchoring Strategy
<How to present pricing on the page / in conversations>

## Discount Policy
- Annual prepay: 15-20% off
- Founder pricing for first X customers: Y% off
- No other discounts

## Pricing Psychology Applied
<Specific anchoring, decoy, or charm tactics used>
```

### 6. Validate with the founder

- "Does this feel fair to you?"
- "Would you pay this if you were your customer?"
- "What's the #1 objection you expect on price?"
- Practice the response to "it's too expensive" using the pricing page as context.

## Completion criterion

`.sales/pricing.md` exists with tiered pricing, anchoring strategy, and discount policy. Founder has practiced the "too expensive" objection once.
