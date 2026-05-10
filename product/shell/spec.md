# Shell Specification

Single-page scroll experience. No navigation chrome. The entire site IS the journey.

## Layout

- **Single column**, max-width ~960px on desktop, full-width on mobile
- **Vertical line** rendered as SVG, fixed left at ~80px on desktop, top-anchored on mobile (becomes a horizontal progress bar)
- **Section padding** generous — ~25vh top/bottom — to give each beat room to breathe
- **Sticky elements** — none (the line scrolls with content; only its draw progress is animated)

## Persistent UI

- **Top-right corner** — small monospace `vikas.followtherabbit.studio` link + scroll-progress percentage (e.g. `[42%]`). No nav menu — the page IS the nav.
- **Bottom-right** — discreet "back to top" arrow, fades in after first scroll
- **Footer** — minimal: GitHub @vimo33 + email + "© 2026 Bildspur · Follow The Rabbit Studio"

## Aesthetic Notes

- **Background:** stone-950 with a subtle warm tint (CSS `oklch()` with hue ~70deg, very low chroma)
- **Foreground:** stone-100 with reduced opacity for body, full opacity for headings
- **Accent (primary):** orange-500 — used for headings, key callouts, active timeline node
- **Accent (secondary):** cyan-400 — used for monospace, code, technical labels, year markers
- **Borders/lines:** stone-100 at 8% opacity
- **Section breaks:** thin orange-500 line at 30% opacity, or just generous whitespace

## Motion

- **Page enter:** subtle fade + slight Y translation (~12px), 600ms ease-out
- **Scroll-progress:** vertical line draws via `clipPath` driven by `scrollYProgress`
- **Section enter:** intersection-observer triggered, stagger children
- **Hover:** project cards lift slightly + accent border glow

## Accessibility

- Reduced-motion preference: animations collapse to fades only
- Keyboard navigation: every project card is tabbable; year markers act as scroll anchors
- Color contrast: all text passes WCAG AA against the dark background
