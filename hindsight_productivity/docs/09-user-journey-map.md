# 09 — User Journey Map

Built with the project's mapping method: foundation first (persona,
scenario, boundaries), then the matrix (5 phase columns × 6 rows), then
construction (validate low-fidelity, design high-fidelity, convert
opportunities into a roadmap with owners and metrics).

**Design principle behind this map:** designing starts from the user's
goal and a workflow that carries them. The interface must lower the user's
cognitive energy — at every point there is a visible next action
(see `10-guided-actions-and-buttons.md`). A user is never left in chaos
or without direction.

---

## Phase 1 — The Foundation

### 1. User persona (primary)

**The cross-format creator-learner.** A creator/student/maker who develops
ideas over days, starting from source material made by others — a podcast
transcript, a textbook chapter, a reference image — and works across text,
notes, and images at the same time. Short on time, high standards for how
things feel, and frustrated that the work lives in five places at once.

- **Interview-grounded (updated 2026-10-16).** The owner's interviews with
  people matching this profile produced the project's central finding:
  **information overload slowed their creation instead of speeding it.**
  Inspiration is easy to get; narrowing down is the hard part. They
  over-collect references they never revisit, keep exploring new ideas
  instead of working the ones they saved, and drift away from their goal.
  In information-foraging terms: saved patches have weak scent, switching
  patches costs nothing, so exploration beats exploitation every day.
  Full diagnosis and the product's counter-design: `11-garden-and-anti-foraging.md`.
- Temperament (from the same interviews): leans **anxious and easily
  overexcited** — quick to gather, quick to worry, hard on themselves
  when they stall. Design response: a curing, slowing, cute space;
  predictable layout; kind mechanics only — nothing in the product can
  be lost (ADR-003).
- The three founding use cases in `03-use-cases.md` are this persona in
  three settings (content, CFA study, artwork) — one persona, three
  templates, not three products. Still to collect: survey data and a
  baseline count of apps touched per finished piece.

### 2. Scenario and primary goal

**Macro-task:** "Take one piece of source material and turn it into my own
finished thing over several days — and be able to see, each day, whether it
got better."

The product's job inside that task: hold the source, take one direction a
day, and show the work's shape on demand. Success for the user is a
**Shipped** Work with its full timeline kept.

### 3. Boundaries

This is a **Future State** map: the ideal flow for a new product. It is not
a map of today's scattered tools. Current-state pain is documented as
friction hypotheses in `01-vision-and-concept.md` and marked for
verification in Phase 3 research, below.

---

## Phase 2 — The Map (5 phases × 6 rows)

Phases: **1 Discover · 2 Start · 3 Work the Loop · 4 Return & Compound ·
5 Ship & Look Back**

### Row 1 — Internal user goals

| Phase | Goal |
| --- | --- |
| 1 Discover | "Find one place for this idea before I lose it." |
| 2 Start | "Get this transcript/script/notes in, without organising anything." |
| 3 Work the Loop | "Make today's small improvement and know it counted." |
| 4 Return & Compound | "Pick up where I left off and see the work getting richer." |
| 5 Ship & Look Back | "Finish it, and keep proof of how it was made." |

### Row 2 — Actions & doing

| Phase | Actions |
| --- | --- |
| 1 | Lands on the page, reads the loop in one screen, clicks **Start a space**. |
| 2 | Uploads one file; waits through splitting; sees the Work in the stream; clicks **Write today's direction**. |
| 3 | Writes Takeaway / Tweak / Question; chooses **Revise** or **Derive**; clicks **See it as a map**. |
| 4 | Returns next day; opens the drafted Question; writes one tweak; re-sees the map; resolves one flag. |
| 5 | Marks the Work **Shipped**; scrolls its timeline; starts or continues another Work; (later) tells a peer it exists. |

### Row 3 — Channels & touchpoints

| Phase | Touchpoints |
| --- | --- |
| 1 | Landing page (hero, stream demo, three modes). |
| 2 | Web app: upload, processing state, stream, Daily Direction form. |
| 3 | Web app: Daily Direction, version view, Eye render, flags. |
| 4 | Web app home (stream with "today" state); optional reminder the user set themselves — never guilt notifications. |
| 5 | Archive/timeline view; export of the timeline. |

### Row 4 — Mindset and emotional curve

Quotes are the thoughts designed for; the curve is the design target to be
checked in usability testing.

| Phase | Mindset | Emotion |
| --- | --- | --- |
| 1 | "Another tool? Show me it is one stream, fast." | Curious, sceptical |
| 2 | "Please don't make me file this." → "Oh, it split it for me." | Hopeful, then relieved |
| 3 | "One tweak is doable." → "The map actually looks like my idea." | Focused, then a spike of clarity |
| 4 | "I remember exactly where this was." | Calm, compounding confidence |
| 5 | "I can see every step that made this." | Pride |

**Curve:** curiosity → small dip at upload (effort risk) → relief at the
first Direction → **spike at the first true Eye render** → steady calm →
pride at Ship. Two valleys are designed against: the post-upload moment
and a weak first map (see Moment of Truth).

### Row 5 — Backstage operations

| Phase | What the system does (targets to test, not guarantees) |
| --- | --- |
| 1 | Landing page must make the loop legible above the fold; motion per `05-design-system.md`. |
| 2 | Intake: virus/type check, split into Parts, thumbnail, Work + stream entry created. Target: a text file is split and visible in under 10 seconds; the processing state names the stage ("Splitting into sections…"), never a bare spinner. |
| 3 | Direction saved to the Work; Revise writes a new Version with the note as its reason; Derive writes a Derivative with provenance links; Eye re-render queued on either. Target: render under 3 seconds for MVP-sized Works. |
| 4 | Flags recomputed on the new render; Flag → tomorrow's Question draft is generated at day close, labelled a draft. |
| 5 | Work status set to Shipped; timeline frozen as the archive record; export generated on request only. |

### Row 6 — Experience opportunities (from the friction in Rows 2–5)

Each opportunity is converted into work in Phase 3, with an owner and a
metric — never left as a wish.

| # | Opportunity | Owner | Metric it must move |
| --- | --- | --- | --- |
| O1 | Post-upload direction: the instant a file is Held, one primary button — **Write today's direction** — replaces any library view | Design | % of first uploads that reach a first Direction in the same session |
| O2 | First Eye render quality: the starter map is built from the split + first Direction only, so it is personal, not generic | Eng + Design | % of first renders the user rates "looks like my idea" in testing |
| O3 | One-tweak constraint enforced kindly in the form (extra tweaks queue as drafts, not errors) | Product | Median time to complete a Daily Direction (target: under 5 minutes) |
| O4 | Flag → Question one-click conversion at day close | Eng | % of Eye flags converted or consciously dismissed |
| O5 | Resume card on return: last Takeaway, last Tweak, drafted Question, one button **Continue this Work** | Design | Day-7 return rate of users with ≥1 Shipped or active Work |
| O6 | Respect the WIP limit in the UI: a 4th active Work asks which one rests | Product | Works completed per user vs. Works abandoned mid-loop |
| O7 | The Garden: a hand-drawn plant earned by each day's completed action, in a 5 × 6 monthly grid — progress as a picture, never a number (docs/11) | Design + Eng | % of active days that end with a planted plot; Day-30 return rate |
| O8 | Saved-First intake: adding new material first surfaces one unworked saved item, with **Work on this today** as the primary button (docs/11) | Design | Ratio of new uploads to saved items worked, per user per week (target: falls over time) |

---

## The Moment of Truth

**Primary Moment of Truth: the 60 seconds after the first upload.**
The user has handed the product a real file and has no direction yet. If
they see a library, settings, or an empty canvas, the product has recreated
the chaos it promised to remove, and drop-off here is fatal. The design
answer is O1 + the button rules in `10-guided-actions-and-buttons.md`:
one Work, one next button, nothing else competing.

**Second Moment of Truth: the first Eye render.** If the map does not
mirror the user's own thinking more clearly than the source file did,
trust in the loop collapses and Return (Phase 4) never happens. This is
why the flags must be right before they are clever, and why the MVP tests
O2 by hand before any automation is trusted.

---

## Phase 3 — Construction

### Step 1 — Synthesis and wireframing (low-fidelity)

- Plot interview/survey findings onto this grid with sticky notes
  (FigJam/Mural-style) before touching screens; keep the grid cells in
  this file as the source of truth and update them from findings.
- Unsequenced observations go in the relevant cell; disputed steps go to
  a verification backlog instead of stalling the map.

### Step 2 — High-fidelity design

- Move the agreed timeline into the design tool; draw the emotional curve
  as a line over the five phases and mark both Moments of Truth on the
  screens themselves (a note on the post-upload screen, a note on the
  first-render screen).
- Every screen in the flow is checked against
  `10-guided-actions-and-buttons.md` before it is considered designed.

### Step 3 — Roadmap conversion

- O1–O8 are already in `06-mvp-scope-and-roadmap.md` order of importance:
  O1 and O2 are Phase-1 exit criteria, O3–O6 are Phase-1/2 work, O7 (the
  Garden) ships in its basic Phase-1 form per docs/11, O8 with intake.
- When an opportunity ships, record its metric's before/after in the
  session log that shipped it. An opportunity without a measured result
  is not done.
