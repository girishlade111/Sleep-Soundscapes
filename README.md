# Sleep Soundscapes

A React component snippet for a sleep-soundscapes player: mix and play ambient noises (rain, forest, white noise) for better sleep, with an auto-stop timer and per-sound volume sliders.

## What It Does

- Plays ambient sound loops (rain, forest, etc.)
- Mix multiple sounds at once, each with its own volume slider
- Timer to auto-stop playback
- Works offline — no accounts, no cloud sync

## Contents

This repo is a **code snippet / component**, not a runnable app:

```
.
├── Sleep Soundscapes   # React component (play/pause, volume sliders, auto-stop timer)
└── README.md
```

The component uses:
- `react` hooks (`useState`, `useEffect`, `useRef`)
- shadcn/ui components (`Button`, `Card`, `Slider`)
- `lucide-react` icons (`Timer`, `Play`, `Pause`, `Volume2`)

Audio files referenced by `audioSrc` must be provided by you — drop your `.mp3`/`.wav` loops into your app and point the paths at them.

## Quick Start

1. Install the peer dependencies in your React project: `react`, `lucide-react`, and the shadcn/ui `button` / `card` / `slider` components.
2. Copy `Sleep Soundscapes` into your project (rename to `SleepSoundscapes.jsx` / `.tsx`) and fix the `/components/ui/*` import paths to your project's shadcn setup.
3. Supply audio files for each sound entry in the `Sound` type.
4. Render `<SleepSoundscapes />` in your app.

## Planned Native Tech (per original concept)

- Android: ExoPlayer · iOS: AVFoundation — if ported to a mobile app.

## License

See [LICENSE](./LICENSE).

Built by Girish Lade — https://ladestack.in
