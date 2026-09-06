# 🎓 How to Adult

A flip-card conversation game: flip a card, ask a teenager the real "how does adulthood actually work" question underneath, and grade how their answer held up.

Built as a one-file browser game — no build step, no dependencies, no install. Just open it and play.

**🎮 Play it:** https://caseyflinn.github.io/how-to-adult/

**Repo:** https://github.com/caseyflinn/how-to-adult

![Vanilla JS](https://img.shields.io/badge/JavaScript-vanilla-yellow)
![No build step](https://img.shields.io/badge/build-none-brightgreen)
![Single file](https://img.shields.io/badge/single--file-html-blue)

---

## What it is

A board of exam-card-styled tiles, each hiding a question about money, work, civic life, accountability, or just growing up. Flip a card, read the question out loud, and let a teenager answer it — no studying, no "right" answer key. Once they've answered, you decide how it landed: **Solid** if it holds up, **Sus** if it doesn't. A stamp locks that verdict onto the card, and a running tally at the top tracks the score across the whole round.

## How to play

1. Flip a card to reveal its question.
2. Ask it out loud and let the teenager answer.
3. Judge the answer — tap **Solid** if it's convincing, **Sus** if it isn't.
4. A stamp locks over the card. Tap the **×** on the stamp to clear it and re-grade.
5. Watch the **Solid / Sus** counters at the top track the round.
6. Hit **Reset Board** to clear every grade and start fresh.

### The categories

| Code | Category                      |
| ---- | ------------------------------ |
| ACC  | Accountability & Consequences  |
| ADU  | Becoming an Adult              |
| CIV  | Civic Life                     |
| SOC  | Social Rules                   |
| PER  | Perspective                    |

## Controls

| Action              | Input                          |
| ------------------- | ------------------------------- |
| Flip a card          | Click / tap the card            |
| Grade the answer     | Click **Sus** or **Solid**      |
| Change a grade       | Click the other button anytime  |
| Clear a grade         | Click the **×** on the stamp    |
| Start a new round     | Click **Reset Board**           |

## Features

- **Sticky scoreboard** — the Solid/Sus tally stays pinned to the top as the board scrolls.
- **Persistent grades** — verdicts save to `localStorage` and survive a refresh.
- **Re-gradable stamps** — the Sus/Solid verdict is a bold lightbox stamp over the card, changeable or clearable anytime.
- **Landscape board** — wide cards, capped at three per row, reflowing down to one on mobile.
- **Light/dark aware** — theme colors follow the system preference automatically.
- **Editable question bank** — every question lives in one JS array in `index.html`, easy to add, remove, or re-word.

## Running it

No server or build required.

```bash
git clone https://github.com/caseyflinn/how-to-adult.git
cd how-to-adult

# Just open the file in any modern browser:
open index.html       # macOS
start index.html      # Windows
xdg-open index.html   # Linux
```

Or drag the file onto a browser tab.

### GitHub Pages

This repo is set up to be served directly:

1. `index.html` already sits at the repo root, so no renaming needed.
2. In **Settings ⚙ Pages**, set the source to your default branch (root).
3. Once it builds, play at **https://caseyflinn.github.io/how-to-adult/**.

## Tech

- **Vanilla JavaScript** — zero libraries, zero build tooling.
- **CSS custom properties** for theming, with automatic light/dark mode support.
- **Google Fonts** — Big Shoulders Display + IBM Plex Sans / Mono.
- **`localStorage`** to save grades between sessions.

## Project structure

```
how-to-adult/
  index.html    # the entire game (markup, styles, and game code)
  README.md     # this file
```

## Credits

- Design & code: **Casey Flinn**

## License

© 2026 Casey Flinn. All rights reserved.

> Swap this section for an open-source license (e.g. MIT) if you'd like others to reuse the code.
