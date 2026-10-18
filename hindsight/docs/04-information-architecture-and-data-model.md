# 04 - Information Architecture and Data Model

This doc is a concept model. It is here for design and prototype work.
The tech schema comes at build time. It must match this doc.

## Main objects

| Object | What it is | Key fields |
| --- | --- | --- |
| **Space** | A named area of life or work, like Content, CFA, Art, or a brand project | name, color, list of Works |
| **Work** | The one unit all modes act on. It starts at Hand intake, or as a Seed | id, title, space, media type, state, start date |
| **SourceFile** | The file the Hand holds for a Work | file link, type, upload date, split into Parts |
| **Part** | One slice of a SourceFile: a segment, a section, or one image area | id, label, order, text or media link |
| **Version** | A new state of a SourceFile, made by a Type A direction | version number, date, change note (the Daily Direction that made it) |
| **DailyDirection** | The Brain note that acts: Takeaway / Tweak / Question | date, the three fields, type (A or B), target Parts |
| **Note** | Any other Brain note: a journal line, feedback from a person | date, author (user or other person), linked Parts if any |
| **Derivative** | A new item made by Type B from one Part: a takeaway card, an outline, flash cards, a draft script, a color study | type, source link (Work + Part + DailyDirection) |
| **Visualization** | One Eye draw of a Work: a mind map, a prototype, a layout view, a concept map | view type, made from (versions and notes in the draw), date |
| **Flag** | One Eye find on a draw: Thin, Orphan, or Conflict | type, target (node, note, or direction), plain-word message |
| **StreamEntry** | One dated line on a Work timeline. Each state change makes one | date, kind, link to the object made or changed |

## Links that count

- A Space holds many Works. A Work sits in one Space. Cross-links
  between Spaces are a later call. See `decisions/`.
- A Work has one SourceFile. The file has many Parts and many Versions.
- A DailyDirection sits on one Work. It aims at one or more Parts. It
  makes one result: a Version (Type A), or one or more Derivatives
  (Type B).
- A Visualization is drawn from a Work's current Version plus all its
  Notes and Daily Directions to date. It draws again on its own when
  one of those changes.
- A Flag sits on a Visualization. With one click, the user can turn a
  Flag into the Question field of the next Daily Direction.
- **The loop never cuts a thing out of the timeline.** A user can
  delete a whole Work. That is their data and their right. See `08`.
  But a Revise makes a new version. It never writes over an old one.

## Screens (product IA)

1. **The Stream** (home): all live Works in all Spaces, newest act
   first. Users can filter by Space and by mode (Hand, Brain, Eye).
2. **A Work view**: three tabs on one object. Hand shows the file and
   its versions. Brain shows notes and Daily Directions. Eye shows the
   current draw and its flags. It is one object in three views. The
   screens must never make it feel like three places.
3. **Spaces list**: a flat list. No folders in the first version.
4. **Archive**: Shipped Works, with full timelines, and a search box.
   This is the hindsight view.

## States

`Seed -> Held -> Directed -> Seen -> Shipped`. See `02` for what each
state means. The state comes from the last StreamEntry. No one sets it
by hand, but for two cases: Seed and Shipped.
