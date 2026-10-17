# 02 - Main Workspace Workflow: The Loop

This is the core doc of the project. All other docs serve this loop.

## The loop in one sentence

I **hold** a source file in the Hand. I **direct** it each day with a
note in the Brain. I **see** it in a clear form through the Eye. What
the Eye shows then sets my next day's note. One Work, one loop.

```
  1. HOLD (Hand) --> 2. DIRECT (Brain) --> 3. SEE (Eye)
        ^                                        |
        |                                        v
        ------- 4. RETURN: gaps in the map set --- 
                the next day's question
```

## The one object: a Work

- A **Work** starts when the Hand gets a thing: a YouTube script, a
  podcast transcript, a CFA chapter file, a photo of a sketch.
- A Work has one timeline. I call the timeline **the stream**. Each
  version, note, new item, and map is a line on that timeline, in
  date order.
- The Brain and the Eye hold no copies. They read the Work and act on it.

## Step 1 - HOLD (Hand)

**My act:** I upload a file, I pull a file in, or I shoot a photo of
work on paper.

**The Hand does four things, and no more.** Intake must stay fast. I
must not have to sort a thing at this step.

1. It makes the Work. It sets a title, the source, and the date.
2. It splits the file into parts. A transcript splits by segment. A
   document splits by section. An image stays one image, with a notes
   area next to it. Each note and each map node must be able to point
   at one part.
3. It puts the Work in the stream. State: **Held**.
4. It picks a first Eye view by type. Text gets a mind map. A product
   gets a prototype. An image gets a layout view. Study files get a
   concept map. I can change the pick.

## Step 2 - DIRECT (Brain)

**My act:** a **Daily Direction**. This is a note tied to one Work.
It is never a loose note. It has three fields, and only three. The
limit is the point. It forces me to pick what counts most today.

1. **Takeaway** - what stuck today, in my own words.
2. **Tweak** - one change for today. One, not a list.
3. **Question** - what is still open. The Eye often drafts this field.
   See Step 4.

I can add other notes to the same Work: journal lines, feedback from
people. Those notes sit on the same timeline. But only a Daily
Direction acts on the file.

### The two ways my note changes a file (Brain -> Hand)

A Daily Direction acts on the file in one of two ways. I pick the way.
The screen shows both picks in plain words.

**Type A - REVISE the file**

- I edit, cut, move, or mark up the source.
- The result is a **new version** of the file: v2, v3, and so on.
- The app never writes over the old file. My note that made the change
  is saved as the reason for the version. So the timeline shows why
  each version exists.
- Case: "Tighten the podcast opening" acts on my script. The result
  is script v2.

**Type B - DERIVE: make a new thing from the file**

- The source file does not change. The app makes a new item from one
  part of it.
- New items can be: a takeaway card, an outline, a title list, a short
  script, flash cards, test questions, a color study, a bank of quotes.
- Each new item keeps a **link back to its source**: the Work, the
  part, and my note that asked for it.
- Case: "Pull today's takeaway" acts on a transcript. The result is a
  takeaway card tied to that one segment.

State after a direction acts: **Directed**.

## Step 3 - SEE (Eye)

**My act:** I call the Eye on a Work. I can do this at any time. The
Eye is a check, not a last step.

**What the Eye draws** - the Work plus all my Brain notes up to now:

| Work type | Eye view |
| --- | --- |
| Video, podcast, or writing idea | Mind map of the claim set: claims, cases, stories |
| Product or site idea | Low-detail prototype from my notes |
| Artwork | Layout view: the work next to its source images and past versions |
| Study files (CFA and the like) | Concept map: topics, rules, and the links between them |

**The rich check.** Each time it draws, the Eye flags three things, in
plain words:

- **Thin** - a part said once and never built up. One node, no case,
  no note.
- **Orphan** - a note tied to no part of the file.
- **Conflict** - a new tweak that clashes with an old direction.

The flags answer my real question: is this idea rich? Is it good to
look at? The flags make the answer clear. I do not have to guess.

State: **Seen**.

## Step 4 - RETURN

- Each flag can draft the **Question** field of my next day's Daily
  Direction. I can edit it or swap it. I never start a day with a
  blank box.
- The loop runs again. My next note does a Revise or a Derive. The Eye
  draws the map again on its own when a new version or a new item lands.
- A Work leaves the daily loop when I mark it **Shipped**. The full
  timeline stays saved. That saved past is the hindsight in the name.

## Rules that keep my loop light

1. **No loose notes.** A note must tie to a Work. If it has no Work, it
   starts as a **Seed**: a small Work of its own. It can get a file later.
2. **One tweak per day per Work.** The three-field form holds this rule.
3. **Cap on live work.** At most **3 Works** run in my daily loop at
   once. The rest sit in the stream. The app sends me no guilt notes
   for them.
4. **No hand work for links or maps.** Versions, new items, back
   links, and Eye updates are side effects of the loop. I do not file,
   link, or redraw a thing by hand.
5. **Forms, not blank pages.** Each of my three main use cases ships
   with a set form: how intake splits the file, what the Daily
   Direction asks, and which Eye view it uses. See `03-use-cases.md`.
6. **Two-minute close.** My day ends with three things on screen:
   today's Takeaway, today's Tweak, and the draft Question for the
   next day. Then I draw today's flower in the Garden. See `11`.
   The app asks me for nothing more.
7. **New intake has a gate. Work in the loop has none.** When I add
   new stuff, the app first shows me one saved item that has no work
   on it yet. Saved-First. See `11`. In the loop, there is no such gate.
8. **A save is not progress.** My progress counts acts in the loop
   only: directions used, versions made, new items made, flags
   cleared, and Works shipped. The Garden counts the same way.

## States

`Seed -> Held -> Directed -> Seen -> (new version or new item -> Seen ...) -> Shipped`

Each state change adds a line to the stream. Each line has a date. If
I wrote the words, the line keeps my words.
