---
name: outreach
description: Handle all outreach — write cold emails and LinkedIn DMs, build follow-up sequences, prep for calls. One hub for every touch.
disable-model-invocation: true
---

# Outreach Hub

One entry point for every stage of outreach. Writes first-touch messages, designs follow-up sequences, preps calls, and coaches on delivery.

The agent writes. Only you send.

---

## Prerequisites

`.sales/context.md`, `.sales/icp.md`, and `.sales/value-proposition.md` must exist.

---

## Flow

### 1. Read workspace

Read `.sales/context.md`, `.sales/icp.md`, `.sales/value-proposition.md`. Read `.sales/competitors.md` if it exists — competitive scripts feed into call prep.

Read existing outreach files in `.sales/outreach/` — build on what's already there rather than starting from zero each time.

Check `.sales/voice-examples.md` if it exists — match the founder's natural tone.

### 2. Research the ICP's current world (one pass)

Before branching, do one research pass that every branch benefits from:

- What is your ICP talking about right now? Search for recent posts, threads, news
- What's the #1 problem they're complaining about in their niche?
- Any recent news or trend affecting them?
- What language do they use when describing the pain? Collect specific phrases

### 3. Discover intent

Ask:
> "What do you need right now?"
>
> **a)** Write cold emails or LinkedIn DMs — first-touch messages
> **b)** Build a follow-up sequence — nurture prospects who haven't replied
> **c)** Prep for a call with [prospect] — research + call flow + objection scripts

Route to the matching flow below.

---

## Branch A: First-touch messages

Follow `outreach/email-dm.md` for the full flow. Summary:

1. **Ask for the target** — specific person/company or profile type
2. **Determine channel** — email (4-sentence formula) or LinkedIn DM (300-char connection + gate question)
3. **Write 3 variations** — curiosity hook, pain-first, social proof
4. **Present + validate** — "Which variation would get a reply from your prospect?"
5. **Write** — to `.sales/outreach/sequence-01.md` or `.sales/outreach/templates/linkedin-dm.md`

---

## Branch B: Follow-up sequence

Follow `outreach/follow-up-sequence.md` for the full flow. Summary:

1. **Read existing sequence** — what was the first touch? What channel?
2. **Design 5-touch sequence** — initial (already sent), Day 3 (new angle), Day 7 (social proof), Day 14 (break-up), Day 30-45 (re-engagement)
3. **Cross-channel strategy** — if founder has email + LinkedIn, mix them
4. **Present + validate** — "Does this timing work for your prospect's world?"
5. **Write** — to `.sales/outreach/templates/follow-up-sequence.md`

---

## Branch C: Call prep

Follow `outreach/call-prep.md` for the full flow. Summary:

1. **Ask for the prospect** — name, company, role, how they know the founder
2. **Research** — LinkedIn, company, recent news, mutual connections. MCP browser if available.
3. **Write call flow** — Rapport (2-3min) → Discovery (15min, 70% listening) → Offer (5min) → Handle objections → Next steps
4. **Pre-write objection scripts** — 3-4 specific objections this prospect is likely to raise
5. **Write** — to `.sales/calls/<prospect-name>.md`

---

## Post-flow: Validate

For message-based branches:
> "Read Option [X] aloud. Does it sound like you? Would it get a reply from your ICP?"

For call prep:
> "Read the discovery questions. Do these feel natural, or do they sound scripted?"

If the founder hesitates, refine. If they say "sounds good," confirm and proceed.

---

## Write workspace

Write to the appropriate file depending on the branch.

Update `.sales/outreach/results.md` if the founder reports any results during the session.

---

## Close

> "Your [emails/sequence/call prep] is ready. Send them today — perfect doesn't send. If you get replies, I can help prep for the next step. If you don't, I can help iterate.
>
> Run `/objection-roleplay` if you want to practice handling objections. Run `/sales-navigator` to see your overall status."

---

## Completion criterion

The outreach file exists (sequence, templates, or call prep). The founder has reviewed the output and confirmed it's ready to use. For call prep: the founder can review it in 5 minutes before the call.
