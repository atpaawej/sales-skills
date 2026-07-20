# Sales Skills for Builders

## You can build it. Now teach your agent to help you sell it.

A framework of composable agent skills for **pre-revenue technical founders** who have a product and need customers. Each skill does one thing. They work together. And they store everything in a workspace so you never start from zero.

[![skills.sh](https://skills.sh/b/atpaawej/sales-skills)](https://skills.sh/atpaawej/sales-skills)

Built from the [Sales for Builders](https://salesforbuilders.aawej.in/) course — psychology fundamentals, practical playbooks, and frameworks that actually work in 2026.

## Why this exists

Most technical founders know how to build but never learned how to sell. The standard advice — "just talk to customers" — is true but useless. What do you say? Who do you talk to? How do you handle "it's too expensive"?

This skills framework turns the course's knowledge into **repeatable, agent-executable workflows**. Not hype. Not theory. Just structured steps that produce real output you can use today.

## Installation

```bash
npx skills add atpaawej/sales-skills --all
```

The CLI auto-detects your agent (Claude Code, Codex, Cursor, Cline, and 70+ more) and prompts you to pick which skills to install.

### Options

```bash
# Install to all agents
npx skills add atpaawej/sales-skills --all

# Install only specific skills
npx skills add atpaawej/sales-skills --skill icp-definer --skill outreach

# Install globally (available in every project)
npx skills add atpaawej/sales-skills -g

# Install to specific agents only
npx skills add atpaawej/sales-skills -a claude-code -a cursor

# List available skills without installing
npx skills add atpaawej/sales-skills --list

# Use one skill without installing
npx skills use atpaawej/sales-skills@icp-definer | claude
```

### After Installation

Once installed, open your agent inside your product folder and run:

```bash
/init-sales-workspace
```

This creates a `.sales/` workspace in your current directory. Then run `/sales-navigator` to see your status.

## How it works

```
                    ┌──────────────────────┐
                    │   /sales-navigator    │
                    │  See where you are   │
                    └──────┬───────────────┘
                           │
            ┌──────────────┼──────────────┐
            ▼              ▼              ▼
   ┌─────────────┐ ┌──────────────┐ ┌──────────────┐
   │ /icp-definer│ │/value-prop-  │ │/competitor-  │
   │             │ │crafter       │ │scout         │
   └─────────────┘ └──────────────┘ └──────────────┘
            │              │              │
            └──────────────┼──────────────┘
                           ▼
            ┌──────────────────────────────┐
            │         /outreach hub         │
            │  First touch · Follow-ups    │
            │  Call prep                   │
            └──────────────────────────────┘
                           │
            ┌──────────────┼──────────────┐
            ▼              ▼              ▼
   ┌─────────────┐ ┌──────────────┐ ┌──────────────┐
   │/pricing-    │ │/landing-page │ │/objection-   │
   │advisor      │ │-drafter      │ │roleplay      │
   └─────────────┘ └──────────────┘ └──────────────┘
                           │
                    ┌──────┴──────┐
                    ▼             ▼
           ┌─────────────┐ ┌──────────────┐
           │/content-    │ │/outreach-    │
           │planner      │ │auditor       │
           └─────────────┘ └──────────────┘
```

Every skill reads from and writes to a `.sales/` directory in your project folder. Data persists. Sessions resume. Skills build on each other.

## Skills

### 🧭 Router
| Skill | What it does |
|---|---|
| `/sales-navigator` | Reads your workspace, shows your status, recommends what to do next |

### 🏗️ Foundation
| Skill | What it does |
|---|---|
| `/init-sales-workspace` | Creates `.sales/` with scaffolded files — run once per product |
| `/icp-definer` | Defines your ICP with deep research, evidence, and peer-model pushback |
| `/value-prop-crafter` | Positions your product using April Dunford's framework |
| `/competitor-scout` | Researches competitors and finds your real differentiator |
| `/pricing-advisor` | Designs value-based pricing with anchoring and psychology |

### 📧 Outreach Hub
| Skill | What it does |
|---|---|
| `/outreach` | One hub for cold emails, LinkedIn DMs, follow-up sequences, and call prep |
| `/objection-roleplay` | Interactive practice — agent plays skeptical prospect |

### 📝 Content
| Skill | What it does |
|---|---|
| `/landing-page-drafter` | Drafts full landing page copy section by section |
| `/content-planner` | Plans 30-day content calendar with first week drafts |

### 📊 Analysis
| Skill | What it does |
|---|---|
| `/outreach-auditor` | Reviews past outreach and gives 3 actionable changes |

## Quickstart

```bash
# 1. Install the skills
npx skills add atpaawej/sales-skills --all

# 2. Create a folder for your product
mkdir my-product-sales
cd my-product-sales

# 3. Open your agent and initialize the workspace
/init-sales-workspace

# 4. See where you stand
/sales-navigator

# 5. Define who to sell to
/icp-definer

# 6. Write your first outreach
/outreach
```

## The Workspace Model

Skills are stateless in the session but stateful through the workspace. Data persists between runs.

```
my-product-sales/
└── .sales/
    ├── context.md              # Product info and founder context
    ├── icp.md                  # Ideal Customer Profile
    ├── value-proposition.md    # Positioning and messaging
    ├── competitors.md          # Competitive landscape
    ├── pricing.md              # Pricing tiers and strategy
    ├── outreach/               # Outreach sequences and results
    ├── pipeline.md             # Deal tracker
    ├── content-calendar.md     # Content plan
    ├── calls/                  # Call preps and notes
    ├── workspace-status.md     # Auto-generated status
    └── voice-examples.md       # Founder's authentic voice samples
```

## Design Principles

Every skill follows the same core interaction:

1. **Research first** — no questions to the founder until the skill has done its own work
2. **Present with evidence** — here's what I found, here's why, here's my recommendation
3. **Founder reacts** — "that's right," "that's wrong but here's what's closer to the truth," or "I disagree"
4. **Peer-model pushback** — if the founder's instinct is counterproductive (e.g., targeting everyone), the skill pushes back with psychology and evidence
5. **Persistence** — before asking the founder anything, check the workspace. If the answer already exists, use it. If not, ask and save it.

Three core rules:
- **Agent writes, founder sends.** No skill ever automates sending. Every skill ends with a handoff to human action.
- **Workspace as source of truth.** Skills compose through shared files, not session memory.
- **MCP when needed, web search otherwise.** Skills use browser tools for specific tasks (visiting landing pages, checking competitor sites); web search is the daily driver.

## Built from

- [Sales for Builders](https://salesforbuilders.aawej.in/) — free sales course for technical founders
- [Writing Great Skills](https://github.com/aawej/writing-great-skills) — principles for designing predictable agent behaviors
- The [skills framework](https://github.com/mattpocock/skills) pattern by Matt Pocock
- [skills.sh](https://skills.sh) — the open agent skills CLI by Vercel Labs

## Out of Scope

This framework has intentional boundaries. See [out of scope](./.outofscope/README.md) for details — skills will not send messages, replace a CRM, integrate with platforms, or handle enterprise sales cycles.

## License

MIT
