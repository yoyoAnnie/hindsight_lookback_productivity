# Session Log — 2026-10-16 — Interview finding, anti-foraging design, the Garden

- **Goal (written before starting):** Fold the owner's interview findings
  and the Garden idea into the product design and docs, resolving the
  overload dilemma in the design rather than just noting it.
- **Tool(s) used:** Muse (working session). Evidence: owner's user
  interviews as reported by the owner this date.
- **Opening prompt used:** n/a (documentation session).

## What was done

- Persona in docs/09 updated from hypothesis to interview-grounded:
  overload slows creation; over-collecting and over-exploring pull users
  away from their goals; temperament leans anxious and overexcited.
- Diagnosis written in the owner's psychology frame — information
  foraging theory: weak scent on saved patches, zero switching cost,
  collecting mistaken for progress.
- Wrote docs/11 (anti-foraging rules + Garden spec) and ADR-003.
- Updated docs/01 (dilemma section), docs/02 (rules 6–8), docs/05 (garden
  values), docs/06 (garden + Saved-First into MVP; feeds/streaks into
  Out), docs/09 (O7 Garden, O8 Saved-First, with metrics), docs/10
  (day close now ends at the Garden), README and CHANGELOG.

## Key design calls in this session

- Garden plant is earned by a **completed action**, not by logging in
  (deviation from the first sketch, reasoned in ADR-003: login rewards
  train the foraging/checking habit; action rewards make effort concrete).
- No catalogue of plants/animals, no wilting/streak-risk, no numbers on
  the garden screen — the reward must not restart collecting or guilt.
- Flower colour comes from the Work done that day, so a monthly garden
  can be read as a record of where the days actually went.

## Decisions made

- [x] Decision record added — `decisions/ADR-003-anti-foraging-and-garden.md`

## Next step (single, concrete)

Prototype the day-close → garden moment (docs/10 test #1 applies: cover
everything but **Draw today's flower** — it should still explain the day).
