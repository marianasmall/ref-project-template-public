@AGENTS.md

<!-- This file exists so Claude Code loads AGENTS.md automatically at session start (the @ line
     imports it). Keep this file tiny: it is paid for on every turn. Narrow detail goes in
     .claude/rules/<topic>.md with `paths:` frontmatter (see .claude/rules/_example-topic.md.example).
     Personal notes go in CLAUDE.local.md, which is gitignored.
     Owner: [name]. Changes to this file get reviewed like code. -->

# Compact instructions

When compacting, keep: files changed this session and why; open decisions and who owns them;
the next step from `handoff.md`; anything waiting on the owner; any "don't touch" areas named
in `AGENTS.md`. Drop: exploratory dead ends and raw tool output already saved to files.
