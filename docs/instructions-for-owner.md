# Instructions for [Owner]: how to drive this project

> Rename this file to the owner's name (e.g. `instructions-for-sam.md`) and fill in the brackets.
> Delete it if the owner is technical and doesn't need a ritual doc.

## The ritual (two moves)

1. Open a **new Terminal window** and type: `[alias]`
   That one word opens this project's folder and starts a Claude session that already knows where it is.
   (To set up the alias, ask Claude: "make me a one-word Terminal shortcut that opens this project and starts Claude.")
2. Say what kind of session it is:
   - **Continue the work:** "pick up the handoff." Claude reads `handoff.md` (and `BULLETIN.md` if there is one) and continues where the last session stopped.
   - **New information arrived:** just say it. "[Person] answered, here's what they said." "The research is in, file it."
   - **A decision landed:** say it plainly. Claude logs it in `decisions.md` and updates whatever depends on it.

## What you never have to do

- **Visit GitHub.** The repo website is how the AI tools stay in sync with each other. Your door is the Terminal word.
- **Copy-paste between AI tools.** Say "check the [project] bulletin" to any of them and it reads the board itself.
- **Remember where things stand.** `handoff.md` always says where things stand; `PLANNING.md` always says what's open; anything you personally need to do is on your calendar.
