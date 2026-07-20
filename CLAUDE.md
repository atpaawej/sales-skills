# CLAUDE.md — Sales Skills Workspace

Sales skills are in `.claude/skills/` or `skills/sales/`. They use a workspace model — each skill reads from and writes to `.sales/` in the founder's project directory.

## Available Skills

All skills are user-invoked (slash-command only):

### Router
- `/sales-navigator` — workspace status dashboard and router

### Setup
- `/init-sales-workspace` — create `.sales/` workspace

### Foundation
- `/icp-definer` — define Ideal Customer Profile
- `/value-prop-crafter` — craft value proposition
- `/competitor-scout` — research competitors
- `/pricing-advisor` — design pricing strategy

### Outreach
- `/cold-email-writer` — generate cold email variations
- `/linkedin-dm-writer` — generate LinkedIn DM scripts
- `/follow-up-sequencer` — build follow-up sequences
- `/call-prepper` — prepare for sales calls
- `/objection-roleplay` — interactive objection practice

### Content
- `/landing-page-drafter` — draft landing page copy
- `/content-planner` — plan 30-day content calendar

### Analysis
- `/outreach-auditor` — review and improve outreach

## How skills work

1. Each skill is a `SKILL.md` file in its own directory under `skills/sales/`
2. Skills read/write `.sales/` files in the founder's current working directory
3. Skills are user-invoked only (`disable-model-invocation: true`)
4. The workspace is the source of truth — skills compose through shared files
