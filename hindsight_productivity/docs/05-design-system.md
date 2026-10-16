# 05 — Design System

Values, not adjectives. Any design prompt, spec, or build must use the
numbers in this file. **Restate them in every opening prompt** — a design
system file is not context a tool can be trusted to read on its own
(see `07-development-process-and-prompting.md`).

## Direction in one line

Futuristic Renaissance × Notion-clean. Reference works studied:
Contra Labs (restraint, card system) and Shopify Editions Winter '26
"RenAIssance" (scroll-driven motion, Renaissance × pixel × modern-object
collage). Motion and transition are the primary taste signal; layout is
secondary.

## Colour

| Token | Hex | Use |
| --- | --- | --- |
| paper | `#F6F1E7` | page background |
| surface | `#FFFEF9` | cards, panels |
| ink | `#211D18` | primary text |
| muted | `#6F675A` | secondary text |
| line | `#E3DCCB` | 1px hairline borders |
| gold | `#B9922E` | rules, numerals, underlines only — under 5% of any screen |
| hand | `#C17A3A` | Hand mode colour (dot, tag, icon) |
| brain | `#4F7D78` | Brain mode colour |
| eye | `#6C4CFF` | Eye mode colour; also the futuristic/pixel accent |
| dark | `#1E1B16` | dark section background (text: paper) |

No gradients. No glassmorphism. No stock photos. Paper grain overlay at 4%
opacity over painted areas only.

## Type

- Display: **Source Serif 4**; italic for exactly one accent word per headline.
- UI/body: **Inter**. Labels/timestamps: mono, 11px, uppercase, tracking 0.08em.
- Hero headline 76px / line-height 0.98 / letter-spacing −0.03em.
- Section headlines 48px / 1.05. Card titles 22px. Body 17px / 1.55. Small 14px.
- Mobile: hero 44px, body unchanged.

## Layout and components

- Max width 1200px, 24px gutters, 8px spacing grid, 128px section padding
  (72px mobile).
- Radius: cards 12px, UI panels 8px, buttons 999px (pill).
- Shadows: none, except the product/app mock: `0 24px 60px rgba(33,29,24,0.12)`.
- Buttons: primary = ink background, paper text. Secondary = text + underline.
- Stream cards: mode colour dot + mono timestamp + title + one-line excerpt.
- Mode icons: simple line icons — hand, brain, eye — drawn once, used at
  16px and 24px only.

## Collage rule (imagery)

One image may combine three eras **only** if unified: Renaissance oil
painting (base) + pixel elements (crisp, 4–6× scale, `image-rendering:
pixelated`) + one modern object (e.g. a laptop showing product UI) — with
one light direction, a soft shadow under every inserted object, and grain
over the finished composition. Painting crops appear as framed panels with
a parchment mat and 8px offset border, or as taped scrapbook details.

## Motion values

Motion is specified, never left to "fancy" or "smooth":

- Easing, all UI: `cubic-bezier(0.22, 1, 0.36, 1)`.
- Target build stack for landing page: Lenis smooth scroll (duration 1.2,
  lerp 0.09) synced to GSAP ScrollTrigger; all scroll animations **scrubbed**
  (tied to scroll progress, reversible), no one-shot pop-ins, no hard
  section cuts.
- Load: hero painting scales 1.08 → 1.00 over 1200ms; headline lines rise
  behind masks, 700ms, 80ms stagger.
- Scroll: section content rises 24px / 700ms on entry; parallax layers —
  painting 0.3×, main content 1.0×, floating cards 1.3×.
- Pinned scenes (prototype tool permitting): pin a chapter for +150%
  scroll distance while its layers transform; background colour
  interpolates between sections.
- Filtering the stream (All / Hand / Brain / Eye): cards reorder with a
  450ms layout animation.
- Hover: card lifts 2px, 300ms; painting panel crossfades painted ↔ pixel
  version, 300ms, scale 1.02.
- Animate `transform` and `opacity` only. Zero layout shift.
- `prefers-reduced-motion`: no parallax, no pinning, fades only.

## The Garden (visual and motion values)

A calming counter-space to the work screens (full spec: `11`). Plots are
rounded-square soil cells, radius 16px, on paper, 10px grid gap, hairline
fence border around each month. Petal palette: the three mode colours,
gold, and one soft pink `#E8A0A8`. Plant lines are hand-drawn style —
2px, slightly irregular — never geometric icons. Garden motion is slower
than product motion on purpose: a new plant draws itself over ~1200ms;
idle sway is ±1deg at 6s and stops under `prefers-reduced-motion`. No
numbers, counts, percentages, or streaks appear on the garden screen.
Nothing in the garden may wilt, die, or expire — in imagery or in copy.

## Language rules (product copy and docs)

Plain human English. Short sentences. Diary/margin-note voice — a person
writing while moving between projects. All copy in a design prompt is
given word for word; tools do not write copy.

**Banned words:** unleash, unlock, elevate, empower, supercharge, seamless
(except as a technical motion description in this file), journey, leverage,
delve, vibrant, cutting-edge, revolutionary, streamline (in copy),
"in today's fast-paced world".
