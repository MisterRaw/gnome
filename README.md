# GNOME

**Generative Nexus for Open Musical Exploration**

A browser-based sound art studio for layering generative textures with field recordings. Built by Alan Raw as part of **Littoral Arts**, for the Salt & Seeds installation and the Write Your Own Future workshop.

## Origins

GNOME grew from **RAW SAS-1** (Sound Art Studio), which I started in May 2026 after a Make Happen Institute Learning Lab session. That first version was deliberately basic: nine generator layers, two sample players and a recorder.

Now that my MA Creative Practice at the Make Happen Institute has begun, I'm developing it in the wild. That means adding more sample players, a bank of my North Sea field recordings, and whatever else proves useful through feedback and use. Every change from here on is logged in the changelog below.

## Design notes

- **Black and red, on purpose.** The colour scheme preserves night vision, so GNOME can be operated backstage and in darkened installation spaces without dazzling the operator.
- **Runs in a browser.** No install. Works on desktop and mobile, including iOS.
- **Built with [Tone.js](https://tonejs.github.io/).**

## Adding field recordings to the sound bank

1. Put audio files in the `sounds/` folder (MP3 keeps them small; WAV works too).
2. List them in `sounds/bank.json`:

```json
[
  { "name": "Tide on shingle", "file": "sounds/tide-on-shingle.mp3" },
  { "name": "Harbour rigging", "file": "sounds/harbour-rigging.mp3" }
]
```

3. Push to GitHub. Each sample player now shows a **Bank** menu with those recordings. While the list is empty, the menu stays hidden and people can still load their own files.

## Changelog

### v0.2: GNOME (started 29 September 2026, MA Action 1)

- Renamed from RAW SAS-1 to GNOME
- Four sample players (was two)
- Sound bank: preloaded field recordings selectable from each player
- Feedback prompt for the MA cohort

### v0.1: RAW SAS-1 (May 2026)

- Nine generator layers, two sample players, stereo panning, BPM detection, recorder
- Built after a Make Happen Learning Lab session
