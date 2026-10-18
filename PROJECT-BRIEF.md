# Hindsight — Project Brief: Motivation and Rationale

This document explains my project: why it exists, what I learned
from users, and the reason behind each core choice. Read it to
understand the project before any work starts.

## 1. What I am building

Hindsight is a scrapbook journal for ideas. I keep my ideas in one
stream and work on them a little each day. The website comes first.
A phone app comes later.

The core unit is a **Work**: one piece of source material plus
everything I do to it over days — my notes, its new versions, the
things I make from it, and the pictures that show its shape. All of
it stays on one timeline, in date order.

## 2. The problem that made me build it

My ideas sat in many apps at once. A file was in a drive. Feedback
was in a chat. A daily note was in a notes app. A sketch was on
paper, shot with a phone and then lost. A goal sat in my head,
never drawn or built.

The pain is not a lack of tools. The pain is the switch between
tools. I lost ideas between apps. The people I talked to told me
the same.

## 3. What users told me

I talked to users who build ideas over days from source material
made by other people: creators, students, artists. One finding
sits at the core of this product:

**More facts made their work slower, not faster.**

New ideas are easy to get. AI tools made that part even easier.
But the work got slower. The reason: it is hard to cut the list
down. Users save links and files and never open them. They keep
looking for new ideas. They do not work on the saved ones. Each
new save pulls them away from the goal they set at the start.

Users also lean tense and quick to get worked up. They gather
fast. They worry fast. They blame their own stall. Any tool I
build for them must calm them down, not speed them up.

## 4. Why this happens — the psychology under it

I study psychology. This pattern has a name: **information
foraging**. People hunt for facts the way an animal hunts for
food. They move from patch to patch. They follow the scent of a
fact. They leave a patch when the gains feel weak.

The web breaks this hunt in three ways:

- It costs nothing to leave a patch, and new patches have no end.
  So in the short run, a jump always beats a stay.
- Saved files have weak scent: a bare title, a lost folder. A
  fresh feed has strong scent. So users hunt fresh facts and do
  not read their own saves.
- A save feels like work done. So the pile grows and no act gets
  taken. It is cost with no gain, dressed as speed.

My product is built as the flip side of a feed. It makes staying
in one patch worth more. It gives saved work a strong scent. It
counts progress as acts on a Work only — never as saves.

## 5. The core idea: one stream, three actions on one Work

I do not sort work by folder. I sort it by what I do with it.
Three modes act on the same Work. They are not three places and
they hold no copies of each other.

- **Hand (Hold)** — the source itself: files, scripts,
  transcripts, podcast notes, reports, images.
- **Brain (Direct)** — my daily notes on that source: what stuck,
  what people said, and the one change I want today.
- **Eye (See)** — the same work drawn in a clear form, so I can
  judge it: is it rich, is it clear, is it good to look at?

The name is the point. All work stays on one timeline, so a look
back is of use. That look back is hindsight.

## 6. The loop, and the reason for each part

The daily loop is: **Hold → Direct → See → Return.**

**Hold.** The Hand takes in a file, a transcript, or a photo of
work on paper. It splits the file into parts — a transcript by
segment, a document by section. Reason: intake must be instant,
with no sorting work for the user, and every later note and map
must be able to point at one exact part. If intake feels like
filing, users quit at the door.

**Direct.** Each day I write one **Daily Direction** on a Work.
It has three fields, and only three:

1. **Takeaway** — what stuck today, in my own words.
2. **Tweak** — one change for today. One, not a list.
3. **Question** — what is still open.

The cap is the point. Three fields and one tweak force a choice
about what counts most today. A long form or a blank page gives
the user their overload back. A note that acts must be tied to a
Work. There are no loose notes, because loose notes are how the
scatter starts. A note with no Work starts as a **Seed**, a small
Work of its own.

**The note changes the file in one of two ways.** I pick the way:

- **Revise** — I edit, cut, move, or mark up the source. The
  result is a new version. The old version is never written over,
  and my note is saved as the reason the version exists. Reason:
  the timeline must show why each version happened, or the look
  back is worth nothing.
- **Derive** — the source stays as it is, and a new item is made
  from one part of it: a takeaway card, an outline, flash cards,
  test questions, a draft. Each new item keeps a link back to its
  source part and to the note that asked for it. Reason: nothing
  in the stream may float free of its source, or trust in the
  stream dies.

**See.** I call the Eye on a Work at any time. It draws the Work
plus all my notes so far — a mind map for a content idea, a
concept map for study, a layout view for art, a first-shape
prototype for a product. Then it flags three things, in plain
words:

- **Thin** — a part said once and never built up.
- **Orphan** — a note tied to no part of the file.
- **Conflict** — a new tweak that clashes with an old direction.

Reason: "is this idea rich?" is the question users actually ask,
and they used to answer it by feel. The three flags turn that
feel into three checks a user can act on. The Eye is a test, not
a decoration.

**Return.** Each flag can draft the Question field of the next
day's Daily Direction. I can edit it or swap it. Reason: no one
should start a day at a blank box. The loop feeds itself, so the
only daily decision left is the one tweak.

**Limits that hold the loop together:**

- At most **3 Works** run in the daily loop at once. Reason: the
  cap is a rule against over-foraging, not a tidy-up rule. More
  live Works means more patches to jump between.
- A Work leaves the daily loop when I mark it **Shipped**. The
  full timeline stays saved. That saved past is the product's
  memory.
- Progress counts acts only: directions used, versions made,
  items derived, flags cleared, Works shipped. A save never
  counts. Reason: if saving counted, the app would pay users for
  the exact habit it exists to break.

## 7. Rules against over-foraging

These rules come straight from the finding in section 3. They
are product law, not preferences:

1. **No feed for new ideas.** No recommendations, no trending, no
   endless scroll of other people's work. New material enters
   only when the user uploads it, on purpose. A discovery surface
   would rebuild the problem inside the product.
2. **Saved-First at intake.** When a user adds new material, the
   app first shows one saved item that has no work on it yet, and
   offers it as today's work. Adding new stays possible, but it
   is one step behind working on what is already saved. Reason:
   put the small friction at the gathering door, and no friction
   inside the loop.
3. **Saved work gets strong scent.** Each part of a file shows my
   own one-line takeaway once it exists. A part with no work
   shows what waits in it. Reason: a saved patch must pull harder
   than the open web.
4. **Residency is visible.** A Work shows how far it has been
   worked: Held, then in progress, then Seen, then Shipped.
   Reason: a stay must have a visible gain, or leaving feels free.

## 8. The Garden — progress you can see grow

The core pain is sunk cost with no sight of gain: work goes in,
nothing shows. The Garden is my answer.

- One plot per day, in a monthly grid of 5 by 6 — about 30 plots
  a month, about 360 plants in a year of small days. A month with
  31 days puts the extra day in a corner as a small animal.
- A plant is earned by a **completed act** — a Daily Direction
  used, or an Eye flag cleared. A login alone shows the Garden
  but plants nothing. Reason: paying for a login trains the
  check-in habit, which is the foraging habit in a new coat. The
  reward must sit on the act.
- The plant is drawn by hand, fast, with a trace guide. Reason:
  the reward is a small thing the user made, not a badge the
  system handed out, and drawing skill must never be judged.
- The flower's color comes from the Work the day's act sat on.
  Reason: a month of flowers can then be read — one color means a
  month on one subject.
- **Nothing dies.** A missed day is bare soil. It can be planted
  later. No plant wilts. There are no streak counts, no numbers,
  no ranks on the Garden screen. Reason: my users are tense, and
  a loss mechanic would make the calm space a threat. A missed
  day must cost nothing.
- There is no catalogue of plants or animals to collect, no
  shop, no rare items, no public gardens. Reason: a collection
  list would restart the collecting habit inside the reward
  itself.
- A tap on a plant opens the stream entry it came from. Reason:
  the flower is a record of a real act, not a decoration.

The Garden also ends the day. Direction done, flower drawn, day
shut. It is a close, not a hook into more screen time.

## 9. Guided steps — why the user is never left lost

Design starts from the user's goal and from a workflow that
carries them. The aim is to cut the user's mental load, so their
mind stays on the idea and not on the tool.

- **One main button per state.** Each screen ends with exactly
  one clear next action, named with a verb and an object. Reason:
  a row of equal buttons hands the decision cost back to the
  user.
- **The app carries the memory.** The next screen shows the last
  Takeaway, the last Tweak, and the drafted Question. Reason: a
  returning user should never pay the cost of rebuilding context.
- **Loop position is always visible**: Hold, Direct, See, Ship.
  Reason: "where am I" must cost no thought.
- **A daily decision budget of three**: which Work, today's one
  Tweak, and Revise or Derive. Everything else is set by the app,
  queued, or pushed to a later day.
- **No guilt mechanics.** No streak warnings, no red badges, no
  "you missed a day". Reason: guilt is a pressure tool, and my
  users already blame themselves. Direction, not shame.
- An empty state is a step, not a hole: one plain line and one
  button. A blank canvas is the overload problem in a new shape.

## 10. The two moments the whole product stands on

From my journey map, two points decide if the loop lives:

1. **The 60 seconds after the first upload.** The user gave the
   app a real file and has no direction yet. If they meet a file
   list, a settings page, or a blank screen, the app rebuilt the
   mess it promised to fix, and they leave. The fix: one Work on
   screen, one button — write today's direction.
2. **The first Eye drawing.** If the map does not show the user's
   own thought in a clearer form than the source file, trust in
   the loop dies, and the user never comes back for day two. The
   fix: flags must be right before they are smart, and the first
   map is built from the user's file and first note only.

## 11. The three uses I designed for first

One user, three forms. The loop does not change. Only the intake
split, the Direction prompts, and the Eye view change.

- **Content (YouTube, podcast, writing).** Upload a script or a
  transcript. Daily notes revise the script or derive titles,
  notes, and cards from it. The Eye draws the claim map. "Rich
  enough" test: each main claim has a case or a story.
- **Study (CFA).** Upload a chapter or notes. Daily notes derive
  flash cards and test questions, or revise the notes after a
  test. The Eye draws the concept map. "Rich enough" test: a
  topic has notes, test work, and one fix. A read alone never
  counts.
- **Art.** Photograph each version of a piece, with its source
  images in the same Work. Daily notes revise (next version) or
  derive (a color study, a crop test). The Eye shows the version
  next to its sources. "Rich enough" test is the flag set: no
  saved source unused, no named part missing from all versions.

## 12. What this product is not, and why

- **Not a general notes app, a file drive, or a task board.**
  Those tools store. This one runs a loop.
- **Not social in the first version.** Work is private by
  default. Sharing adds other people's scent to a space built to
  lower it.
- **Not an AI that thinks for the user.** The Brain is the user's
  own mind. The machine can split files, link parts, draw maps,
  flag gaps, and draft a Question. It does not pick the daily
  change, and a system draft is always marked as a draft. Reason:
  the judgment is the user's skill. A tool that takes the
  judgment takes the growth with it.
- **No folders inside folders, no tag system** in the first
  version. Sorting systems are where saved things go to be
  forgotten.

## 13. Privacy

The user's files, notes, and maps are seen by that user only.
Every derived item shows what it was made from. Deleting a Work
deletes all of it. User work is not used to train models. My own
project idea is private in the same way: it is documented for me,
and it is not shared with or pitched to other users.

## 14. Scope logic

- **Web first, one user, private.** The loop is the value. It
  must be proven before any app, team, or sharing work.
- **Phase 1 runs the full loop end to end for one use case**
  (content), with the other two as set forms. Reason: a thin full
  loop teaches more than three half loops.
- **The Garden ships in basic form in Phase 1**, because the
  day-close ritual is part of the loop, not a later extra.
- **Later phases add depth, not new surfaces**: richer Eye views,
  then a phone app for fast intake and the daily note, then a
  decision — based on real use — on whether teamwork belongs in
  this product at all.

## 15. Open questions I hold

- Will users keep a daily habit if the loop takes more than five
  minutes a day? The three fields, the one tweak, and the drafted
  Question are my bets against that risk. They are bets until
  real use tests them.
- Rule-based flags can only say part of "is it rich". I test the
  flags against my own judgment, case by case, before I trust
  them.
- Intake split quality makes or breaks the source links. If the
  split is wrong, every note and flag built on it feels wrong.

— Annie
