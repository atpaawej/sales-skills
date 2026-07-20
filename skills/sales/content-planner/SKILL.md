---
name: content-planner
description: Plan a 30-day content calendar with drafted posts. Matched to your available hours and authentic voice — not a vague editorial calendar.
disable-model-invocation: true
---

# Content Planner

Content marketing works — but only if you're consistent. This skill builds a 30-day plan you can actually stick to, matched to your available hours and your authentic voice.

The output is not a vague editorial calendar. It's actual drafted posts for the first week.

---

## Prerequisites

`.sales/context.md`, `.sales/icp.md`, and `.sales/value-proposition.md` must exist.

---

## Flow

### 1. Read workspace

Read `.sales/context.md`, `.sales/icp.md`, `.sales/value-proposition.md`. Check if `.sales/content-calendar.md` exists — if so, offer to extend the existing calendar or start a new month.

Read `.sales/voice-examples.md` if it exists — match the founder's natural tone.

### 2. Research what's working

Do not ask the founder anything yet. Research:

- What content is working in the ICP's space? Search for popular posts, threads, articles
- What questions is your ICP asking? Reddit, Quora, HN, Twitter/X, LinkedIn discussions
- What do competitors post about? What gets engagement?
- What format is trending? (short posts, threads, videos, newsletters, podcasts)

### 3. Find the founder's authentic voice

Ask — and **save the answers to `.sales/voice-examples.md`** so you never ask again:

- "What channels do you want to post on?"
- "How many hours per week can you COMMIT — not hope for?"
- "What topics could you talk about for 30 minutes without preparing?"
- "Do you prefer writing long-form (essays, threads) or short-form (tweets, posts)?"
- "What's a hot take you have about your industry that might be unpopular?"
- "Who's a creator you admire? What do you like about their style?"

If `.sales/voice-examples.md` already has this data, skip the questions and use what's stored.

### 4. Define 3-4 content pillars

Topics the founder can talk about repeatedly without running dry:

| Pillar | Description | Example angle |
|---|---|---|
| 1. The problem | Why it matters, war stories, cost of ignoring it | "Why your manual process costs $10k/month" |
| 2. Solution philosophy | How you think about solving it (not product pitches) | "The right way to think about [problem]" |
| 3. Founder journey | Building in public, lessons, vulnerability | "I spent 6 months building a feature nobody used" |
| 4. Industry insights | Trends, news, your takes | "Why [trend] matters for [ICP]" |

### 5. Build the calendar based on real hours

**2 hrs/week**
```
Week 1: Post 1 (Pillar 1) + Post 2 (Pillar 2)
Week 2: Post 3 (Pillar 3) + Post 4 (Pillar 1)
Week 3: Post 5 (Pillar 4) + Post 6 (Pillar 2)
Week 4: Post 7 (Pillar 1) + Post 8 (Pillar 3)
```

**5 hrs/week**
Same as 2hr + 1 deep thread per week (Pillar 4)

**10+ hrs/week**
Daily posts + 2 threads + 1 newsletter

If the founder's commitment seems unrealistic, push back: "You said 10 hrs/week but you're building a product and have a day job. Let's start at 5 hrs/week. Consistency beats intensity."

### 6. Draft the first week's posts

Write full content for the first 3 posts:

```
## Post 1
**Platform:** [Twitter/LinkedIn/blog]
**Topic:** [topic]
**Hook:** [first line — most important]
**Body:** [full post]
**CTA:** [if any]

## Post 2
...
```

Each post must:
- Start with a hook that stops the scroll
- Speak to the ICP's specific situation
- Lead with an opinion, a story, or a data point — never a generic observation
- End with a CTA or a thought-provoking question

### 7. Write `.sales/content-calendar.md`

```markdown
# Content Calendar: <Product Name>

Last updated: <date>

## Content Pillars
1. [Pillar 1]
2. [Pillar 2]
3. [Pillar 3]

## Weekly Commitment
<X hours/week, Y posts/week>

## 30-Day Calendar
### Week 1
- Mon: [Post title] — [Pillar X] — *drafted below*
- Wed: [Post title] — [Pillar X]
- Fri: [Post title] — [Pillar X]

### Week 2-4
<planned but not drafted>

## First Week Drafts
<full text of post 1>
<full text of post 2>
<full text of post 3>

## Content Bank
<extra ideas for when inspiration runs dry>
```

### 8. Validate

- "Is the volume realistic for your life right now?"
- "If you could only post one thing this week, which would be most valuable?"
- "Does this feel like content YOU would write, or content you're forcing?"

If the volume feels too high, cut it in half. Consistency beats intensity.

### 9. Close

> "Your content plan is ready. Post the first piece **[this week]** — that's the only deadline that matters. The rest of the plan is a guide, not a contract.
>
> Run `/landing-page-drafter` to align your landing page messaging with this content, or `/outreach` to start reaching out directly."

---

## Completion criterion

`.sales/content-calendar.md` exists with a 30-day plan. First 3 posts are fully drafted. Founder has committed to posting at least once this week.
