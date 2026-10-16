# 07 — Development Process and Prompting

How work on Hindsight is done and recorded, so the GitHub history reads as a
real development process — not a pile of files.

## The session rhythm

1. **Before:** state the session's single goal in the session log
   (copy `../templates/session-log-template.md` into `../sessions/`).
2. **Opening move:** one scaffolding prompt (below) starts any design or
   build session. All structure is decided here.
3. **Middle:** refinement and corrections only.
4. **After:** finish the session log (what changed, what was rejected and
   why, next step), update `../CHANGELOG.md`, and add a decision record if
   a structural choice was made.

## Rules learned from recorded designer sessions

These rules come from a study of five designers running single design-tool
sessions against the same brief (sessions captured end-to-end with screen,
audio, and input recording). Apply them as project law:

1. **Specify visual values in the opening prompt, even when a design system
   already exists.** The only designer who restated values reached a
   production-ready result. An approved system is not context a tool can be
   trusted to read on its own. → The values live in `05-design-system.md`
   and are pasted, in full, into every opening prompt.
2. **Scaffolding belongs at the start.** Only one designer wrote a
   scaffolding prompt anywhere except the opening. After the first move,
   the session is a refinement-and-correction game — so the opening prompt
   must carry the full page/product structure: sections in order, layout,
   components, exact copy, motion values, responsive rules.
3. **Be cautious with meta prompts.** The single largest quality drop in
   the study came from a prompt asking the tool to step back. Treat words
   like "reconsider", "rethink", "start over" as a request to discard the
   approved work.
   - **Role-play is also meta.** "Act as a professional designer" is banned
     for the same reason. Use direct build instructions instead.
   - **Correction template (the only follow-up form):**
     `Keep everything else exactly as it is. Change only [element]: from [A] to [B].`

   Open question carried from the study: whether the regression after meta
   prompts is a property of the tool, or of how designers learn to prompt
   it. This project logs its own sessions so the question can be answered
   from our record later.

## The current approved opening prompt (landing page)

Stored here as the canonical version. Edit here first, then use.

- Source: session of 2026-10-16 — product definition, values from
  `05-design-system.md`, scaffold of 8 sections (nav, hero, problem strip,
  three modes, stream centrepiece, Visualize close-up, human touch,
  close + footer), copy written in full, motion values specified, mode
  colours and roles defined (Hand / Brain / Eye), corrections rule stated.
- The full text was delivered in the 2026-10-16 working session and is the
  basis of the landing-page design session log:
  `../sessions/2026-10-16-concept-and-documentation.md`.

When the opening prompt changes materially, add a decision record
explaining why.

## What gets committed, and when

- Docs and specs: as soon as they are agreed, same day.
- Session logs: at the end of the session they describe, never batched.
- Designs/prototypes: export + link from the session log; source files in
  the tool, exports in the repo if the tool allows.
- Code (later phases): small commits, plain messages (see
  `../CONTRIBUTING.md`).
