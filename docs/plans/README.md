# Plans

Big builds get planned here before anything is built. "Big" means roughly: more than three or
four files, several decisions that depend on each other, or more than about half an hour of
focused work. Small fixes don't need a plan.

## The pattern

1. **Plan on disk.** Copy `_TEMPLATE-plan.md` to `YYYY-MM-DD-<slug>-plan.md`. Break the job into
   small numbered tasks, each with what "done" looks like and how to check it.
2. **Progress ledger next to it.** Copy `_TEMPLATE-PROGRESS.md` to `YYYY-MM-DD-<slug>-PROGRESS.md`.
   One line per task: status, commit, reviewer notes. This file is what survives a crash or a
   compaction; a new session reads it and knows which task is next.
3. **Fresh implementer per task, separate fresh reviewer per task.** Each task goes to a new
   subagent (a helper session with a clean slate) that reads only the plan and its task. A second
   new subagent reviews the result and tries to break it. Fix what it finds, re-review that part.
4. **The main session coordinates; it doesn't build.** It hands out tasks, reads results, and
   updates the ledger, which keeps its own context clean for the whole build.
5. **Match the model to the job.** Most capable model for design judgment and the final review of
   the whole build; a lighter one for well-specified tasks.

You can ask for this directly: *"Write a plan with a progress ledger in docs/plans, then run it
with a fresh implementer and reviewer per task."*
