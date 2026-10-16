# AGENTS.md: AI context for [project-name]

> Any AI working in this repo: read this file first. It replaces the need for a human to
> re-explain context. Keep it current: when something here changes, update it in the same
> session that changed it. Keep it under ~200 lines; it's re-read on every turn.

## What this repo is
[Purpose in 2–3 sentences. What it produces, who uses it.]

## Where things live
[Key files and folders and their jobs.]

## Rules for this repo
- Read `handoff.md` at the start of every session; the top block is current.
- Read `decisions.md` before any structural change. Don't reopen a Locked row without a new reason.
- When a decision lands, add a numbered row to `decisions.md` in the same session, including the option rejected.
- At session end, add a new top block to `handoff.md` (newest first) ending in a paste-ready prompt.
- Before compacting a long session, save state to `handoff.md` first.
- Anything only the owner can do goes on their calendar with every location written in, not just into chat.
- Nothing from `_private/` gets copied into tracked files.
- [Project-specific rules you could check in a diff, e.g. "prices always include tax."]

## How work is submitted
[Branch and commit conventions, who reviews, what "done" means. Changes to CLAUDE.md and
AGENTS.md get reviewed like any other change. Optional: commit a `.mcp.json` so the repo
carries only the connectors it needs.]

## Big builds
For work touching more than a few files or needing more than ~30 minutes: write a plan and a
progress ledger in `docs/plans/` first, then run each task with a fresh implementer and a
separate fresh reviewer. See `docs/plans/README.md`.

## Who's who
[Roles involved. Roles are enough; skip personal details.]

## Gotchas
[Known traps, stale areas, things that look canonical but aren't.]
