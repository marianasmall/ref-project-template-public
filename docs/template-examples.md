# Filled-in examples (fictional)

> Delete this file once you've read it. Everything here is made up: "Hollow Oak Bakery" is an
> imaginary neighborhood bakery getting a simple website (home page, menu page, order-ahead form).
> The point is to show what real entries look like, which empty templates can't.

## decisions.md

```markdown
# Decisions: client-hollow-oak-bakery

> Append-only. Newest at top. Read before any structural change. Do not reopen
> a Locked row without a new reason, and say what the new reason is.

## Locked

| # | Date | Decision | Why | Rejected |
|---|---|---|---|---|
| D-9 | 2026-03-12 | Menu photos are the owner's own phone photos, shot on the shop counter. | Real bread sells better than stock; the owner already has 40+ usable shots. | Stock photography (looks generic, licensing to track). Hiring a photographer (owner said "not this year"). |
| D-8 | 2026-03-10 | Order-ahead uses a simple form that emails the shop, not a payment system. | The shop takes payment at pickup today and wants to keep it that way for launch. | Online checkout (fees, refunds, more to maintain). Revisit after 3 months of order volume. |
| D-7 | 2026-03-08 | Allergen information appears on the menu page only after the owner signs off on each item, in writing. | Wrong allergen info is a safety problem, not a typo. | Copying allergen notes from the old printed menu (it is two years out of date). |

## Open

| # | Question | Owner | Settle by |
|---|---|---|---|
| Q-3 | Show prices on the menu page, or "ask in store"? | Owner | 2026-03-19 |
```

## handoff.md, top block

```markdown
# Handoff: client-hollow-oak-bakery

> **▶ 2026-03-12 4:40 PM. READ THIS FIRST.**
> - **Done:** home page copy final; menu page layout built on branch `menu-page-2026-03-12` (commit a1b2c3d), photos placed per D-9.
> - **Mid-flight:** order-ahead form (D-8) is wired but untested; test send goes to our own inbox, not the shop's.
> - **Waiting on the owner:** price decision (Q-3) and allergen sign-off for 6 items (D-7). Both on the calendar for Fri 3/13, with the item list in the event.
> - **Next:** test the form end to end, then open a pull request for the menu page.
> - **Don't touch:** allergen lines stay as "pending sign-off" placeholders until D-7 is satisfied.

--- PASTE BELOW ---

Continuing the Hollow Oak Bakery website in ~/Projects/client-hollow-oak-bakery,
branch menu-page-2026-03-12.

Read first: AGENTS.md (loads automatically), then this handoff, then decisions.md
D-7 to D-9.

State: menu page built, order form wired but untested. Prices and allergen
sign-off are waiting on the owner (calendar, Fri 3/13).

First action: send a test order through the form to our own inbox and confirm
the email arrives with every field. Do not change allergen placeholders.

---

## Earlier sessions

> **2026-03-10 11:15 AM.** Home page copy drafted; D-8 settled (email form, no checkout). Next was the menu layout.
```

## Session summary

Session summaries live outside the repo (a log file, or a notes database), one per session,
always with the same fields.

```markdown
## 2026-03-12 16:40 — Bakery site: menu page + order form

**What was done:**
- Built the menu page layout with the owner's photos (D-9)
- Wired the order-ahead form to email the shop (D-8); not yet tested
- Files: site/menu.html, site/order.html, site/css/menu.css

**Decisions:**
- D-9: owner's own photos. Rejected stock (generic, licensing) and a hired photographer (owner declined).

**Open loops:**
- Owner owes: price decision (Q-3) and allergen sign-off for 6 items. Calendar, Fri 3/13.
- We owe: end-to-end form test before the pull request.

**Next steps:**
- Test the form, then open the menu-page pull request.

**Where state lives:**
- ~/Projects/client-hollow-oak-bakery, branch menu-page-2026-03-12
- handoff.md (top block), decisions.md (D-7 to D-9, Q-3)

**Transcript:** ~/.claude/projects/<project-folder>/<session-id>.jsonl
```

## Compacting a long session

Save state to `handoff.md` first, then compact with a focus line that names what must survive:

```
/compact Keep: the bakery site menu-page work on branch menu-page-2026-03-12, open Q-3 (prices), the owner owes allergen sign-off (calendar Fri), and the rule to never publish allergen claims without the owner's sign-off. Drop: the font-comparison tool output.
```
