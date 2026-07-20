---
name: icp-definer
description: Define your Ideal Customer Profile. I research the market, map segments, and recommend who to sell to — backed by evidence, narrowed to names you can reach today.
disable-model-invocation: true
---

# ICP Definer

Your product solves a problem. The question is: who feels it so acutely that they'd pay right now?

I'll research that question, present my finding, and handle your pushback. You just need to react — tell me what's right and what's wrong.

---

## Prerequisites

`.sales/context.md` must exist. Run `/init-sales-workspace` first if it doesn't.

---

## Flow

### 1. Read workspace

Read `.sales/context.md`. Check if `.sales/icp.md` already exists — if it does, start with:
> "Your workspace already has an ICP defined. I can help you refine it or start fresh. What do you want to do?"

Check if `.sales/voice-examples.md` or `.sales/competitors.md` exist — any existing data sharpens the research.

### 2. Research the market (extensive web research)

Do not ask the founder anything yet. Research:

**A. Understand the problem deeply**
- Search for the problem itself (not the product). What are people saying about it?
- Cast a wide net: Reddit, Hacker News, Twitter/X, blogs, forums, review sites (G2, Capterra), YouTube comments, LinkedIn discussions
- What language do people use? Their exact words, not industry jargon
- What's the emotional tone? Frustrated? Resigned? Actively looking?
- Capture at least 3-5 real quotes or posts from real people experiencing this problem
- If a browser tool is available (MCP), open relevant pages for deeper reading. Otherwise use web search + fetch.

**B. Map the market segments**
- Find 3-5 distinct segments of people/companies that experience this problem
- For each segment identify:
  - Who they are (role, company size, industry)
  - How acutely they feel the problem (mild, moderate, severe)
  - What they currently do instead of using a solution
  - What the problem likely costs them (time, money, stress)
- Look for patterns across segments — the same complaint appearing in different places

**C. Identify the best starting segment**
- Not who needs it most — who will pay, implement quickly, and stay
- The segment where the problem is most acute AND the buyer has budget/authority
- The segment that's easiest to reach (they hang out in accessible places)

**D. Find real companies/people in this segment**
- Search for actual companies that fit the profile
- Find 5-10 real examples (company names, LinkedIn profiles, people)
- Identify where they congregate online (specific communities, subreddits, newsletters, events)
- Note how to reach them (cold email, LinkedIn DM, Twitter/X, community engagement)

### 3. Build your hypothesis

Synthesize everything into a clear recommendation:

```markdown
## Market Research Summary

I researched [problem space] and found [key insight].

The problem is real. Here's evidence:
- [Quote/post 1 from a real person]
- [Quote/post 2 from a real person]
- [Search volume or community size indicator]

## Segments Identified

1. [Segment A] — [who they are]
   Pain level: [high/medium/low]
   Willingness to pay: [high/medium/low]  
   Ease to reach: [high/medium/low]
   Evidence: [specific sources]

2. [Segment B] — same analysis...

3. [Segment C] — same analysis...

## My Recommendation

🎯 **[Segment Name]**

Why:
- They feel the problem most acutely: [evidence]
- They have budget/authority: [evidence]
- They're reachable: [specific communities, channels]

3 real targets in this segment:
1. [Company/Person] — [why they fit, how to reach]
2. [Company/Person] — [why they fit, how to reach]
3. [Company/Person] — [why they fit, how to reach]
```

### 4. Present to the founder

Deliver your findings. Structure it as:

> "Here's what I found from researching [problem space]. Your product solves [problem], and the market confirms this is a real pain point — here's proof [quotes/data].
>
> Based on my analysis, the best starting ICP is **[segment]**. Here's why: [reasoning].
>
> Here's what I recommend you **ignore for now**: [other segments] — [why not yet].
>
> What's right about this? What's wrong?"

### 5. Handle the founder's reaction

Three scenarios:

**Founder says "that feels right"**
Proceed to write.

**Founder says "that's wrong because [valid correction]"**
Refine your recommendation. Update the segments, adjust the target, re-present. One or two rounds max — then write and move on.

**Founder says "let's target everyone" or "why so narrow?"**
Push back. Use the same psychology the sales playbook teaches:
- **Acknowledge**: "I understand why you'd want maximum reach — it feels like you're leaving money on the table by narrowing."
- **Reframe**: "The problem is that when you target everyone, you appeal to no one. A broad ICP means generic messaging, low reply rates, and wasted time."
- **Evidence**: "Here's what happens with broad outreach vs narrow ICP targeting — narrow consistently sees 5-15% reply rates while broad gets under 1%."
- **Propose**: "Let's start narrow. If it doesn't work, we widen. But starting narrow gives us a clean signal — we know exactly who said no and why."

If the founder still disagrees after the pushback, note the disagreement and proceed with their input. The workspace file records the decision: "Founder overrode recommendation — results will tell us who was right."

### 6. Write `.sales/icp.md`

```markdown
# Ideal Customer Profile

Last updated: <date>

## Research Sources
<all searches, sites, communities consulted>

## Market Evidence
<real quotes, posts, data points proving the problem exists>

## Recommended ICP
- **Who:** [specific role, title, company profile]
- **The trigger:** [what makes the problem acute enough to act]
- **The alternative:** [what they do today instead of buying]

## Why This Segment
- **Problem in their words:** [real quotes from research]
- **Quantified value:** [what solving this is worth to them]
- **Why they'd pay:** [urgency, budget, ROI clarity]

## Where To Find Them
- **Communities:** [specific — not "LinkedIn" but actual groups, subreddits, forums]
- **Keywords:** [what they search for when the problem hurts]
- **Influencers:** [who they follow, what they read]

## Real Targets (Start Here)
1. [Company/Person] — [context, how to reach]
2. [Company/Person] — [context, how to reach]
3. [Company/Person] — [context, how to reach]

## Segments Researched But Not Recommended
<record of other segments considered and why they weren't chosen>
```

### 7. Close

> "Your ICP is **[one-liner]**. You should reach out to those 3 targets this week. Run `/outreach` next to write your first emails, or `/value-prop-crafter` to sharpen how you talk about what you do."

---

## Completion criterion

`.sales/icp.md` exists with a specific, research-backed segment. The founder has seen the evidence and confirmed the ICP feels right enough to start outreach — or has overridden with their own input, which is documented.
