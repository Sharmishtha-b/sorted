# Sorted

A daily ranking puzzle. Every day you get one category and five entries, like *Planets, by diameter* or *Movies, by release year*. Put them in the right order in three tries.

**[Play it here →](https://YOUR-USERNAME.github.io/sorted/)**

## How to play

- Tap two blocks to swap them (or drag one onto another), then hit **Lock in**.
- After each try, every block tells you something:
  - ✓ green: right place
  - ▲ coral: belongs higher
  - ▼ coral: belongs lower
- It never tells you *how far* to move. That part is logic.
- Everyone gets the same puzzle each day. Finish it and share your result without spoilers:

```
Sorted #001 · 2/3
Planets, by diameter
🔼🟩🔽🔽🔼
🟩🟩🟩🟩🟩
```

## Features

- Real-time 3D board built with Three.js: glossy blocks, gold/silver/bronze medals, swap and flip animations, confetti on a win
- New puzzle every day at midnight, picked deterministically from the date
- Stats saved in the browser: games played, win %, current and best streak, and a distribution of tries per win
- Bonus rounds for when one puzzle a day isn't enough
- Works on desktop and mobile; keyboard players can press two number keys (1–5) to swap ranks

## Tech

A single `index.html` file: vanilla JavaScript, CSS, and [Three.js r128](https://threejs.org/) from a CDN. No build step, no backend. Progress and stats live in `localStorage`.

## Data

The 20 lists use well-established figures. Values marked `~` are approximate (populations, weights, lengths and the like vary by source and year). Spot a mistake? Open an issue.

## Built with AI

I built this with Claude (Anthropic) as a pair programmer: I came up with the direction and made the design and gameplay calls, and iterated on the look and rules until it felt right.

## License

MIT
