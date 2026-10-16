# 10 — Guided Actions and Buttons

The rule the whole product is designed by: **the user always knows the one
next thing to do.** Buttons are not decoration — they are the workflow made
visible. They carry the user from Hold to Ship so their cognitive energy
goes to the idea, not to figuring out the tool.

## The seven rules

1. **No dead ends.** Every screen and every state ends with exactly **one
   primary button**. Secondary actions are quiet text links. Three
   competing primary buttons is a design defect, not a choice.
2. **Buttons say what happens.** Verb + object, in the user's words:
   "Write today's direction", "See it as a map", "Mark as shipped".
   Banned as primary labels: OK, Submit, Continue, Next, Get started
   (without an object).
3. **The system carries the memory.** Where the next step depends on
   history, the button or the screen shows it: tomorrow's Question is
   drafted from the Eye's flags; the resume card shows the last Takeaway
   and Tweak. The user should never have to recall state the product knows.
4. **Position is always visible.** The Work header shows loop position —
   Hold ✓ · Direct ● · See ○ · Ship ○ — so "where am I" costs zero thought.
5. **Empty is a direction, not a void.** Every empty state has one line of
   plain text and one primary button. A blank canvas is never a first screen.
6. **Escape is quiet.** "Back to stream" is always available as a text link.
   It is never the primary button; leaving must exist but never shout.
7. **Few decisions, real ones only.** The daily loop is budgeted at
   **3 decisions**: which Work (defaulted to the last active one), today's
   one Tweak, and Revise-or-Derive. Everything else is defaulted, queued,
   or deferred by the system — and say so on screen.

## The one exception: the genuine fork

The Daily Direction apply step has **two** buttons, because the choice is
real (see `02-workspace-workflow.md`, ADR-002). Each is labelled with its
consequence, so the user chooses by outcome, not by guessing:

- **Revise the file** — "Creates the next version. The original is kept."
- **Make something new** — "The file stays as it is. Adds a card linked to it."

No other screen may use two primary buttons without a decision record.

## Button map — primary action per state

| State the user is in | The one primary button |
| --- | --- |
| Empty stream (no Works yet) | **Upload your first file** (quiet link: "or start with a note") |
| File uploading / splitting | No button — a named progress state ("Splitting into sections…"). Never a bare spinner |
| Work just Held | **Write today's direction** |
| Daily Direction form complete | **Revise the file** / **Make something new** (the fork, above) |
| Directed, Eye not yet viewed | **See it as a map** |
| Eye open, flags present | On each flag: **Use as tomorrow's question** |
| Eye open, no flags | **Done for today** (→ day-close screen) |
| Day close | Shows today's Takeaway + Tweak and tomorrow's drafted Question. Button: **Draw today's flower** (→ the Garden, docs/11; after planting, **Back to stream**) |
| Garden, today's plot unplanted, day's action done | **Draw today's flower** (traced guide; under a minute) |
| Garden, no action yet today | No plant button at all — one quiet line: "A direction plants today's flower." plus **Write today's direction**. The garden never asks for a login-only visit |
| Returning user, active Work waiting | **Continue this Work** (on the resume card) |
| Work judged finished by the user | **Mark as shipped** (in the Work header menu, confirmed in one step) |
| Work Shipped | **Start a new Work** |
| Note written with no Work attached | **Attach it to a Work** (quiet link: "keep it as a Seed") |
| A 4th Work would exceed the WIP limit | **Rest a Work first** (opens the chooser; creating is blocked kindly, not silently) |

## Anti-patterns (banned)

- A blank first screen, a dashboard of widgets with no next step, or a
  "Welcome!" screen that asks the user to explore.
- Icon-only navigation with no labels anywhere in the core loop.
- Modal chains (a dialog that opens a dialog), and settings offered before
  the first Work exists.
- Guilt mechanics: streak warnings, red badges, "you missed a day" copy.
  Direction is offered, never enforced with shame.
- Hiding the next step inside a menu when the state table above assigns
  it a primary button.

## Test for any new screen (before it is "designed")

1. Cover everything except the primary button: does it still tell the user
   what this screen is for?
2. Count the decisions on the screen. More than the budget for its step?
   Default or defer something.
3. Arrive here as a returning user with no memory of yesterday: does the
   screen itself restore the context (position, last action, drafted next
   step)?
