---
name: content-planner
description: Plan a 30-day content calendar based on the product, ICP, and marketing channels. Generates post ideas and drafts.
disable-model-invocation: true
---

# Content Planner

Creates a 30-day content marketing plan tailored to the founder's bandwidth and channels. The goal: consistent, useful content that attracts the ICP without burning out the founder.

## Prerequisites

- `.sales/context.md` exists
- `.sales/icp.md` exists
- `.sales/value-proposition.md` exists

## Flow

### 1. Read workspace and assess

Read `.sales/context.md`, `.sales/icp.md`, `.sales/value-proposition.md`.

Ask the founder:
- "What channels do you want to post on? (Twitter/X, LinkedIn, blog, newsletter, YouTube, etc.)"
- "How many hours per week can you commit to content?"
- "What topics can you talk about authentically?"
- "Do you enjoy writing long-form (essays, threads) or short-form (tweets, posts)?"
- "Do you have any content already published?"

### 2. Build content pillars

Define 3-4 content pillars — topics you can talk about repeatedly:
1. **The problem** — why it matters, war stories, costs of ignoring it
2. **The solution** — how you think about solving it (not just your product)
3. **Founder journey** — building in public, lessons, vulnerability
4. **Industry insights** — trends, news, takes on your space

### 3. Create the calendar

Based on available hours:

**Minimal plan (2 hrs/week):** 2 posts/week
```
Week 1: Pillar 1 post + Pillar 2 post
Week 2: Pillar 3 post + Pillar 1 post
Week 3: Pillar 4 post + Pillar 2 post
Week 4: Pillar 1 post + Pillar 3 post
```

**Moderate plan (5 hrs/week):** 3 posts + 1 thread
```
Same as minimal + 1 Twitter/X thread per week
```

**Aggressive plan (10 hrs/week):** 4 posts + 2 threads + 1 newsletter
```
Daily posts, 2 deep threads, weekly newsletter
```

### 4. Write `.sales/content-calendar.md`

```markdown
# Content Calendar: <Product Name>

Last updated: <date>

## Content Pillars
1. [Pillar 1] — <description>
2. [Pillar 2] — <description>
3. [Pillar 3] — <description>

## Weekly Schedule
<Based on founder's available hours>

## Day-by-Day (Next 30 Days)

### Week 1
- **Mon:** [Topic] — <brief angle> (Pillar 1)
- **Wed:** [Topic] — <brief angle> (Pillar 2)
- **Fri:** [Thread] — <thread concept> (Pillar 3)

### Week 2
...

## Content Bank
<Extra topic ideas the founder can pull from>
```

### 5. Draft the first week

Write the actual first 3 posts for the founder:
- Title/hook
- Body (draft)
- Call to action (optional)

### 6. Validate

- "Does this feel like content *you* would want to write?"
- "Is the volume realistic for your schedule?"
- "If you could only write one post this week, which would be most valuable?"

## Completion criterion

`.sales/content-calendar.md` exists with a 30-day plan. First week's posts are drafted. Founder has committed to posting at least once this week.
