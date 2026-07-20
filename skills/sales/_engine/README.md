# Workspace Engine

Shared I/O and utilities used by all sales skills. Keeps file operations consistent and predictable so skills focus on their actual job, not workspace plumbing.

## How to use

Skills call the engine's procedures as prose instructions. The engine is not a script — it's a shared reference the agent follows.

---

## Procedures

### `check_init()`

Check that `.sales/` workspace exists and has `context.md`.

```
Check if .sales/context.md exists.
If not: tell the user to run /init-sales-workspace first, then stop.
```

### `workspace_status()`

Read `.sales/workspace-status.md` or rebuild it by checking which files exist.

Returns the current state so skills can adapt their behavior based on what's already been done.

### `read_context()`

Read `.sales/context.md` so every skill has the product name, description, founder info, and ICP.

### `read_icp()`

Read `.sales/icp.md` if it exists.

### `write_file(path, content)`

Write a file into `.sales/` with proper headers:

```
Write the file to .sales/<path>
Add a header: "# <Title>" followed by "Last updated: <current date>"
If the file already exists, note the previous content and confirm with the user before overwriting.
```

---

## File Map

Skills reference paths consistently. Never hardcode a path in a skill body — always use these canonical paths:

| Concept | Path |
|---|---|
| Product context | `.sales/context.md` |
| ICP | `.sales/icp.md` |
| Value proposition | `.sales/value-proposition.md` |
| Competitors | `.sales/competitors.md` |
| Pricing | `.sales/pricing.md` |
| Workspace status | `.sales/workspace-status.md` |
| Outreach sequence | `.sales/outreach/sequence-01.md` |
| Outreach templates | `.sales/outreach/templates/<name>.md` |
| Outreach results | `.sales/outreach/results.md` |
| Content calendar | `.sales/content-calendar.md` |
| Call prep | `.sales/calls/<prospect-name>.md` |
| Pipeline | `.sales/pipeline.md` |
