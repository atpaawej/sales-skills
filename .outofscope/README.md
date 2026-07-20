# Out of Scope

This document defines what Sales Skills for Builders explicitly **does not do**. Every skill has boundaries. These boundaries are intentional — they keep the framework focused, fast, and honest.

---

## 1. Cannot Do The Founder's Job

| Thing | Why it's out of scope |
|---|---|
| **Sending emails or DMs** | The agent drafts. The founder hits send. No skill will ever automate the sending. |
| **Taking sales calls** | No agent can take a call for you. Skills prep you, but you show up. |
| **Building relationships** | Skills can suggest who to connect with. They can't build trust or rapport. |
| **Making pricing decisions** | Skills generate options and psychology rationale. The founder decides the number. |
| **Validating positioning** | Skills produce options. Only the founder can say "that doesn't sound like me." |
| **Shipping content** | Skills draft. The founder posts, publishes, or sends. |

**Principle:** Agent writes, founder sends. No skill in this framework produces a sale by itself. Every skill ends with a handoff to human action.

---

## 2. Not a CRM

The `.sales/` workspace stores markdown files. It is not:

- A database with query capabilities
- A deal pipeline with drag-and-drop stages
- A customer relationship management system
- A replacement for tools like HubSpot, Pipedrive, or Folk

If a founder needs CRM features, they should use a CRM. The skills framework feeds into their workflow — it does not replace it.

---

## 3. Not a Marketing Platform

Skills do not:

- Send automated email campaigns (no Mailchimp, ConvertKit, or similar integration)
- Schedule social media posts
- Run ad campaigns (Google Ads, Meta Ads, LinkedIn Ads)
- Track website analytics
- Manage SEO rankings

These are platform concerns. The skills help you *plan* content and *draft* copy. Distribution and measurement are separate tools.

---

## 4. Not a Code Framework

Each skill is a `SKILL.md` file — markdown with YAML frontmatter. Skills are not:

- Executable scripts or programs
- API endpoints or web services
- npm packages or libraries
- Containers or microservices
- Any form of compiled or interpreted code

They are instruction sets for an AI agent. The agent reads the markdown and executes the steps conversationally.

---

## 5. Not One-Size-Fits-All Advice

This framework is built from the [Sales for Builders](https://salesforbuilders.aawej.in/) course. The approaches used — 4-sentence cold email, ICP-first positioning, value-based pricing, Feel-Felt-Found objections — are chosen for a specific context.

Skills will not:

- Adapt to every sales methodology (MEDDIC, Challenger, SPIN, Sandler, etc.)
- Handle enterprise sales cycles (multi-stakeholder, multi-month, multi-region)
- Handle regulated industries without modification (finance, healthcare, legal)
- Replace domain expertise (if you're selling to doctors, the agent doesn't know medicine)

The target user is a **pre-revenue technical founder selling to other technical or business buyers**. If that's not you, some assumptions will break.

---

## 6. Not a Replacement for the Course

The skills implement specific, agent-doable slices of the Sales for Builders course. They do not replace:

- Reading the psychology foundation (why people buy, the ethics of persuasion)
- Internalizing the mindset shift (from builder to seller, imposter syndrome work)
- Learning from the Founder Library stories (Pieter Levels, Marc Lou, Alex Hormozi)

The skills are **execution tools**, not education. Founders who skip the course miss the context that makes the skills effective.

---

## 7. No Multi-User or Team Features

The workspace model is designed for a solo founder working alone. It does not include:

- Shared workspaces across team members
- Role-based access or permissions
- Merge conflict resolution for `.sales/` files
- Audit trails or change history (beyond what git provides)

If you're a team, each founder runs their own workspace, or you layer this on top of your own collaboration tools.

---

## 8. No Platform Integrations

Skills ship as standalone `SKILL.md` files. They will not include:

- API integrations (Notion, Slack, Google Sheets, Airtable, etc.)
- Webhooks or automation triggers (Zapier, Make, n8n)
- OAuth or authentication flows
- Database connections or query layers

If a founder wants to connect `.sales/` output to other tools, that is their DIY layer. The data is plain markdown — pipe it anywhere.

---

## Why These Boundaries Exist

Every feature that shipped would create an expectation of maintenance, compatibility, and support. These boundaries keep the framework:

- **Light** — installs in seconds, works in any agent, no dependencies
- **Honest** — no illusion that an agent can replace the founder's job
- **Composable** — fits into whatever else the founder already uses
- **Iterable** — easy to fork, modify, or throw away and rebuild

If a skill tries to do too much, it does nothing well. These boundaries protect the one-thing-well principle.
