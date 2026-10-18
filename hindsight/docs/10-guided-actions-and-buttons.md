# 10 - Guided Actions and Buttons

The rule for the whole product: **the user always knows the one next
step.** Buttons are not trim. Buttons are the workflow, made clear on
screen. They walk the user from Hold to Ship. So the user's mind
stays on the idea, not on the tool.

## The seven rules

1. **No dead ends.** Each screen and each state ends with **one main
   button**. Other acts are quiet text links. Three main buttons in a
   row is a design fault, not a choice for the user.
2. **Buttons say what will happen.** Verb plus object, in the user's
   words: "Write today's direction", "See it as a map", "Mark as
   shipped". Banned as main button text: OK, Submit, Continue, Next,
   Get started (with no object).
3. **The app holds the past, so the user does not have to.** If the
   next step needs past state, the screen shows it. The Eye's flags
   draft the next day's Question. The return card shows the last
   Takeaway and the last Tweak.
4. **Place in the loop is on screen at all times.** The Work top bar
   shows: Hold (done) · Direct (now) · See (next) · Ship (last). So
   "where am I" costs no thought.
5. **An empty screen is a step, not a hole.** Each empty state has one
   line of plain text and one main button. A blank first screen is
   banned.
6. **The exit is quiet.** "Back to stream" is there at all times, as a
   text link. It is never the main button. A way out must exist. It
   must not shout.
7. **Few picks, and real ones only.** The daily loop has a budget of
   **3 picks**: which Work (set to the last live one if the user does
   not pick), today's one Tweak, and Revise or Derive. All else is set
   by the app, put in a queue, or pushed to a later day. And the
   screen says so.

## The one case with two buttons: the real fork

The Daily Direction apply step has **two** buttons. The pick is real.
See `02` and ADR-002 in `decisions/`. Each button says what it will do,
so the user picks by result, not by a guess:

- **Revise the file** - "Makes the next version. The old one is kept."
- **Make something new** - "The file stays as is. Adds a card with a link to it."

No other screen gets two main buttons, but with one way out: a record
in `decisions/` that says why.

## Button map: the main button for each state

| State | The one main button |
| --- | --- |
| Empty stream, no Works yet | **Upload your first file** (quiet link: "or start with a note") |
| File uploads or splits | No button. A named load state: "Splitting into sections..." Never a bare spin wheel |
| Work just Held | **Write today's direction** |
| Daily Direction form is full | **Revise the file** / **Make something new** (the fork, see above) |
| Directed, Eye not seen yet | **See it as a map** |
| Eye is open, flags are up | On each flag: **Use as tomorrow's question** |
| Eye is open, no flags | **Done for today** (goes to the day close screen) |
| Day close | The screen shows today's Takeaway and Tweak, and the draft Question for the next day. Button: **Draw today's flower** (goes to the Garden, see `11`. After the plant is drawn: **Back to stream**) |
| Garden, today's plot is bare, day's act is done | **Draw today's flower** (with a trace guide. Takes under a minute) |
| Garden, no act yet today | No plant button. One quiet line: "A direction plants today's flower." Plus: **Write today's direction**. The Garden never asks for a bare login visit |
| User comes back, a live Work waits | **Continue this Work** (on the return card) |
| User calls the Work done | **Mark as shipped** (in the Work top bar menu. One step to confirm) |
| Work is Shipped | **Start a new Work** |
| A note has no Work tied to it | **Attach it to a Work** (quiet link: "keep it as a Seed") |
| A 4th Work would break the live cap | **Rest a Work first** (opens the pick list. New work is blocked in a kind way, not in a mute way) |

## Banned patterns

- A blank first screen. A home grid of boxes with no next step. A
  "Welcome" screen that tells the user to go and look around.
- Icon-only nav with no word labels, in any part of the core loop.
- A pop-up box that opens a pop-up box. Settings shown before the
  first Work exists.
- Guilt tools: streak risk, red badges, "you missed a day" copy.
  We offer direction. We do not shame a user into it.
- The next step hid in a menu, when the table above gives that state
  a main button.

## Tests for a new screen (pass all three, or it is not designed)

1. Hide all but the main button. Does the button still say what this
   screen is for?
2. Count the picks on the screen. Is the count at or under the budget
   for this step? If not, set a default or push a pick to a later day.
3. Come to the screen as a user who was here last on a past day, with
   no recall of that day. Does the screen give the full state back:
   loop place, last act, and the draft next step?
