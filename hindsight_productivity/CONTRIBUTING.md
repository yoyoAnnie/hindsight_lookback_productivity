# Contributing to Hindsight

This is a private, single-owner project. These rules exist so the record
stays clean as the project grows and if collaborators join later.

## Ground rules

1. **One object rule.** Anything you design or build must act on the shared
   *Work* object. Do not create a feature that copies content into a separate
   space. See `docs/04-information-architecture-and-data-model.md`.
2. **Plain language.** Product copy, UI text, and docs use plain human
   English. The banned-words list is in `docs/05-design-system.md`.
3. **Values before adjectives.** Never describe design as "clean" or "fancy"
   in a spec. Give the hex, the size, the duration, the easing.

## Workflow for any change

1. Open an issue first (use `.github/ISSUE_TEMPLATE/`).
2. If the change alters structure, the workflow, or the data model, add a
   decision record in `decisions/` using the template in `templates/`.
3. Work in a branch named `area/short-description`
   (e.g. `design/hero-parallax`, `docs/cfa-use-case`).
4. Open a pull request using `.github/pull_request_template.md`.
5. End every working session with a log in `sessions/`
   (`templates/session-log-template.md`) and a line in `CHANGELOG.md`.

## Design / AI-tool sessions

Follow `docs/07-development-process-and-prompting.md`:

- Scaffolding and all visual/motion values go in the **opening** prompt of a
  session, even if a design system already exists.
- After the opening, only corrections: *"Keep everything else exactly as it
  is. Change only X: from A to B."*
- Never use meta prompts ("reconsider", "rethink", "start over") — in this
  project's recorded experience, they cause the tool to discard approved work.

## Commits

Short, plain, present tense: `add eye gap flags to workflow doc`,
`fix stream card spacing to 12px`. One subject per commit where practical.
