# 06 — MVP Scope and Roadmap

## MVP (website first)

One user, private, web. The full loop for **one** use case end to end,
with the other two cases available as templates:

**In**

1. Spaces (flat list) and Works; Hand intake for text files, PDFs, images.
2. Automatic split into Parts for text (sections/segments).
3. Brain: Notes + the three-field Daily Direction, with Type A (Revise →
   version) and Type B (Derive → takeaway card, outline, flashcards)
   manipulations.
4. Eye: mind map and concept map views, regenerated on change; the three
   flags (Thin / Orphan / Conflict) in rule-based form.
5. The Stream home: filters by Space and by mode; Work view with
   Hand / Brain / Eye as three views of one object.
6. Landing page presenting the product (design per `05-design-system.md`).
7. Archive of Shipped Works with full timelines.
8. The Garden, basic form (`11`): monthly 5 × 6 grid, traced drawing at
   day close after a completed action, plant linked to its stream entry,
   simple year overview. Plus Saved-First intake and no discovery surface
   anywhere (ADR-003).

**Out (explicitly, for the MVP)**

- No collaboration, sharing, comments from other accounts, or public pages.
- No native apps (responsive web only) — app is Phase 3.
- No prototype/wireframe Eye view (mind/concept map first; prototype view is
  Phase 2).
- No nested folders, no tags system, no calendar integration.
- No Explore/discovery feed, recommendations, streaks, wilting/expiry
  mechanics, or collectible rewards (ADR-003).
- No AI-generated content presented as the user's own words. Assistance is
  limited to splitting, linking, rendering, flagging, and drafting the
  Question field — always shown as a draft the user edits.

## Phases

| Phase | Content | Exit test |
| --- | --- | --- |
| 0 — Document & design | This repo; landing page design; clickable prototype of the loop | Prototype walked through Use Case A without explanation |
| 1 — MVP web | Loop above for Use Case A, templates for B and C | One real Work carried from upload to Shipped by the owner |
| 2 — Eye grows | Prototype Eye view; artwork composition view; richer flags | Use Case C completed on a real piece |
| 3 — App | Native app, same objects and loop, capture-first (photo intake, daily direction on phone) | Daily Direction completed on phone in under 2 minutes |
| 4 — Decide | Collaboration / sharing question revisited, with data from real use | Decision recorded in `decisions/` either way |

## Risks and open questions

- Will users keep a daily habit if the loop takes more than ~5 minutes?
  (Mitigated by design: three fields, one tweak, drafted Question.)
- Rule-based flags may feel shallow next to the promise "see if it is rich
  enough". Phase 1 must test flags against the owner's own judgement.
- File-splitting quality decides whether provenance links feel magic or
  broken. Prototype this before the full intake build.
- Naming/trademark check for "Hindsight" before any public launch.
