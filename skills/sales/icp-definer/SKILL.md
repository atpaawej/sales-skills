---
name: icp-definer
description: Define your Ideal Customer Profile through market research and investigative questioning. Produces a narrow, actionable ICP you can use for outreach today.
disable-model-invocation: true
---

# ICP Definer

Your product solves a problem. The question is: **who feels that problem so acutely that they'd pay for a solution right now?**

This skill finds that answer. It does not ask you "who is your customer?" and fill a template. It researches, cross-examines, and narrows until you have a segment specific enough to name actual companies and people.

The file writing is a side effect. The real work is the investigation.

## Prerequisites

- `.sales/context.md` must exist (run `/init-sales-workspace` first). Use the `_engine` procedures for all workspace I/O.

## Flow

### 1. Immerse in the product

Read `.sales/context.md`. Then ask the founder exactly three questions — not to fill a form, but to calibrate your research:

1. "If your product stopped working tomorrow, which customer would notice first and complain loudest?"
2. "What did you personally observe or experience that made you build this?"
3. "Who have you already shown this to, and what did they say?"

Do not proceed until you have real answers. Push past "I haven't shown anyone yet" — ask "if you had to show one person today, who would it be?"

### 2. Research the market (web search required)

Use web search to research the space. You are looking for:

**A. Who is talking about this problem?**
- Search for the problem itself (not your product). Who's complaining about it? On Reddit, Hacker News, Twitter, blogs?
- What language do they use? Their exact words — not industry jargon, but the raw way real people describe the pain.
- Who is *already* solving adjacent problems? Not competitors — adjacent players. They validate the market exists.

**B. What segments exist in this market?**
- Find 3-5 distinct segments that experience this problem.
- For each segment, estimate: how many companies/people? How much does the problem cost them? How aware are they of the problem?

**C. Who would pay the most?**
- Not who needs it most — who would pay the most, fastest, and stay longest.
- This is usually not the same segment as "who needs it most." A startup needs it. An enterprise will pay.

### 3. Present your findings and grill the founder

Present your research like an investigator presenting to a detective:

```
I researched the market for [product category]. Here's what I found:

The problem [problem description] is real. People are talking about it in [specific places].
Here are the segments I identified:

1. [Segment A] — [description, size, pain level, willingness to pay]
   Evidence: [specific search result, quote, data point]

2. [Segment B] — [description, size, pain level, willingness to pay]
   Evidence: [specific search result, quote, data point]

3. [Segment C] — [description, size, pain level, willingness to pay]
   Evidence: [specific search result, quote, data point]
```

Then grill:

- "Segment A looks promising because [reason]. But you told me [founder's context]. Does that align or conflict?"
- "You said your ICP is [founder's guess]. My research suggests [different segment]. Help me understand the gap."
- "If you had to pick ONE of these segments and ignore the rest for 30 days, which one makes you feel most confident you can get a 'yes'?"
- "Name 5 companies in this segment. If you can't, it's still too broad."

Your tone: curious but relentless. If the founder says "I don't know," don't accept it — rephrase, dig deeper, push. The goal is specificity.

### 4. The narrowing loop

For each round of narrowing:
1. Propose a refined segment with evidence
2. Ask: "Does this feel right? Too narrow? Too broad?"
3. If too broad: push harder. "Segment of one" is the ultimate target — one specific person at one specific company.
4. If too narrow: expand slightly and test again.
5. End when: the founder can name 3-5 real companies/people AND feels confident reaching out this week.

Document the narrowing decisions:
```
Round 1: Started with [broad segment]
Round 2: Narrowed to [narrower] because [reason]
Round 3: Refined to [final] because [reason]
```

### 5. Research the final segment in depth

Once the segment is locked, research it specifically:

- Where do these people hang out online? (specific subreddits, Slack communities, newsletters, conferences)
- What keywords do they search for when the problem becomes acute?
- What solutions do they currently use or try?
- Who are the influencers/thought leaders they follow?
- What would make them say "tell me more" in an outreach message?

### 6. Write `.sales/icp.md`

Write the final ICP using `_engine` write procedures:

```markdown
# Ideal Customer Profile: <Final Segment>

Last updated: <date>

## The Segment
- **Who:** [specific role, title, persona — e.g. "Head of Engineering at B2B SaaS companies, 20-50 employees"]
- **The trigger:** [what makes the problem acute enough to act — e.g. "when they miss a compliance deadline and lose a customer"]
- **The alternative:** [what they do today instead of buying — e.g. "manual spreadsheet tracking, one engineer spends 10 hours/week"]

## Why This Segment
- **Problem in their words:** [direct quotes from research]
- **Quantified value:** [what the solution is worth to them in time/money]
- **Why they'd pay:** [urgency, budget availability, ROI clarity]

## Market Evidence
- **Sources consulted:** [search queries, sites, communities researched]
- **Validation signals:** [posts, complaints, questions that confirm the pain exists]

## Where To Find Them
- **Communities:** [specific — not "LinkedIn" but "r/devops, Hacker News threads about compliance, the Rands Leadership Slack"]
- **Keywords they search:** [the exact search terms they use when the problem hurts]
- **Influencers they follow:** [specific people, newsletters, podcasts]

## Outreach Angle
- **The hook:** [one sentence that would stop them from scrolling]
- **Their admission:** [what they'd say if they were honest about the pain]

## Narrowing History
<record of rounds: started broad, narrowed by X, refined by Y>

## Next Steps
- [3-5 specific companies/people to reach out to this week]
```

### 7. Deliver the verdict

After writing, summarize:

```
Your ICP is: [one-sentence summary]

This means:
- You should reach out to [company/people list]
- You should avoid [tempting but wrong segments]
- Your outreach hook should be: [specific hook]

3 companies you can contact TODAY:
1. [Company] — [why they fit, who to contact]
2. [Company] — [why they fit, who to contact]
3. [Company] — [why they fit, who to contact]
```

### 8. Final push

"Do you commit to reaching out to at least 3 people in this segment this week? If not, we need to refine until you feel that confidence. If yes, run `/cold-email-writer` next."

## Completion criterion

`.sales/icp.md` exists with a segment specific enough that the founder can name 3-5 real companies/people. Web research was done — the findings are cited and traceable. The founder has confirmed confidence in the segment.
