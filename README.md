# Shadow Player 🎬

A single-file player built for **language shadowing** — the technique of listening to and repeating short chunks of native speech to build fluency through imitation.

No accounts. No installs. Just open the HTML file and go.

---

## What it does

Shadow Player breaks a video into small, repeatable chunks so you can listen, pause, and shadow each segment before moving on. It works with YouTube URLs and local video or audio files, and supports `.srt` subtitle files for local content.

**Key features:**

- **Chunk-based playback** — split any video into segments (3–120 seconds) and navigate chunk by chunk
- **Replay button** — instantly replay the current chunk as many times as you need
- **Adjustable speed** — 0.5× to 2× playback for easier or more challenging shadowing
- **Auto-advance** — optionally move to the next chunk automatically after each one ends
- **Progress bar** — seek anywhere in the video with a click
- **Local file support** — open video or audio files directly from your device (MP4, MKV, MOV, WebM, MP3, M4A, and more)
- **SRT subtitles** — load a `.srt` file alongside a local video for live subtitle display
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

### YouTube

1. Download `shadow-player.html` and open it in any modern browser
2. Make sure the **YouTube** tab is selected
3. Paste a YouTube URL and press **Load**
4. Set your chunk size (default: 10 seconds)
5. Press replay, shadow, repeat

### Local file

1. Switch to the **Local file** tab
2. Drop a video or audio file onto the drop zone, or click **Browse**
3. Once the video loads, click **Load .srt** to add a subtitle file (optional)
4. Set your chunk size and start shadowing

No server required — everything runs locally in the browser.

---

## Subtitles

Subtitles are supported for local files via `.srt` (and basic `.vtt`) files. To use them:

1. Load your video file first
2. A subtitle row will appear below the file picker — click **Load .srt** and choose your subtitle file
3. The current cue displays as an overlay at the bottom of the video, updating in sync with playback
4. Click ✕ to remove the subtitle file at any time

---

## How shadowing works

Language shadowing is a method popularized by polyglots and linguists where you:

1. Listen to a short chunk of natural speech
2. Repeat it aloud, mimicking rhythm, intonation, and pronunciation as closely as possible
3. Replay and refine until it feels natural
4. Advance to the next chunk

Shadow Player is built around this loop. The chunk size, replay button, speed control, and subtitle display are all there to serve it.

---

## Browser support

Works in any modern browser (Chrome, Firefox, Safari, Edge). An internet connection is required only for YouTube playback.

---

## Technical notes

- Single HTML file — no build step, no dependencies, no framework
- YouTube playback via the [YouTube IFrame Player API](https://developers.google.com/youtube/iframe_api_reference)
- Local files loaded via the browser's native `<video>` element and `URL.createObjectURL()`
- SRT parsing is done entirely in-browser — no file is uploaded anywhere
- All state is in-memory; nothing is stored or transmitted

---

## License

MIT
