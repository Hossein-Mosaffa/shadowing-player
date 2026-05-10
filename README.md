# Shadow Player 🎬

A single-file YouTube player built for **language shadowing** — the technique of listening to and repeating short chunks of native speech to build fluency through imitation.

No accounts. No installs. Just open the HTML file and go.

---

## What it does

Shadow Player breaks a YouTube video into small, repeatable chunks so you can listen, pause, and shadow each segment before moving on. It's designed for language learners who want to drill real spoken content — podcasts, interviews, films, anything on YouTube.

**Key features:**

- **Chunk-based playback** — split any video into segments (3–120 seconds) and navigate chunk by chunk
- **Replay button** — instantly replay the current chunk as many times as you need
- **Adjustable speed** — 0.5× to 2× playback for easier or more challenging shadowing
- **Auto-advance** — optionally move to the next chunk automatically after each one ends
- **Progress bar** — seek anywhere in the video with a click
- **Light / dark theme** — toggle to suit your environment
- **Keyboard shortcuts** — hands-free control while you shadow

---

## Keyboard shortcuts

| Key | Action |
|-----|--------|
| `Space` | Replay current chunk |
| `→` | Next chunk |
| `←` | Previous chunk |
| `R` | Cycle through playback speeds |

---

## How to use

1. Download `shadow-player.html`
2. Open it in any modern browser
3. Paste a YouTube URL and press **Load**
4. Set your chunk size (default: 10 seconds)
5. Press replay, shadow, repeat

No server required — everything runs locally in the browser.

---

## How shadowing works

Language shadowing is a method popularized by polyglots and linguists where you:

1. Listen to a short chunk of natural speech
2. Repeat it aloud, mimicking rhythm, intonation, and pronunciation as closely as possible
3. Replay and refine until it feels natural
4. Advance to the next chunk

Shadow Player is built around this loop. The chunk size, replay button, and speed control are all there to serve it.

---

## Browser support

Works in any modern browser (Chrome, Firefox, Safari, Edge). Requires an internet connection to load YouTube videos via the iframe API.

---

## Technical notes

- Single HTML file — no build step, no dependencies, no framework
- Uses the [YouTube IFrame Player API](https://developers.google.com/youtube/iframe_api_reference)
- All state is in-memory; nothing is stored or transmitted

---

## License

MIT
