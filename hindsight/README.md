# Hindsight

All your thinking, in one stream.

Hindsight is a scrapbook journal for ideas. It solves one problem. A
person's ideas sit in many apps at once. A file is in a drive. Feedback
is in a chat. A sketch is on paper. Work gets lost between the apps.

Hindsight puts all of it in one stream. The user works in three modes:

| Mode | Verb | What it does |
| --- | --- | --- |
| **Hand** - Projects | Hold | Holds the source: files, scripts, transcripts, reports, images |
| **Brain** - Notes | Direct | Holds daily notes. The notes tell the Hand what to change or what to make |
| **Eye** - Visualize | See | Shows the same work as a mind map or a prototype, so the user can see its shape |

The three modes are not three places. They are three actions on the same
object. We call that object a **Work**. The loop is:
**Hold -> Direct -> See -> Return**. See `docs/02-workspace-workflow.md`.

## Status

Concept and design phase. The website comes first. The app comes later.
We log each work session in this repo. See
`docs/07-development-process-and-prompting.md` and the logs in `sessions/`.

## How to read these docs

Read the docs in number order if you are new. Start with 01 and 02.

- `docs/01-vision-and-concept.md` - why this exists, who it is for, what it is not
- `docs/02-workspace-workflow.md` - the main workflow: the Hand -> Brain -> Eye loop
- `docs/03-use-cases.md` - YouTube and podcast work, CFA study, and art, step by step
- `docs/04-information-architecture-and-data-model.md` - the objects, the states, and the links between them
- `docs/05-design-system.md` - colors, type, sizes, motion values, and language rules
- `docs/06-mvp-scope-and-roadmap.md` - what ships first and what waits
- `docs/07-development-process-and-prompting.md` - how we run work sessions and how we log them
- `docs/08-privacy-and-ip.md` - private by default. The ideas in this repo belong to the owner
- `docs/09-user-journey-map.md` - the user, the main task, the map of the 5 phases, and the hard points in the flow
- `docs/10-guided-actions-and-buttons.md` - one main button per state, so the user always knows the next step
- `docs/11-garden-and-anti-foraging.md` - why users collect too much and act too little, and the Garden: one hand-drawn plant per day of real action, on a 5 x 6 grid per month
- `decisions/` - records of big choices and why we made them
- `templates/` - copy one of these when you start a new doc

## Rules for this repo

1. This repo is **private**. Do not make it public. Do not copy the concept
   out of the repo. See `LICENSE.md`.
2. Each work session ends with a log in `sessions/`.
3. Each big choice gets a record in `decisions/`.
4. Design work uses the rules in `docs/07`. Put the full plan and the full
   values in the first prompt. After that, fix one thing at a time. Do not
   restart the work with a vague prompt.
5. Write docs in plain words, like a developer who talks to a reader face
   to face. Short sentences. Basic link words: and, but, so, because,
   then, if, when. See `docs/05` for the full language rules.

## Start here if you will work on this

1. Read `docs/01` and `docs/02` first. All other docs build on the loop.
2. Copy a file from `templates/`. Do not start from a blank page.
3. Open an issue first. Use the forms in `.github/ISSUE_TEMPLATE/`.

---

(c) 2026 Annie. All rights reserved. See `LICENSE.md`.
