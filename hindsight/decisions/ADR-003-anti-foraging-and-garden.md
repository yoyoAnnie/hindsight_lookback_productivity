# ADR-003 — Design against over-foraging; the Garden rewards actions, never logins or collecting

- **Date:** 2026-10-16
- **Status:** Accepted

## Context

User interviews reported information overload slowing creation rather than
speeding it: narrowing down is hard, users over-collect references they
never revisit, and keep exploring instead of working what they saved —
information-foraging behaviour (weak scent on saved patches, zero cost to
switch patches). Interviewees also lean anxious and easily overexcited.

Two product questions followed: whether Hindsight should contain any
discovery surface, and how to reward daily use (the owner's garden idea:
a hand-drawn flower a day in a 5 × 6 monthly grid).

## Decision

1. **No discovery surface, and friction at intake.** No Explore feed or
   recommendations anywhere. Adding new material first surfaces an
   unworked saved item (Saved-First). Collecting earns no progress signal
   of any kind.
2. **The Garden exists, tied to action.** One plot per day, planted only
   after a Daily Direction is applied or a flag is resolved — not on
   login. The drawing is traced/guided, under a minute, and the plant links
   back to the stream entry that earned it.
3. **Nothing can be lost.** No streaks-at-risk, wilting, expiry, red
   states, or social comparison anywhere in the product. Missed days are
   empty soil, full stop.

## Alternatives considered

- Plant on login (as first sketched) — rejected: it rewards opening the
  app, i.e. it trains the checking/foraging habit the product exists to
  break, and produces exactly the "empty sunk cost" feeling interviewees
  described when a streak has no work behind it.
- A catalogue/collection layer for plants and animals — rejected: it
  rebuilds collecting inside the reward system.
- An Explore page to "help inspiration" — rejected: it contradicts the
  core interview finding; inspiration is not the users' problem,
  narrowing is.

## Consequences

- `docs/11-garden-and-anti-foraging.md` is the binding spec for the garden
  and intake behaviour; the journey map (docs/09) gains opportunities O7
  and O8; the day-close flow in docs/10 ends at the garden.
- Progress metrics project-wide count actions only (docs/09, Row 6).
- Any future proposal for recommendations, streaks, or collectible
  rewards must supersede this ADR explicitly, with interview evidence.
