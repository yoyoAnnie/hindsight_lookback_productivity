# 05 - Design System

This doc holds values, not loose words. A design prompt, a spec, or a
build must use the numbers in this doc. And the values go in the first
prompt of each session, in full. A tool does not read this file on its
own. See `07`.

## Direction in one line

Old painting warmth, like a Renaissance work, with the clear layout of
Notion. Sites we studied: Contra Labs for calm layout and cards, and
Shopify Editions Winter '26 for scroll motion and for collage of old
art, pixel art, and a new object in one frame. Motion comes first.
Layout comes second.

## Colors

| Token | Hex | Use |
| --- | --- | --- |
| paper | `#F6F1E7` | page background |
| surface | `#FFFEF9` | cards and panels |
| ink | `#211D18` | main text |
| muted | `#6F675A` | second text |
| line | `#E3DCCB` | 1px borders |
| gold | `#B9922E` | rules, numbers, and underlines only. Under 5% of a screen |
| hand | `#C17A3A` | Hand mode color: dot, tag, icon |
| brain | `#4F7D78` | Brain mode color |
| eye | `#6C4CFF` | Eye mode color. Also the pixel and future accent |
| dark | `#1E1B16` | dark section background. Text on it: paper |

No color fades. No glass blur. No stock photos. A paper grain layer sits
on painted areas only, at 4%.

## Type

- Display font: **Source Serif 4**. Use italic for one word per
  headline, and no more.
- UI and body font: **Inter**. Labels and times: a mono font, 11px,
  all caps, letter spacing 0.08em.
- Hero headline: 76px, line height 0.98, letter spacing -0.03em.
- Section headlines: 48px, line height 1.05. Card titles: 22px.
  Body: 17px, line height 1.55. Small text: 14px.
- Phone: hero headline 44px. Body stays the same.

## Layout and parts

- Max width 1200px. Side gaps 24px. Space grid 8px. Top and bottom
  space per section 128px. On phone: 72px.
- Radius: cards 12px, UI panels 8px, buttons 999px (pill).
- Shadows: none. One case is the app mock: `0 24px 60px rgba(33,29,24,0.12)`.
- Buttons: main button is ink background with paper text. The second
  button is text with an underline.
- Stream cards: a mode color dot, a mono time stamp, a title, and one
  line of text.
- Mode icons: plain line icons for a hand, a brain, and an eye. Draw
  them once. Use them at 16px and 24px only.

## Collage rule for images

One image can mix three time layers, but it must look like one image:

- base layer: a Renaissance oil painting
- mid layer: pixel art, sharp, at 4 to 6 times its size, no blur
- top layer: one new object, like a laptop that shows the app

All layers share one light source. Each new object casts a soft shadow.
A grain layer goes on top of the full image. Painting crops sit in a
frame with a paper mat and an 8px offset border. Or they sit as a taped
piece in the scrapbook sections.

## Motion values

Motion is set here in numbers. Do not leave it to words like "fancy"
or "smooth" in a prompt.

- Ease for all UI motion: `cubic-bezier(0.22, 1, 0.36, 1)`.
- Build stack for the landing page: Lenis for smooth scroll (time 1.2,
  lerp 0.09), tied to GSAP ScrollTrigger. All scroll motion is tied to
  scroll position. The user can scroll back and the motion runs back.
  No one-time pop-ins. No hard cuts between sections.
- On load: the hero painting scales from 1.08 to 1.00 in 1200ms.
  Headline lines rise from behind a mask, 700ms each, 80ms apart.
- On scroll: section content rises 24px in 700ms as it comes in.
  Parallax speeds: painting 0.3x, main content 1.0x, float cards 1.3x.
- Pinned scenes, if the tool can do them: pin one chapter for +150%
  scroll length. Its layers change while it is pinned. The background
  color shifts step by step from one section to the next.
- Stream filter (All / Hand / Brain / Eye): cards move to new spots
  with a 450ms layout motion. No jump cuts.
- Hover: a card lifts 2px in 300ms. A painting panel cross-fades to
  its pixel form in 300ms, at scale 1.02.
- Animate `transform` and `opacity` only. No layout shift.
- If the user set reduced motion in their system: no parallax, no
  pins. Fades only.

## The Garden: colors and motion

The Garden is a calm space next to the work screens. Full spec: `11`.

- Plots are round-corner squares, radius 16px, on paper. Grid gap 10px.
  A thin fence line wraps each month page.
- Petal colors: the three mode colors, gold, and one soft pink `#E8A0A8`.
- Plant lines look hand drawn: 2px, a bit rough. No clean shape icons.
- Garden motion is slow on purpose. A new plant draws in about 1200ms.
  Idle sway is 1 degree each way, 6 seconds per cycle. It stops if the
  user set reduced motion.
- No numbers on the Garden screen. No counts, no percent, no streak.
  The picture is the measure.
- Nothing in the Garden wilts, dies, or runs out. Not in the art, and
  not in the words.

## Copy

Set all product copy word for word in the design prompt. The tool
does not write copy.

**Banned words in product copy:** unleash, unlock, elevate, empower,
supercharge, journey, leverage, delve, vibrant, cutting-edge,
revolutionary, streamline, and "in today's fast-paced world".
