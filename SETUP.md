# 🌆 Profile README — design system notes

This repo renders on [github.com/SpyrosTheBoss](https://github.com/SpyrosTheBoss) (special profile repo).

## Layout
- `README.md` — the page. Sections: HERO → 01 IDENTITY → 02 ARSENAL → 03 LIVE TELEMETRY → 04 HOLLOW ZERO → 05 UPLINK.
- `assets/*.svg` — **hand-built animated SVGs** (pure CSS keyframes, no JS, self-contained — they animate natively on GitHub):
  - `hero.svg` — glitch title, scrolling hazard tape, perspective grid, scanline
  - `terminal.svg` — typed dossier with staggered line reveal + blinking cursor
  - `agent-stats.svg` — animated skill bars with rank chips + shimmer
  - `training.svg` — fake live ML training log (cycling loss, wobbling GPU bar)
  - `tv-buddy.svg` — PX-07, floating TV-bot mascot (blinks!)
  - `h-0*.svg` — section headers · `divider*.svg` — animated separators
- `.github/workflows/snake.yml` — regenerates the contribution snake every 12h → `output` branch.

## Palette
`#F72585` magenta · `#7B2FF7`/`#A957FF` purple · `#00E5FF` cyan · `#FF2E63` red · `#F9F871` acid · `#0D0221`/`#0F0526` void

## Editing rules of thumb
- SVG text uses only system font stacks (`ui-monospace…`, `Segoe UI…`) — external fonts don't load inside `<img>`-embedded SVGs.
- No external refs inside SVGs; GitHub's camo proxy serves them, CSS animations run as-is.
- Keep every asset background-solid (`#0D0221`+) so light-mode GitHub doesn't wash it out.
- Widgets (stats/streak/graph/trophies) are external services themed via URL params — bg is `0F0526` to match panels.

## Still open (optional)
- UPLINK: real LinkedIn / X / Discord hrefs (placeholders now); email badge parked in a comment.
- `assets/jane-doe.png` art slot in section 04 (commented out until an image exists).
