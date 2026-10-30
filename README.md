# Bloodline

A generative, story-driven visual for a single song, built in one HTML file with a canvas and no dependencies.

**Live:** https://mrsaad.github.io/song-viz/

## Controls

| Input | Action |
| --- | --- |
| Click / Space | Play / pause |
| ← / → | Skip 10 s |
| Drag the timeline | Scrub |
| H | Show / hide the key legend |

## Story

The visuals follow the song's three verses and hook:

- **Intro** – a faint spinning record and a rising moon
- **Verse 1** – a childhood night: a moon in a window, two small lights, a drunken haze, a cracked room
- **Chorus** – the record becomes a blood-red heart pumping along veins; a searchlight finds an empty ring
- **Verse 2** – fatherhood: a new light drifts away and turns cold as the cycle repeats
- **Verse 3** – smoke, an empty house drawn in line, a light that never arrives; the record cracks and skips
- **Outro** – the search ends where it began, the child under the moon

## How it works

`index.html` builds the page, audio player and visuals itself. Beat timings and loudness/onset envelopes were analysed from `new.mp3` ahead of time (~99.4 bpm) and are embedded in the script, so the visuals stay in sync without any audio analysis at runtime.

## Run locally

Keep `new.mp3` next to `index.html` and serve the folder:

```bash
python3 -m http.server
```

Then open http://localhost:8000.
