# Hindsight

**All your thinking, in one stream.**

Hindsight is a scrapbook journal for ideas and brainstorming. It solves one
problem: a person's ideas are scattered across different projects, spaces, and
apps — a file in one place, feedback in a chat, a sketch on paper — and get lost
between them.

Hindsight puts everything in one continuous stream, worked on through three
connected modes:

| Mode | Verb | What it does |
| --- | --- | --- |
| **Hand** — Projects | Hold | Holds the source: files, scripts, transcripts, reports, images |
| **Brain** — Notes | Direct | Daily notes and instructions that change or build on what the Hand holds |
| **Eye** — Visualize | See | Renders the same work as a mind map or prototype, so you can see its shape |

The three modes are not three separate spaces. They are three actions on the
**same object** — a *Work* — in a loop: **Hold → Direct → See → Return**.
See [`docs/02-workspace-workflow.md`](docs/02-workspace-workflow.md).

## Status

Concept and design phase. Website landing page first, app later.
Development is documented in this repository as it happens — see
[`docs/07-development-process-and-prompting.md`](docs/07-development-process-and-prompting.md)
and the session logs in [`sessions/`](sessions/).

## Documentation map

- [`docs/01-vision-and-concept.md`](docs/01-vision-and-concept.md) — why this exists, who it is for, what it is not
- [`docs/02-workspace-workflow.md`](docs/02-workspace-workflow.md) — the principal workflow: the Hand → Brain → Eye loop
- [`docs/03-use-cases.md`](docs/03-use-cases.md) — YouTube/podcast content, CFA study, artwork, step by step
- [`docs/04-information-architecture-and-data-model.md`](docs/04-information-architecture-and-data-model.md) — objects, states, and how they connect
- [`docs/05-design-system.md`](docs/05-design-system.md) — visual values, motion values, language rules
- [`docs/06-mvp-scope-and-roadmap.md`](docs/06-mvp-scope-and-roadmap.md) — what ships first, what waits
- [`docs/07-development-process-and-prompting.md`](docs/07-development-process-and-prompting.md) — how design/build sessions are run and recorded
- [`docs/08-privacy-and-ip.md`](docs/08-privacy-and-ip.md) — private by default; ownership of ideas and files
- [`docs/09-user-journey-map.md`](docs/09-user-journey-map.md) — persona, scenario, future-state journey map (5 phases × 6 rows), moments of truth, metrics
- [`docs/10-guided-actions-and-buttons.md`](docs/10-guided-actions-and-buttons.md) — the no-dead-ends rule: one primary button per state, decision budget, banned anti-patterns
- [`docs/11-garden-and-anti-foraging.md`](docs/11-garden-and-anti-foraging.md) — the overload finding, information-foraging diagnosis, anti-foraging rules, and the Garden (a hand-drawn plant per action-day, 5 × 6 monthly grid)
- [`decisions/`](decisions/) — decision records (why a choice was made)
- [`templates/`](templates/) — session log, feature spec, use case, decision record

## Repository rules

1. This is a **private** repository. Do not make it public and do not copy
   concept documents outside it. See `LICENSE.md`.
2. Every working session ends with a session log in `sessions/`.
3. Every structural decision gets a decision record in `decisions/`.
4. Design work follows the prompting rules in
   `docs/07-development-process-and-prompting.md`: values and scaffolding in
   the opening prompt, corrections after that — never a fresh restart.

## Quick start (for future collaborators)

1. Read `docs/01` and `docs/02` first. Everything else builds on the loop.
2. Copy the templates in `templates/` instead of starting a blank document.
3. Open an issue using the templates in `.github/ISSUE_TEMPLATE/` before
   building anything new.

---

© 2026 Annie. All rights reserved. See `LICENSE.md`.
