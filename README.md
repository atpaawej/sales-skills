# Sales Skills for Builders

## You can build it. Now teach your agent to help you sell it.

A framework of composable agent skills for **pre-revenue technical founders** who have a product and need customers. Each skill does one thing. They work together. And they store everything in a workspace so you never start from zero.

Built from the [Sales for Builders](https://salesforbuilders.aawej.in/) course — psychology fundamentals, practical playbooks, and frameworks that actually work in 2026.

## Why this exists

Most technical founders know how to build but never learned how to sell. The standard advice — "just talk to customers" — is true but useless. What do you say? Who do you talk to? How do you handle "it's too expensive"?

This skills framework turns the course's knowledge into **repeatable, agent-executable workflows**. Not hype. Not theory. Just structured steps that produce real output you can use today.

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
            │       Outreach Skills        │
            │  /cold-email-writer          │
            │  /linkedin-dm-writer         │
            │  /follow-up-sequencer        │
            │  /call-prepper               │
            │  /objection-roleplay         │
            └──────────────────────────────┘
                           │
            ┌──────────────┴──────────────┐
            ▼                             ▼
   ┌──────────────┐              ┌──────────────┐
   │/pricing-     │              │/landing-page │
   │advisor       │              │-drafter      │
   └──────────────┘              └──────────────┘
```

Every skill reads from and writes to a `.sales/` directory in your project folder. Data persists. Sessions resume. Skills build on each other.

## Skills

### 🧭 Router
| Skill | What it does |
|---|---|
| `/sales-navigator` | Reads your workspace, shows your status, and recommends what to do next |

### 🏗️ Foundation
| Skill | What it does |
|---|---|
| `/init-sales-workspace` | Creates `.sales/` with scaffolded files — run once per product |
| `/icp-definer` | Defines your Ideal Customer Profile with research and validation |
| `/value-prop-crafter` | Positions your product using April Dunford's framework |
| `/competitor-scout` | Researches competitors and finds your differentiator |
| `/pricing-advisor` | Designs tiered pricing with anchoring, decoys, and psychology |

### 📧 Outreach
| Skill | What it does |
|---|---|
| `/cold-email-writer` | Generates 4-sentence cold emails with follow-ups |
| `/linkedin-dm-writer` | Writes connection requests + gate-question DMs |
| `/follow-up-sequencer` | Builds 5-touch follow-up sequences |
| `/call-prepper` | Researches prospects, writes call flows, preps objections |
| `/objection-roleplay` | Interactive roleplay — agent plays prospect, you practice |

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
# 1. Create a folder for your product
mkdir my-product-sales
cd my-product-sales

# 2. Initialize the workspace (inside Claude Code)
/init-sales-workspace

# 3. See where you stand
/sales-navigator

# 4. Define who to sell to
/icp-definer

# 5. Write your first cold emails
/cold-email-writer
```

## The Workspace Model

Skills are stateless in the session but stateful through the workspace.

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
    └── calls/                  # Call preps and notes
```

## Principles

- **One skill, one job.** Each skill does exactly one thing well.
- **Agent writes, founder sends.** No illusion of progress. The agent prepares; the founder executes.
- **Workspace as source of truth.** Skills compose through shared files, not session memory.
- **Start with who, not how.** `/icp-definer` comes first because everything else depends on knowing who you're selling to.

## Built from

- [Sales for Builders](https://salesforbuilders.aawej.in/) — free sales course for technical founders
- The [skills framework](https://github.com/mattpocock/skills) pattern by Matt Pocock — composable, predictable, repeatable

## License

MIT
