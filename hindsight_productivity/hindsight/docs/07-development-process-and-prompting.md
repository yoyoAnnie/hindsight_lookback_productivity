# 07 - Development Process and Prompting

This doc says how we work and how we log the work. It is here so the
repo reads as a real work record, not a pile of files.

## How one work session runs

1. **Before:** write the one goal of the session in the session log.
   Copy `../templates/session-log-template.md` into `../sessions/`.
2. **First move:** one prompt sets the full plan for the session. All
   structure is set here.
3. **Middle:** fixes and small changes only.
4. **After:** close the session log. Say what changed. Say what we
   tried and cut, and why. Say the next step. Update `../CHANGELOG.md`.
   Add a record in `decisions/` if a big choice was made.

## Rules we learned from a study of design sessions

A study watched five designers. Each one ran one design session in
the same tool, on the same brief. The sessions were taped end to end:
screen, sound, mouse, clicks, and keys. Three rules came out of it.
We use them as law on this project.

1. **Put the visual values in the first prompt, even if a design
   system is set.** One designer did this. That designer got a result
   that was fit to ship. A set system is not text the tool will read
   on its own. So the values live in `05-design-system.md`, and we
   paste them in full in each first prompt.
2. **The full plan goes in the first prompt.** One designer wrote a
   plan prompt at a point past the first move. All others did not.
   After the first move, a session is a fix game. So the first prompt
   must hold the full structure: parts in order, layout, parts list,
   exact copy, motion values, and phone rules.
3. **Do not use meta prompts.** The worst drop in the study came from
   a prompt that told the tool to step back and think again. Words
   like "reconsider", "rethink", and "start over" tell the tool it
   can throw out work that was set and good.
   - Role play is meta too. "Act as a pro designer" is banned. Write
     plain build steps.
   - **The fix form, and the only form we use after move one:**
     `Keep everything else exactly as it is. Change only [element]: from [A] to [B].`

   One point stays open from the study. We do not know if the drop is
   a fault of the tool, or a fault of how designers learn to prompt
   it. This project logs its own sessions. In time, our own log can
   help answer that.

## The set first prompt for the landing page

This is the one true copy. Change it here first, then use it.

- Source: the work session of 2026-10-16. It holds the product facts,
  the values from `05`, a plan of 8 parts in order (nav, hero, problem
  line, three modes, stream center piece, Visualize close look, human
  touch, close and footer), full copy set word for word, motion values,
  mode colors, and the fix-only rule for all prompts after it.
- The session log for that day is
  `../sessions/2026-10-16-concept-and-documentation.md`.

If the first prompt changes in a big way, add a record in
`decisions/` and say why.

## What we commit, and when

- Docs and specs: the same day we agree on them.
- Session logs: at the end of the session they log. Never in a batch
  days later.
- Designs and click models: a file export goes in the repo if the tool
  lets us. The session log links to it.
- Code, in later phases: small commits. Plain commit text.
  See `../CONTRIBUTING.md`.
