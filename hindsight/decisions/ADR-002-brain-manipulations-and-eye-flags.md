# ADR-002 — Brain instructions manipulate Hand files in exactly two ways; the Eye reports gaps back

- **Date:** 2026-10-16
- **Status:** Accepted

## Context

"Notes connected to files" is too vague to build or design against. The
connection needed a precise shape: what does a note *do* to a file, and what
does a visualisation give back, beyond a picture?

## Decision

1. A Brain instruction (the Daily Direction: Takeaway / Tweak / Question)
   applies to a Hand file in exactly two ways:
   - **Type A — Revise:** change the file, producing a new preserved version.
   - **Type B — Derive:** make a new, provenance-linked item from the file
     without changing it.
2. The Eye is a check, not only a view. Every render flags **Thin**,
   **Orphan**, and **Conflict** items, and a flag can be converted into the
   Question of the next Daily Direction — closing the loop.

## Alternatives considered

- Notes as comments only (no manipulation) — rejected: comments do not
  move work forward; the user still does the file work in another app,
  which recreates the scatter.
- Free-form "AI, improve this" actions — rejected: the Brain is the user's
  judgement; open-ended automation hides what changed and why, and breaks
  the version/provenance record.

## Consequences

- Versions and provenance links are core objects in `docs/04`, not extras.
- The workflow doc (`docs/02`) is written around Hold → Direct → See →
  Return, with the Return step mandatory in any flow design.
- Each use case must define what "rich enough" means via these flags
  (`docs/03`).
