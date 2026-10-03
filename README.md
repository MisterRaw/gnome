# GNOME

**Generative Nexus for Open Musical Exploration**

Gnome is my browser-based sound art studio for layering generative textures with field recordings. Built by Loosetriggers (Alan Raw) as part of my Creative Practice MA Project.

## Origins

GNOME grew from RAW SAS-1 (Sound Art Studio One), which I started in 2026 after a Make Happen Institute Learning Lab session inspired me to experiment. That first version was very basic: nine generator layers, a sample player and a recorder.

Now that my MA Creative Practice at the Make Happen Institute has begun, I'm developing this software in the wild. That means adding more elements based on feedback and user experience. Including early suggestions from beta testers for more sample players, a DJ mixer style volume slider and speed section (which I have just added), a bank of my field recordings preloaded, and whatever else proves useful through further feedback and use. Changes will be logged in the changelog below.

## Design notes

- **Black and red, on purpose.** The colour scheme preserves night vision, so GNOME can be operated backstage and in darkened installation spaces without dazzling the operator.
- **Runs in a browser.** No install, so it is easy to deploy on any machine instantly. Works on desktop and mobile, including iOS.

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

### v0.2: GNOME (Pushed to GitHub Pages October 3rd 2026, MA Action 1)

- Added minor chords.
- Pushed with sharable link for feedback.

### v0.2: GNOME (started 29 September 2026, MA Action 1)

- Renamed from RAW SAS-1 to GNOME
- Four sample players now (was one, then made it two after beta feedback)
- Sound bank: preloading field recordings selectable from each player from my own collection.
- Feedback prompt for the MA cohort on the player page.

### v0.1: RAW SAS-1 (May 2026)

- Added speed control and volume sliders like a DJ mixer.
- Added stereo panning, BPM detection.
- Added recorder.
- Nine generator layers, sample player.
- Built after a Make Happen Learning Lab session, as an experimental work station.
