# ADR-001 — Three modes act on one Work in one stream

- **Date:** 2026-10-16
- **Status:** Accepted

## Context

The first framing of Hindsight was three spaces — Hand for projects, Brain
for notes, Eye for visualisation. Three spaces repeats the exact problem the
product exists to solve: the user's material scattered across places, with
copies drifting apart.

## Decision

Hand, Brain, and Eye are three **modes of action on a single object** (a
Work) with one timeline, the stream. The Hand holds the source, the Brain's
notes act on that source, the Eye renders that same source plus its notes.
No feature may copy content into a separate space.

## Alternatives considered

- Three linked spaces with sync — rejected: sync is the scatter problem
  wearing a uniform; links break, copies drift.
- Folder-first organisation with modes as tags — rejected: folders ask the
  user to organise before they can think, which intake must never do.

## Consequences

- The data model (`docs/04`) is built around the Work and its timeline.
- The Work view is one screen with three views, never three destinations.
- Any future feature proposal must state which objects it touches and how
  it respects the one-object rule (`CONTRIBUTING.md`).
