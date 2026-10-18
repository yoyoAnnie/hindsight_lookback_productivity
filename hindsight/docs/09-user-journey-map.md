# 09 - User Journey Map

How I built this map: I set the base first (the user, the main task,
the bounds). Then I built the grid: 5 phase columns and 6 rows. Then
I did the work in three steps: group what I know, draw the full
design, and turn the weak points into road map work with an owner
and a number to check.

The rule under this map: I design from the user's goal and from a
workflow that walks the user through the task. My screens must cut
the user's mental load. At each point, one next step is clear. See
`10-guided-actions-and-buttons.md`. I never leave a user lost.

---

## Step 1 - The base

### 1. The user I design for

**The creator-learner who works across forms.** This user builds
ideas over days. They start from source work made by other people:
a podcast transcript, a book chapter, a source image. They work in
text, notes, and images at the same time. They have little time.
They have high taste. And their work sits in five places at once.
I know this user well. I am this user.

**What my talks with users showed (set 2026-10-16).** I talked to
users who fit this type. One find sits at the core of my product:

**More facts made their work slow, not fast.** New ideas are easy
to get. It is hard to cut the list down. My users save links and
files and never open them. They keep on with new ideas, and they do
not work on the saves. Each day of this pulls them away from the goal.

In my field, psychology, this is information foraging. Saved files
have a weak pull. New feeds have a strong pull. It costs nothing to
jump. So users jump and do not stay. My full write-up and my fix are
in `11-garden-and-anti-foraging.md`.

**The mood of my user.** Users in my talks lean tense and quick to
get worked up. They save fast. They worry fast. They blame their own
stall. My design must answer that: a calm space that slows the user
down, with a soft and cute feel. The steps stay the same each day.
Kind rules only. A user can lose nothing in this app. See ADR-003 in
`decisions/`.

My three use cases in `03` are this one user in three places:
content work, CFA study, and art. One user, three forms. Not three
products. Still to get: survey data, and a count of apps touched
per finished piece of work.

### 2. The scene and the main goal

**Main task, in the user's words:** "Take one piece of source work
and turn it into my own finished thing over days. And each day, see
if it got better."

My app's job in that task: hold the source, take one direction a
day, and show the shape of the work when the user asks. A win for
the user is a **Shipped** Work with its full timeline saved.

### 3. The bounds I set

This map is a **Future State** map. It shows the right flow for my
new product. It is not a map of the messy tools my users have now.
The pain of the tools they have now is in `01`, as a set of claims
for me to test.

---

## Step 2 - The map (5 phases x 6 rows)

My 5 phases: **1 Find · 2 Start · 3 Work the Loop · 4 Come Back and
Build Up · 5 Ship and Look Back**

### Row 1 - What my user wants at each phase

| Phase | Goal in the user's words |
| --- | --- |
| 1 Find | "Give me one place for this idea before I lose it." |
| 2 Start | "Get this file in. Do not make me sort it." |
| 3 Work the Loop | "Make one small gain today, and know it counted." |
| 4 Come Back | "Pick up where I left off. See the work get rich." |
| 5 Ship | "End it. And keep proof of how I made it." |

### Row 2 - Acts my user takes

| Phase | Acts |
| --- | --- |
| 1 | Lands on my page. Reads the loop on one screen. Clicks **Start a space**. |
| 2 | Uploads one file. Waits for the split. Sees the Work in the stream. Clicks **Write today's direction**. |
| 3 | Writes Takeaway, Tweak, Question. Picks **Revise** or **Derive**. Clicks **See it as a map**. |
| 4 | Comes back the next day. Opens the draft Question. Writes one tweak. Sees the map again. Clears one flag. |
| 5 | Marks the Work **Shipped**. Scrolls its timeline. Starts a new Work or goes on with one. Tells a friend the app exists (a later step). |

### Row 3 - Touch points

| Phase | Where the user meets my app |
| --- | --- |
| 1 | My landing page: hero, stream demo, three modes. |
| 2 | Web app: upload, load state, the stream, the Daily Direction form. |
| 3 | Web app: Daily Direction, version view, Eye draw, flags. |
| 4 | Web app home: the stream with a "today" state. A ping is fine if the user set it. No guilt pings, ever. |
| 5 | The archive: timeline view, and an export of the timeline. |

### Row 4 - Mind set and the feel curve

The quotes are the thoughts I design for. The curve is my target.
I test it with real users later.

| Phase | Thoughts in the user's head | Feel |
| --- | --- | --- |
| 1 | "One more tool? Show me the one stream, fast." | Keen, but not sold |
| 2 | "Do not make me file this." Then: "It split the file for me." | Hope, then relief |
| 3 | "One tweak, I can do that." Then: "The map looks like my idea." | Focus, then a spike of clear sight |
| 4 | "I know just where this was." | Calm. Trust builds |
| 5 | "I can see each step that made this." | Pride |

**My curve in words:** keen at the start. A dip at upload, when
work may feel hard. Relief at the first Direction. A spike at the
first true Eye draw. Calm on each return. Pride at Ship. Two dips
get my design work: the point right after upload, and a weak first
map. See the hard points, next.

### Row 5 - Work my system does (targets I test, not hard claims)

| Phase | System work |
| --- | --- |
| 1 | My landing page must make the loop clear in the top screen. Motion rules are in `05`. |
| 2 | Intake: file type check, split into Parts, thumb image, Work made, stream line made. My target: a text file splits and shows in under 10 seconds. The load state names the step: "Splitting into sections..." It is never a bare spin wheel. |
| 3 | The app saves the Direction to the Work. Revise writes a new Version, and the note is saved as the reason. Derive writes a new item with source links. Eye draw goes in a queue on each save. My target: a draw in under 3 seconds for a Work of MVP size. |
| 4 | Flags run again on the new draw. At day close, Flag-to-Question drafts the next day's Question. It is marked as a draft. |
| 5 | The Work state is set to Shipped. The timeline is locked as the saved record. Export is made when the user asks, and not before. |

### Row 6 - Weak points, and the work I turn them into

Each weak point gets an owner and a number for me to check. It does
not stay a wish.

| # | Work to do | Owner | Number it must move |
| --- | --- | --- | --- |
| O1 | Right after upload, one main button shows: **Write today's direction**. It takes the place of a file list view | Design (me) | % of first uploads that reach a first Direction in the same session |
| O2 | First Eye draw quality: I build the first map from the split plus the first Direction only, so the map is the user's, not a stock map | Build + Design | % of first draws the user rates "looks like my idea" in my tests |
| O3 | Hold the one-tweak cap with a soft touch in the form. Extra tweaks queue as drafts. They are not an error | Product (me) | Mean time to do a Daily Direction. My target: under 5 minutes |
| O4 | One click turns a flag into the next day's Question, at day close | Build | % of Eye flags turned into a Question, or shut with a clear tap |
| O5 | A return card on the home screen: last Takeaway, last Tweak, draft Question, one button: **Continue this Work** | Design (me) | Day-7 return rate for users with one or more live or Shipped Works |
| O6 | Hold the cap on live Works in the UI. A 4th live Work asks the user which one rests | Product (me) | Works done per user, next to Works left mid-loop per user |
| O7 | The Garden: one hand-drawn plant per day of real action, on a 5 x 6 grid per month. Progress as a picture, not a number. See `11` | Design + Build | % of live days that end with a plant drawn. Day-30 return rate |
| O8 | Saved-First intake: when a user adds new stuff, I show one saved item with no work on it first. Main button: **Work on this today**. See `11` | Design (me) | New uploads per week, next to saved items worked per week, per user. My target: the ratio falls over time |

---

## The hard points (make or break for me)

**Hard point 1: the 60 seconds after the first upload.** The user
gave my app a real file. They have no direction yet. If they see a
file list, a settings page, or a blank screen, I just built the same
mess I said I would fix. Users drop here, and few come back. My fix
is O1, plus the button rules in `10`: one Work, one next button, no
other thing in the way.

**Hard point 2: the first Eye draw.** If my map does not show the
user's own thought in a clearer form than the source file, trust in
my loop dies. Phase 4 (Come Back) then never starts. So my flags
must be right before they are smart. And I test O2 by hand before I
trust any auto rule.

---

## Step 3 - How I turn the map into build work

### Part 1 - Group what I know (low detail)

- I put talk and survey finds on this grid with sticky notes first.
  I use a board tool like FigJam or Mural. The cells in this file
  stay my true source. I update them from the finds.
- Facts with no clear phase go in the cell that fits best. Points I
  fight about go on a check list. My map does not stop for a fight.

### Part 2 - Draw the full design (high detail)

- I move the set timeline into my design tool. I draw the feel curve
  as a line over the five phases. I mark both hard points on the
  screens that hold them: a note on the post-upload screen, a note
  on the first draw screen.
- Each screen in my flow must pass the checks in `10` before I call
  it designed.

### Part 3 - Turn the map into a road map

- O1 to O8 sit in `06` in rank order. O1 and O2 are gates for
  Phase 1: Phase 1 does not pass if they fail. O3 to O6 are Phase 1
  and 2 work. O7 (the Garden) ships in basic form in Phase 1, per
  `11`. O8 ships with intake.
- When a piece of work ships, I log its number, before and after, in
  the session log that shipped it. Work with no number check is not
  done, in my book.
