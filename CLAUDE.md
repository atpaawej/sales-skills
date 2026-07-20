# CLAUDE.md — Sales Skills Workspace

Sales skills are in `skills/sales/`. They use a workspace model — each skill reads from and writes to `.sales/` in the founder's project directory.

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
- `/outreach` — one hub for cold emails, LinkedIn DMs, follow-ups, and call prep
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
5. Skills are self-contained — no shared engine or abstraction layer
6. The outreach hub uses reference files (`email-dm.md`, `call-prep.md`, etc.) loaded by the main `SKILL.md` on demand
