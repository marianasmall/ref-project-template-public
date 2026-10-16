<!-- ============ ABOUT THIS TEMPLATE: delete from here to the END marker after you spawn a repo ============ -->

# Project template

A ready-made set of project files that lets you, a fresh Claude Code session, or any other AI tool pick up a project cold, without anyone re-explaining it.

It pairs with the **[Never lose a project](https://github.com/marianasmall/claude-code-starter-kit/blob/main/docs/never-lose-a-project.md)** guide in the Claude Code Starter Kit, which explains what each file is for, the end-of-session loop that keeps them true, and why. You can use this template without the kit; the kit's `/kit:session-end`, `/kit:handoff`, and `/kit:scaffold-project` commands just make the loop automatic.

## Use this template

1. On GitHub, click **Use this template → Create a new repository**.
2. Name it with a category prefix, all lowercase with hyphens: `project-`, `client-`, `site-`, `app-`, `config-`, `brand-`, `ref-`, or `archive-` (for example `client-hollow-oak-bakery`). Choose **Private** unless you mean to publish it.
3. Clone it into your projects folder and open Claude Code there.
4. Say: *"This repo was just made from the project template. Help me fill in README, AGENTS.md, and PLANNING.md, then delete what I don't need."*

## What's inside

| File | Its one job | Keep it? |
|---|---|---|
| `README.md` | What this is, in plain language, for humans | Always. Delete this "About this template" section |
| `AGENTS.md` | Everything an AI needs to brief itself | Always |
| `CLAUDE.md` | One line (`@AGENTS.md`) so Claude Code loads `AGENTS.md` automatically | Always |
| `PLANNING.md` | Goal, scope, roadmap, current state | Always |
| `decisions.md` | Numbered decisions, with the options you rejected | Always |
| `handoff.md` | Where the last session stopped, newest block on top | Always |
| `.gitignore` | Keeps `_private/`, `CLAUDE.local.md`, `.env` files, and `_backups/` out of git | Always |
| `.gitleaks.toml` | Settings for [gitleaks](https://github.com/gitleaks/gitleaks), a scanner that catches passwords and keys before you commit them | Keep if you use gitleaks |
| `BULLETIN.md` | Message board for when two or more AI tools work the same project | Delete if only one AI tool works here |
| `docs/instructions-for-owner.md` | The owner's whole ritual in plain words | Delete if the owner doesn't need it |
| `docs/plans/` | Plan and progress-ledger templates for big builds | Keep; it's small |
| `docs/template-examples.md` | Filled-in fictional examples of each file | Delete once you've read it |
| `.claude/rules/_example-topic.md.example` | Stub for a rule that loads only for certain files | Delete if unused |
| `LICENSE` | MIT license for this template | Replace with your own, or delete for a private repo |

## About `_private/`

Create a `_private/` folder for anything you wouldn't publish. It's listed in `.gitignore`, so git skips it and a normal commit won't push it to GitHub. That's all it does: it isn't encrypted, a forced `git add` can still commit it, and cloud-sync software will still copy it if your projects folder is synced. The rule also only covers files git isn't already tracking; if something in `_private/` was committed earlier, run `git rm -r --cached _private/` once (it stays in the repo's history). Keep passwords and API keys in a password manager, not in project files.

`handoff.md` and `decisions.md` are committed on purpose, so they go wherever the repo goes. In a public or widely shared repo, keep names and sensitive detail in `_private/` instead.

<!-- ============ END of "about this template". Everything below is your project's README. ============ -->

# [Project Name]

> One sentence: what this is.

## What this is
[What this repo holds, who it's for, what it produces.]

## How to use it
[Where to start, what to open first.]

## Key files
| Path | What's there |
|---|---|
| `AGENTS.md` | AI context. Any model reads this first |
| `PLANNING.md` | Goal, scope, roadmap |
| `decisions.md` | Numbered decision log |
| `handoff.md` | Where the last session stopped |
