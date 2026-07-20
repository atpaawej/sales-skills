---
name: sales-navigator
description: See your sales workspace status at a glance. Shows what's done, what's next, and routes you to the right skill.
disable-model-invocation: true
---

# Sales Navigator

The entry point. Reads your `.sales/` workspace, shows your status, and helps you decide what to do next.

---

## Flow

### 1. Read workspace status

Check which files exist in `.sales/`:

| File exists | What it means |
|---|---|
| `.sales/context.md` | Workspace initialized |
| `.sales/icp.md` | ICP defined |
| `.sales/value-proposition.md` | Value proposition crafted |
| `.sales/competitors.md` | Competition mapped |
| `.sales/pricing.md` | Pricing strategy done |
| `.sales/outreach/sequence-01.md` | Outreach drafted |
| `.sales/calls/` — has files | Calls happening |
| `.sales/pipeline.md` — has entries | Active pipeline |
| `.sales/content-calendar.md` | Content plan active |

Update `.sales/workspace-status.md` with the current state.

### 2. Show dashboard

Print the founder's status:

```
╔══════════════════════════════════════════╗
║  Sales Navigator — <Product Name>       ║
╚══════════════════════════════════════════╝

📋 Context      ✅ Done  (last updated <date>)
🎯 ICP          ❌ Not yet defined
💬 Value Prop   ❌ Not yet defined
🏢 Competitors  ❌ Not mapped
💰 Pricing      ❌ Not set
📧 Outreach     ❌ Not drafted
📞 Calls        — No activity yet
📊 Pipeline     — Empty
📅 Content      ❌ No plan

─── RECOMMENDED NEXT ───
→ Run /icp-definer  — who are you selling to?
```

**Recommendation logic:**
- If `context.md` missing → recommend `/init-sales-workspace`
- If `context.md` exists but `icp.md` missing → recommend `/icp-definer`
- If `icp.md` exists but `value-proposition.md` missing → recommend `/value-prop-crafter`
- If `value-proposition.md` exists but `outreach/` has no sequences → recommend `/outreach`
- If `competitors.md` missing → suggest `/competitor-scout` (non-blocking)
- If `pricing.md` missing → suggest `/pricing-advisor` (non-blocking)
- If outreach exists but `pipeline.md` is empty → suggest starting to prospect
- If calls are happening → suggest `/objection-roleplay`
- If content plan missing → suggest `/content-planner` (non-blocking)

### 3. Route the founder

> "Where do you want to go? (Type the skill name, e.g. `/icp-definer`)"

If they type a skill name, invoke it. If they're unsure, recommend the next step based on the dependency chain.

---

## Completion criterion

The founder has a clear picture of their sales workspace status and knows what to do next — either by choosing a skill or following the recommendation.
