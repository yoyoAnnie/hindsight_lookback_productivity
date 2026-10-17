# 06 - MVP Scope and Roadmap

MVP means the first version that a user can use. Web first. One user.
Work is private.

## In the MVP

The full loop runs end to end for **one** use case. The other two
cases ship as forms (templates).

1. Spaces (a flat list) and Works. Hand intake takes text files,
   PDFs, and images.
2. Intake splits text files into Parts on its own, by section or segment.
3. Brain: Notes, plus the Daily Direction with three fields. The
   direction acts in two ways: Revise (Type A, makes a new version)
   and Derive (Type B, makes a takeaway card, an outline, or flash cards).
4. Eye: mind map view and concept map view. The map draws again when
   the Work changes. Three flags run as plain rules: Thin, Orphan,
   Conflict.
5. The Stream home: users can filter by Space and by mode. The Work
   view shows Hand, Brain, and Eye as three views of one object.
6. The landing page that shows the product. Design values are in `05`.
7. An archive of Shipped Works, with full timelines.
8. The Garden, in its basic form. See `11`. One month grid of 5 x 6.
   The user draws a plant at day close, after a real act is done. The
   plant links to its stream line. The year view is a plain 3 x 4 grid
   of months. Intake uses Saved-First. There is no feed for new ideas
   in any part of the app. See the ADR-003 record in `decisions/`.

## Out of the MVP

We cut these on purpose. They are not "to do soon." They are out
until a phase below says they are in.

- No team work. No share links. No notes from other accounts. No
  public pages.
- No phone apps. Web only, and it must work on a phone screen. The app
  is Phase 3.
- No prototype Eye view in the MVP. Mind map and concept map come
  first. The prototype view is Phase 2.
- No folders in folders. No tag system. No calendar link.
- No feed for new ideas. No picks "for you." No streak counts. No
  items that wilt or run out. No items you collect as a reward.
  See ADR-003.
- No AI text shown as the user's own words. The machine can split,
  link, draw, and flag. It can draft the Question field. A draft is
  marked as a draft, and the user edits it.

## Phases

| Phase | What ships | Test to pass the phase |
| --- | --- | --- |
| 0 - Docs and design | This repo. The landing page design. A click model of the loop | A new person can walk through Use Case A in the model, with no one there to explain it |
| 1 - MVP web | The loop above, for Use Case A. Forms for Cases B and C | I take one real Work from upload to Shipped |
| 2 - Eye grows | Prototype Eye view. Art layout view. Richer flags | A user runs Use Case C on a real piece of art, start to end |
| 3 - App | A phone app. Same objects, same loop. It is made for fast intake: shoot a photo, write the day's direction | A user does a full Daily Direction on a phone in under 2 minutes |
| 4 - A call to make | Team work and share links: yes or no, based on real use data | The call is logged in `decisions/`, both ways count as a pass if the data is there |

## Risks and open points

- Will users keep a daily habit if the loop takes more than 5 minutes?
  The design fights this risk: three fields, one tweak, a draft
  Question. But we must test it with real users.
- Rule-based flags may feel thin. The Eye says "is it rich?" and rules
  can only say part of that. Phase 1 must test flags next to the
  my own call, case by case.
- Split quality makes or breaks the back links. If splits are bad,
  links feel wrong. Test the split on real files before we build
  full intake.
- The name "Hindsight" needs a trademark check before any public launch.
