# Hippocorn Run — Hustle Commons 404 page

A quirky, playable 404 page for [Hustle Commons](https://hustlecommons.com): a Super Mario Bros.–style
platformer starring the **Hippocorn** mascot. If someone lands on a page that doesn't exist, they can
gallop the Hippocorn home — hopping rainbow pipes, bopping glitch bugs, and grabbing rainbow coins —
and reach the flag to find their way back.

Everything lives in a **single self-contained file**: [`404.html`](404.html).
No build step, no dependencies, no external requests.

## Features

- 🎮 **Side-scrolling platformer** — run, variable-height jump, stomp enemies, collect coins, reach the flag
- ⌨️ **Keyboard + 📱 touch** — arrows/WASD + Space on desktop; on-screen ◀ ▶ / JUMP buttons on phones
- 🎵 **Chiptune music + SFX** — synthesized live with the Web Audio API (no audio files); mute toggle included
- 🎨 **On-brand** — real Hustle Commons palette and the licensed **Aeonik** + **GT America Mono** fonts, embedded
- ♿ **Robust** — fixed 60 Hz timestep (consistent on 60/120/144 Hz displays), responsive desktop/tablet/mobile,
  graceful audio autoplay handling

## Controls

| Action | Keyboard | Touch |
| --- | --- | --- |
| Move | ◀ ▶ / A D | on-screen ◀ ▶ |
| Jump | Space / ↑ / W | JUMP button |

## Deploying as a 404 page

It's a static file — point your host's 404/not-found route at it. Examples:

- **Netlify:** drop `404.html` in your publish directory (served automatically — no config needed).
- **Vercel:** add a `404.html` (or a Next.js `not-found` page that serves this markup).
- **Cloudflare Pages / S3 / most static hosts:** set the custom error-document / 404 path to this file.

## Notes

- **Mascot art:** the game ships with a built-in pixel Hippocorn. To use the official sprite, drop a
  `hippocorn.png` next to the HTML file — it's picked up automatically.
- **Fonts:** Aeonik and GT America Mono are embedded (base64). These are licensed fonts; usage here is
  covered under the same web-font license as hustlecommons.com.

Built with [Claude Code](https://claude.com/claude-code).
