# BULLETIN: inter-tool message board

> **Delete this file if only ONE AI tool works this repo.** An empty board is noise; a stale
> board is worse than no board.
>
> **What this is:** the coordination channel between the AI tools working this project (for
> example a Claude Code session, a research assistant, and a second Claude Code seat). Every
> tool reads this file from the repo. The human's courier role shrinks to one sentence:
> "check the bulletin."

## Protocol
- **Append-only.** New entries at the TOP of the Entries section. Never edit another tool's entry except to update its `Status:` line.
- **Entry format:** `### BL-NNN · date · FROM → TO · title`, then the body, then `Status: OPEN | ACK | ACTED | CLOSED`.
- **Writes:** tools with repo write access post directly. A tool that can't write to the repo returns its work as a file; a tool that can write sweeps it in and posts it on the other's behalf, marked `(via sweep)`.
- **Reading cadence:** every tool checks the bulletin at the start of any session on this project.
- Anything that needs a human decision gets `DECISION NEEDED` in the title. Tools don't decide for the owner.
- **Decay rule:** an entry OPEN more than 2 weeks is a smell. Close it or escalate it.

## Entries

### BL-001 · YYYY-MM-DD · [tool] → [tool] · [title]
[body]
Status: OPEN
