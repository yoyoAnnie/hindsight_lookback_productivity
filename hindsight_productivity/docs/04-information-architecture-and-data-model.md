# 04 — Information Architecture and Data Model

Conceptual model only. Enough for design and prototyping; a technical
schema comes with the build phase and must stay consistent with this file.

## Core objects

| Object | Definition | Key fields |
| --- | --- | --- |
| **Space** | A named area of life/work the user thinks in (e.g. Content, CFA, Art, a brand project) | name, colour, list of Works |
| **Work** | The single unit everything acts on; created at Hand intake or as a Seed | id, title, space, medium type, status, created date |
| **SourceFile** | The file the Hand holds for a Work | file ref, type, upload date, split into Parts |
| **Part** | An addressable slice of a SourceFile (segment, section, or image region) | id, label, order, text/media ref |
| **Version** | A Revised state of a SourceFile, created by a Type A Brain direction | version no., date, change note (= the Daily Direction that caused it) |
| **DailyDirection** | The Brain's acting note: Takeaway / Tweak / Question | date, three fields, manipulation type (A or B), target Part(s) |
| **Note** | Any other Brain entry: journal line, feedback from a person | date, author (user/other), linked Part(s) if any |
| **Derivative** | An item Derived (Type B) from a Part: takeaway card, outline, flashcards, script draft, palette study | type, provenance (Work + Part + DailyDirection) |
| **Visualization** | An Eye render of a Work: mind map / prototype / composition / concept map | view type, generated-from (versions + notes included), date |
| **Flag** | An Eye finding on a Visualization: Thin / Orphan / Conflict | type, target (node / note / direction), plain-language message |
| **StreamEntry** | One dated line on a Work's timeline; every state change creates one | date, kind, ref to the object created/changed |

## Relationships (the connections that matter)

- A Space contains many Works. A Work belongs to one Space (cross-links are
  a later decision — see `decisions/`).
- A Work has one SourceFile, which has many Parts and many Versions.
- A DailyDirection belongs to exactly one Work, targets one or more Parts,
  and produces exactly one outcome: a Version (Type A) **or** one or more
  Derivatives (Type B).
- A Visualization is generated from a Work's current Version + all its
  Notes/DailyDirections to date. It is regenerated automatically when either
  changes.
- A Flag belongs to a Visualization and can be converted, with one action,
  into the Question field of the next DailyDirection.
- **Nothing is deletable from the timeline by the loop.** Users can delete a
  Work entirely (their data, their right — see `08-privacy-and-ip.md`), but
  versions and notes are never silently overwritten; Revision creates, it
  does not replace.

## Navigation (product IA)

1. **The Stream** (home): all active Works across Spaces, newest activity
   first; filter by Space and by mode (Hand / Brain / Eye items).
2. **A Work view**: three panes/tabs on one object — Hand (file + versions),
   Brain (notes + Daily Directions), Eye (current visualisation + flags).
   One object, three views: the IA must never present these as three places.
3. **Spaces list**: simple list, no nested folders in the MVP.
4. **Archive**: Shipped Works, full timelines, searchable — the hindsight
   view.

## Statuses

`Seed → Held → Directed → Seen → Shipped`, as defined in
`02-workspace-workflow.md`. Status is computed from the latest StreamEntry,
never set by hand except Seed and Shipped.
