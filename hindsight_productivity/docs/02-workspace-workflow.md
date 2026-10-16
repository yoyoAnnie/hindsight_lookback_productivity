# 02 — Principal Workspace Workflow: The Loop

This is the core document of the project. Everything else serves this loop.

## The one-sentence version

A user **holds** source material in the Hand, **directs** it daily with
notes in the Brain, **sees** it concretely through the Eye — and what the
Eye shows becomes the next day's direction. One Work, going around one loop.

```
        ┌──────────────────────────────────────────┐
        │                                          │
        ▼                                          │
  1. HOLD (Hand) ──► 2. DIRECT (Brain) ──► 3. SEE (Eye)
     upload file        daily instruction     mind map /
     becomes a Work     revises or derives    prototype
                        a new version         + gap flags ──┘
                             4. RETURN: gaps become tomorrow's Brain question
```

## The object everything acts on: a Work

- A **Work** is created the moment the Hand receives something: a YouTube
  script, a podcast transcript, a CFA chapter PDF, a photo of a sketch.
- A Work has one timeline — **the stream**. Every version, note, derivative,
  and visualisation is an entry on that timeline, in date order.
- Brain and Eye never hold separate copies. They read and act on the Work.

## Step 1 — HOLD (Hand)

**User action:** upload / import / photograph a source file.

**Hand does only four things at intake** (keep intake fast; do not ask the
user to organise):

1. Creates the Work with title, source, and date.
2. Splits the file into addressable parts (transcript → segments;
   document → sections; image → the image + reference notes area).
   Every Brain note and Eye node must be able to point at a part.
3. Places the Work in the stream. Status: **Held**.
4. Suggests an Eye view type by medium (text → mind map; product → prototype;
   image → composition; study set → concept map). User can change it.

## Step 2 — DIRECT (Brain)

**User action:** a **Daily Direction** — a note attached to a specific Work,
never free-floating. It has exactly three fields (this constraint is the
main streamlining decision in the product):

1. **Takeaway** — what stuck today, in the user's own words.
2. **Tweak** — *one* direction or change for today. One, not a list; the
   limit forces priority and keeps the daily act small.
3. **Question** — what is still unresolved. (Often pre-filled by the Eye —
   see Step 4.)

Other Brain entries (journal lines, feedback from other people) attach to
the same Work and timeline, but a Daily Direction is the entry that
*acts* on the Hand's material.

### The two manipulations (Brain → Hand)

A Daily Direction is applied to the Hand's file in exactly one of two ways.
The user picks the type; the interface shows both as plain choices.

**Type A — REVISE the file itself**
- Edit, restructure, annotate, or cut the source.
- Result: a **new version** of the file (v2, v3…). The original is never
  overwritten; the version note is generated from the Daily Direction, so
  the timeline explains *why* each version exists.
- Example: "Tighten the podcast opening" applied to the script → script v2.

**Type B — DERIVE something new from the file**
- The source stays untouched; a new linked item is made from a part of it.
- Derivatives: takeaway card, outline, title list, short-form script,
  flashcards, practice questions, palette study, quote bank.
- Every derivative keeps a **provenance link**: source Work + part +
  the Brain note that asked for it.
- Example: "Pull today's takeaway" from a transcript → takeaway card linked
  to that segment.

Status after a direction is applied: **Directed**.

## Step 3 — SEE (Eye)

**User action:** call the Eye on any Work, at any point — not only at the
end. The Eye is a check, not a finale.

**What the Eye renders** (same Work + all Brain layers so far):

| Work type | Eye view |
| --- | --- |
| Video / podcast / writing idea | Mind map of the argument: claims, examples, stories |
| Product / website idea | Low-fidelity prototype / wireframe from the notes |
| Artwork | Composition layout + moodboard of references and versions |
| Study material (e.g. CFA) | Concept map: topics, formulas, and how they connect |

**The richness check.** On every render the Eye flags three things,
in plain language:

- **Thin** — a branch/part mentioned once, never developed (one node,
  no example, no note).
- **Orphan** — a Brain note not connected to any part of the file.
- **Conflict** — a new tweak that contradicts an earlier direction.

Flags are answers to the user's real question — *"is this idea rich
enough / interesting enough yet?"* — made visible instead of guessed.

Status: **Seen**.

## Step 4 — RETURN

- Every Eye flag drafts the **Question** field of tomorrow's Daily
  Direction. The user edits or replaces it; they never start from blank.
- The loop repeats: the next Brain direction Revises or Derives again,
  the Eye re-renders automatically when a new version or derivative lands.
- A Work leaves the active loop only when the user marks it
  **Shipped/Done**. Its full timeline is kept — that archive is the
  "hindsight" the product is named for.

## Streamlining rules (apply everywhere)

1. **No free-floating notes.** A note must attach to a Work, or it becomes a
   *Seed* — a mini-Work of its own that can later receive a file.
2. **One tweak a day per Work.** Enforced by the three-field Daily Direction.
3. **WIP limit.** At most **3 active Works** in the daily loop. Others rest
   in the stream without guilt prompts.
4. **No manual re-rendering, filing, or linking.** Versions, derivatives,
   provenance links, and Eye updates happen as side effects of the loop.
5. **Templates, not blank pages.** Each founding use case ships with an
   intake split, Daily Direction prompts, and an Eye view preset
   (see `03-use-cases.md`).
6. **Two-minute close.** The day ends with the product showing today's
   Takeaway + Tweak and tomorrow's drafted Question — and the user plants
   today's flower in the Garden (see `11`). Nothing else is asked.
7. **Gathering is gated, working is not.** Adding new material first
   surfaces an unworked saved item (Saved-First, `11`). Inside the loop
   there is no friction at all.
8. **Collecting is never progress.** Only actions inside this loop —
   directions applied, versions, derivatives, flags resolved, Works
   Shipped — count anywhere in the product, including the Garden.

## States summary

`Seed → Held → Directed → Seen → (Revised / Derived → Seen …) → Shipped`

Every state change is a stream entry, dated, in the user's words where the
user supplied words.
