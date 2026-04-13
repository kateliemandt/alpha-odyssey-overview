# Alpha Odyssey — Overview

A single-page grid of every workshop and physical challenge for Alpha Odyssey Summer 2026, plus all 53 mastery side quests. Nine weeks, four age levels, every card collapsible for a quick scan.

**Sister site:** [alpha-odyssey-briefs](https://github.com/kateliemandt/alpha-odyssey-briefs) — same content, long-form editorial layout, one brief per screen.

## Structure

```
index.html        — shell, CSS, renderer
data/
  week1.js … week9.js   — per-week workshop + physical-challenge data
  sidequests.js         — all 53 mastery side quests
```

Each `weekN.js` appends to `window.ODYSSEY.weeks`; `sidequests.js` populates `window.ODYSSEY.sideQuests`. The renderer normalizes minor format drift between files and paints the full site.

## Running locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Aesthetic

Editorial-literary — Young Serif display, Cardo body, JetBrains Mono UI — on midnight navy, parchment cream, hammered gold. Wine-red accents for the Friday pass/fail stakes. Parchment grain overlay. No Inter, no purple gradients.
