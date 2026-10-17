# 11 - The Garden, and My Fight Against Over-Foraging

## The find this doc answers

Users I talked to told me a story that cuts the other way from the
common claim. The claim says: more facts plus AI tools make work
fast. Their work got slow. Mine did too.

New ideas are easy to get. It is hard to cut the list down. My users
collect too much. They save links and files they never open again.
They look for new ideas, and they do not work on the saves. Day by
day, they drift from the goal they set at the start.

## The cause, in plain psychology terms

**Information foraging theory** (Pirolli and Card): people hunt for
facts the way an animal hunts for food. They move from patch to
patch. They follow the scent of a fact. They leave a patch when the
gains feel weak.

The web breaks this hunt in three ways:

- It costs nothing to leave a patch. And new patches have no end. So
  in the short run, a jump always beats a stay.
- Saved files have **weak scent**: a bare title, a lost folder. A
  fresh feed has strong scent. So my users hunt fresh facts, and
  they do not read their own saves.
- A save *feels* like work done. So the pile grows, and no act gets
  taken. Cost with no gain, dressed as speed.

I built Hindsight to do the flip side of a feed. I make a stay in
one patch worth more. I give saved work a strong scent. And I count
progress as **acts on a Work only**, never as saves.

## My rules against over-foraging (for the whole product)

1. **No feed for new ideas. At all.** No picks for you. No trends.
   No "you may like this too." No scroll with no end, of work by
   other people. New facts come in when you upload them, on purpose.
2. **Saved-First at intake.** When you add new stuff, the first
   thing on screen is one saved item with no work on it yet. My text
   is: "Before you gather more, this one waits." The main button is
   **Work on this today**. A quiet link says "Add new anyway." The
   hard part sits at my intake door. In the loop, there is no block.
3. **A save earns nothing.** An upload adds no plant, no progress
   ring, and no count on any board. My progress counts Daily
   Directions used, versions, new items, flags cleared, and Works
   Shipped. A big pile can not look like progress in any part of my app.
4. **Strong scent for saved work.** Each Part of a file shows your
   own one-line takeaway, once it exists. A Part with no work shows
   what waits in it: "3 segments, no notes yet." Eye flags do the
   same job at the Work level. Your saved patch must pull more than
   the open web.
5. **Work in a patch is clear to see.** A Work shows how far you
   worked it: Held, then In progress (with a count of directions),
   then Seen, then Shipped. A stay has a clear gain. A leave mid-way
   is a choice you can feel, not a slip.
6. **My cap on live Works is a rule against over-foraging.** It is
   not a tidy-up rule. The cap is 3. See `02`. A 4th Work waits in
   the stream till one rests or ships.

## The mood my design must hold

Users in my talks lean tense and quick to get worked up. They gather
fast. They worry fast. They blame their own stall. So I made my app
a calm space that slows them down, with a soft and cute feel. Not a
work-rate machine.

- Steps do not change: same layout, same next button in the same
  spot, each day.
- Slow: Garden motion is set slow on purpose. See my values below.
- Kind rules only: **nothing in my app can die, wilt, run out,
  break, or be lost.** No streak at risk. No red marks. No ranks. No
  boards that rank users next to each other. A missed day costs you
  nothing.

## The Garden - progress you can see grow

The Garden is a quiet part of my app. It has its own tab. It never
cuts into the loop. Think of the LeetCode grid of green squares, but
each cell here is a small thing you made by hand.

### How it works

1. **One plot per day.** Each month is one garden page: a **5 x 6
   grid, 30 plots**. A month with 31 days puts the 31st day in a
   corner as a **small animal**, not a plot.
2. **You earn a plant by an act, not by a login.** A login shows you
   the Garden. But you can draw a plot only when your day's small
   act is done: you used a Daily Direction (Revise or Derive), or
   you cleared an Eye flag. I made this call on purpose, and it
   breaks from my first sketch of the idea. My first sketch paid you
   for a login. That trains the check-in habit, which is the
   foraging habit in a new coat. So I pay for the act. Your day
   close screen's main button is: **Draw today's flower**.
3. **Drawn by hand, in under a minute.** My draw step gives you a
   trace guide for the petals, so skill is not judged. Five free
   lines are fine on top of the guide. I set the flower's color from
   the Work your day's act sat on. So you can read a month of
   flowers: all teal means a CFA month. Mixed colors mean a split
   month.
4. **Nothing dies.** A missed day is bare soil. It stays bare, or
   you can plant it on a later day. I never mark it as a fail. And
   no plant wilts, at any time.
5. **Animals visit. They are not loot.** A small hand-drawn animal
   shows up about once a week, on a plot with a plant. You draw it
   the same trace way. Animals cost no points. You do not draw them
   at random from a prize pool. And I made no list of all animals
   to get. A list like that would start the collecting habit back
   up, inside my reward itself.
6. **The year view.** Twelve month gardens sit in a 3 x 4 grid.
   That is about 360 plants for a year of small days. A tap on a
   plant opens the stream line it came from: the Work, the date,
   and the Takeaway that earned it. The flower is the record.

### Why this fits my hard truth

- Your core pain is cost with no sight of gain. Work feels sunk.
  The Garden makes one small act **real and kept**, on the day it
  happens.
- The reward ends your day. Direction done, flower drawn, day shut.
  That is what my day close in `09` and `10` needs: an end, not a
  hook that pulls you into more web time.
- A plant needs an act. So the Garden is a true count of your
  progress, in picture form. You can not fake a full garden with saves.

### Garden values (see also `05`)

- Plots: round-corner soil squares, radius 16px, on paper. A thin
  fence line wraps each month page. Grid gap 10px.
- Petals: my three mode colors, plus gold, plus one soft pink
  `#E8A0A8`. Lines look hand drawn: 2px, a bit rough. No clean
  shape icons.
- Motion: slow, by my set rule. A new plant draws in about 1200ms,
  with ease `cubic-bezier(0.22,1,0.36,1)`. Idle sway is 1 degree
  each way, 6 seconds per cycle. It stops in full if you set
  reduced motion in your system.
- No numbers on the Garden screen. No counts, no percent, no
  streak. The picture is the count.

## Scope and phases, as I set them

- **Phase 1 (MVP):** the month grid of 5 x 6. The trace draw step.
  A plant at day close. Color from your day's Work. Tap a plant to
  open its stream line. The year view as a plain 3 x 4 grid.
  Animals only in the 31st-day corner.
- **Phase 2:** a visitor animal each week. Plant a missed day at a
  later date. Export one image per month, for your archive.
- **Never, in my plan:** a plant shop. Rare plants. Trades. Public
  gardens. Rank boards.
