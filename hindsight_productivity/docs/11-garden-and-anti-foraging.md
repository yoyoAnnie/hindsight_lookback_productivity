# 11 — The Garden, and Designing Against Over-Foraging

## The finding this answers

Interviewees for this project reported the opposite of the usual
"more information + AI = faster creation" story:

> Information overload made them **slower**, not more efficient. Getting
> inspiration is easy; narrowing down is hard. They over-collect —
> saving references they never return to, exploring new ideas instead of
> working the ones they saved — and drift further from the goal they
> started with.

## The diagnosis, in the owner's psychology terms

**Information foraging theory** (Pirolli & Card): people forage for
information the way animals forage for food — moving between *patches*,
following *information scent*, and leaving a patch when its returns feel
weak. The modern failure mode is built into the costs:

- Leaving a patch costs nothing and new patches are infinite, so
  **exploration always beats exploitation** in the moment.
- Saved references have **weak scent** (a bare title, a forgotten folder),
  while a fresh feed has strong scent. So users re-forage instead of
  reading what they already saved.
- Collecting *feels* like progress, so the hoard grows while no action is
  taken — sunk cost dressed as momentum.

Hindsight is therefore designed to do the opposite of a feed: raise the
value of staying in one patch, strengthen the scent of saved material, and
count progress **only** as actions taken on a Work — never as items
collected.

## Anti-foraging rules (product-wide)

1. **No Explore feed. Ever.** No recommendations, no trending, no
   "you might also like", no infinite scroll of other people's ideas.
   Inspiration enters only when the user deliberately uploads it.
2. **Saved-First at intake.** When a user goes to add new material, the
   first thing shown is one unworked saved item — *"Before gathering
   more, this is waiting"* — with the primary button **Work on this
   today**. "Add new anyway" exists, as a quiet link. The friction is at
   the gathering door, never inside the loop.
3. **Collecting earns nothing.** Uploading adds no plant, no progress
   ring, no count on any dashboard. Progress is counted only in Daily
   Directions applied, versions, derivatives, flags resolved, and Works
   Shipped. Hoarding cannot look like progress anywhere in the product.
4. **Strong scent for saved things.** Every Part carries the user's own
   one-line takeaway once it exists; unworked Parts show what waits in
   them ("3 segments, no notes yet"). Eye flags do the same job at Work
   level. A saved patch should smell stronger than the open internet.
5. **Patch-residency is visible.** A Work shows how digested it is —
   Held → In progress (n directions) → Seen → Shipped — so staying has a
   visible payoff and leaving mid-way is a felt choice, not an accident.
6. **WIP limit is an anti-foraging rule,** not housekeeping: 3 active
   Works (see `02`). A fourth waits in the stream until one rests or ships.

## The emotional design target

The interviewed users lean **anxious and easily overexcited** — quick to
gather, quick to worry, hard on themselves when they stall. The product's
answer is to be a **curing, slowing, cute space**, not a productivity
machine:

- Predictable: the same layout and the same next-button position every day.
- Slow: garden motion is deliberately slower than product motion (below).
- Kind mechanics only: **nothing in the product can die, wilt, expire,
  break, or be lost.** No streaks-at-risk, no red, no comparisons, no
  leaderboards. Absence costs nothing.

## The Garden — progress you can see growing

A dedicated quiet corner of the product (its own tab; it never interrupts
the loop). Think LeetCode's contribution grid — except every cell is a
small hand-made thing, not a green square.

### How it works

1. **One plot a day.** Each month is a garden page: a **5 × 6 grid of 30
   plots**. On months with a 31st day, the 31st earns a **small animal**
   in the garden's corner instead of a plot.
2. **Earned by action, not by logging in.** Logging in shows the garden;
   a plot can only be planted after the day's small action is done — a
   Daily Direction applied (Revise or Derive), or an Eye flag resolved.
   This is a deliberate correction to "reward the login": rewarding
   logins would train checking-in, the foraging habit itself. The day-close
   screen's primary button becomes **Draw today's flower**.
3. **Hand-drawn, in under a minute.** The drawing step offers a traced
   petal guide (so drawing skill is never judged) plus free strokes; five
   strokes is plenty. The flower's colour defaults to the colour of the
   Work/space the day's action belonged to — so a month's garden can be
   *read*: mostly teal means a CFA month; mixed means a scattered one.
4. **Nothing dies.** A missed day is empty soil. It stays empty, or the
   user may plant it later — the product never marks it failed, and no
   plant ever wilts. The garden records what happened; it does not grade.
5. **Animals are visitors, not loot.** A small hand-drawn animal also
   appears roughly weekly on a planted plot (drawn the same traced way).
   Animals are not purchasable, randomised, or collectible in a catalogue.
   There is deliberately no catalogue — a catalogue would restart
   collecting inside the reward.
6. **The year view.** Twelve monthly gardens in a 3 × 4 overview —
   ~360 plants after a year of small days. Tapping a plant opens the
   stream entry it came from: the flower *is* the record (Work, date,
   the Takeaway that earned it).

### Why this fits the dilemma

- The anxious forager's pain is that effort feels like sunk cost —
  invisible, endless, unrewarded. The garden makes a small action
  **concrete and permanent** the same day it happens.
- The reward closes the daily loop emotionally (Directive done → flower
  drawn → day over), which is what the journey map's day-close needs
  (`09`, `10`): an ending, not a cliff-hanger into more browsing.
- Because only actions plant, the garden doubles as an honest progress
  metric the user can trust — a full garden cannot be faked by collecting.

### Garden values (see also `05-design-system.md`)

- Plots: rounded-square soil cells, radius 16px, paper background,
  hairline fence border per month page; grid gap 10px.
- Petals: the three mode colours + gold + one soft pink `#E8A0A8`;
  lines hand-drawn style (2px, slightly irregular), never geometric icons.
- Motion: slower than the product — a new plant draws itself over
  ~1200ms, `cubic-bezier(0.22,1,0.36,1)`; idle sway ±1deg at 6s, which
  stops entirely under `prefers-reduced-motion`.
- No numbers on the garden screen: no counts, no percentages, no streak.
  The picture is the metric.

## Scope and phases

- **Phase 1 (MVP):** monthly 5 × 6 grid, traced drawing step, plant at day
  close, colour from the day's Work, tap plant → stream entry, year view
  as a simple 3 × 4 overview. No animals except the 31st-day corner.
- **Phase 2:** weekly visitor animals; planting a missed day
  retroactively; garden export (one image per month) for the archive.
- **Never:** plant shop, rarity, trading, public gardens, leaderboards.
