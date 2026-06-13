# 🎰 365 Agents Roulette

A delightful slot-machine-style randomiser that picks one agent from the [365 Custom Agents](https://app.notion.com/p/44b823a526424642945d362fb6c554f6) Notion database. Press **SPIN**, watch the names whirr past, and discover your next agent to build or use.

## Features

- **Slot-machine reel** with smooth acceleration, blur, and settle-back animation
- **Result card** showing name, day, pillar, category, status, description, tags, and tools
- **Copy prompt** button for one-click prompt extraction
- **Pillar filters** to narrow the roulette to specific pillars
- **Confetti burst** on every spin landing
- **Keyboard support** — press Space or Enter to spin
- **Fully offline** — all 365 agents are embedded in the single HTML file
- **Zero dependencies** — vanilla HTML/CSS/JS, no frameworks, no CDNs

## Usage

Open `index.html` in any modern browser (Chrome, Safari, Firefox). That's it.

Or visit the live site:https://singular-palmier-4baa63.netlify.app/

## Refreshing data

To update the embedded agent data from Notion:

1. Regenerate `index.html` from the 365 Custom Agents database
2. Commit and push to `main`
3. Vercel auto-deploys on push

The footer shows "Data as of [date]" so staleness is always visible.

## Technical notes

- **Single file**: everything lives in `index.html` — CSS, JS, and data
- **~176 KB** total size (well under the 400 KB soft budget)
- **No network requests** at runtime — verify in DevTools
- Respects `prefers-reduced-motion` for accessibility
- WCAG AA contrast, visible focus states, `aria-live` on the result card

---

Built by [Nasri](https://nasrinasir.com).
