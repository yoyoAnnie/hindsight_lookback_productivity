# Hindsight

All my thinking, in one stream.

I'm Annie. I'm building Hindsight, a scrapbook journal for ideas.

I built it for one problem. My ideas sat in many apps at once. A file
was in a drive. Feedback was in a chat. A sketch was on paper. I lost
work between the apps, and I lost time on the switch.

So I put all of it in one stream. I work in three modes:

| Mode | Verb | What it does |
| --- | --- | --- |
| **Hand** - Projects | Hold | Holds the source: files, scripts, transcripts, reports, images |
| **Brain** - Notes | Direct | Holds my daily notes. My notes tell the Hand what to change or what to make |
| **Eye** - Visualize | See | Shows the same work as a mind map or a prototype, so I can see its shape |

The three modes are not three places. They are three actions on the
same object. I call that object a **Work**. The loop is:
**Hold -> Direct -> See -> Return**. See `docs/02-workspace-workflow.md`.

## Status

Concept and design phase. I build the website first. The app comes
later. I log each work session in this repo. See
`docs/07-development-process-and-prompting.md` and the logs in
`sessions/`.

## How to read these docs

Read the docs in number order if you are new. Start with 01 and 02.

- `docs/01-vision-and-concept.md` - why I built this, who it is for, what it is not
- `docs/02-workspace-workflow.md` - the main workflow: the Hand -> Brain -> Eye loop
- `docs/03-use-cases.md` - how I use it for YouTube and podcast work, CFA study, and art, step by step
- `docs/04-information-architecture-and-data-model.md` - the objects, the states, and the links between them
- `docs/05-design-system.md` - colors, type, sizes, and motion values
- `docs/06-mvp-scope-and-roadmap.md` - what ships first and what waits
- `docs/07-development-process-and-prompting.md` - how I run work sessions and how I log them
- `docs/08-privacy-and-ip.md` - private by default. The ideas in this repo are mine
- `docs/09-user-journey-map.md` - the users I talked to, the main task, the map of the 5 phases, and the hard points in the flow
- `docs/10-guided-actions-and-buttons.md` - one main button per state, so you always know your next step
- `docs/11-garden-and-anti-foraging.md` - why we collect too much and act too little, and the Garden: one hand-drawn plant per day of real action, on a 5 x 6 grid per month
- `decisions/` - records of big choices and why I made them
- `templates/` - copy one of these when you start a new doc

## Rules for this repo

1. This repo is **private**. Do not make it public. Do not copy the
   concept out of the repo. See `LICENSE.md`.
2. Each work session ends with a log in `sessions/`.
3. Each big choice gets a record in `decisions/`.
4. For design work, I put the full plan and the full values in the
   first prompt. After that, I fix one thing at a time. I do not
   restart the work with a vague prompt. See `docs/07`.

## Start here if you will work on this with me

1. Read `docs/01` and `docs/02` first. All other docs build on the loop.
2. Copy a file from `templates/`. Do not start from a blank page.
3. Open an issue first. Use the forms in `.github/ISSUE_TEMPLATE/`.

---

(c) 2026 Annie. All rights reserved. See `LICENSE.md`.
