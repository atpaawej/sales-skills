---
name: content-planner
description: Plan a 30-day content calendar with drafted posts. Uses the ICP's world and your value proposition to create content that attracts the right people.
disable-model-invocation: true
---

# Content Planner

Content marketing works — but only if you're consistent. This skill builds a 30-day plan you can actually stick to, matched to your available hours and your authentic voice.

The output is not a vague editorial calendar. It's actual drafted posts for the first week.

Use `_engine` procedures for all workspace I/O.

## Prerequisites

- `.sales/context.md`, `.sales/icp.md`, `.sales/value-proposition.md` exist.

## Flow

### 1. Read workspace and research

Read `.sales/context.md`, `.sales/icp.md`, `.sales/value-proposition.md` using `_engine` procedures.

Then research:
- What content is working in your ICP's space? (search for popular posts, threads, articles)
- What questions are your ICP asking? (Reddit, Quora, Hacker News, Twitter)
- What do competitors post about? What gets engagement?

### 2. Find founder's authentic voice

Ask:
- "What channels do you want to post on?"
- "How many hours per week can you COMMIT — not hope for?"
- "What topics could you talk about for 30 minutes without preparing?"
- "Do you prefer writing long-form (essays, threads) or short-form (tweets, posts)?"
- "What's a hot take you have about your industry that might be unpopular?"
- "Who's a creator you admire in any space? What do you like about their style?"

### 3. Define 3-4 content pillars

These are topics you can talk about repeatedly without running dry:

| Pillar | Description | Example angle |
|---|---|---|
| 1. The problem | Why it matters, war stories, cost of ignoring it | "Why your team's manual process is costing you $10k/month" |
| 2. The solution philosophy | How you think about solving it (not product pitches) | "The right way to think about [problem]" |
| 3. Founder journey | Building in public, lessons, vulnerability | "I spent 6 months building a feature nobody used" |
| 4. Industry insights | Trends, news, your takes | "Why [trend] matters for [ICP]" |

### 4. Build the calendar based on real hours

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

### 5. Draft the first week's posts

Write the full content for the first 3 posts:

```
## Post 1
**Platform:** [Twitter/LinkedIn/blog]
**Topic:** [topic]
**Hook:** [first line — most important]
**Body:** [full post]
**CTA:** [if any]

## Post 2
...

## Post 3
...
```

Each post must:
- Start with a hook that stops the scroll
- Speak to the ICP's specific situation
- Lead with an opinion, a story, or a data point — never a generic observation
- End with either a CTA or a thought-provoking question

### 6. Write `.sales/content-calendar.md`

Use `_engine` write procedures:

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

### Week 2
...

### Week 3
...

### Week 4
...

## First Week Drafts
<full text of post 1>
<full text of post 2>
<full text of post 3>

## Content Bank
<extra ideas for when inspiration runs dry>
```

### 7. Validate

- "Is the volume realistic for your life right now?"
- "If you could only post one thing this week, which would be most valuable to your ICP?"
- "Does this feel like content YOU would write, or content you're forcing?"

If the volume feels too high, cut it in half. Consistency beats intensity.

## Completion criterion

`.sales/content-calendar.md` exists with a 30-day plan. First 3 posts are fully drafted. Founder has committed to posting at least once this week.
