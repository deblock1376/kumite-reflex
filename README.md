# Kumite Reflex

Read → process → react drills for karate point fighters. Prop a phone, tablet or laptop at head height 2–3 m away, take your stance, and move the instant the cue lands.

## Drill ladder

| Level | Drill | Trains |
|---|---|---|
| 1 | Footwork | Simple reaction: one arrow, one move |
| 2 | Technique call | Choice reaction: numbers call techniques, combos at higher levels |
| 3 | Aka · Ao | Go/No-Go: your belt color follows, the other color mirrors, YAME freezes |
| 4 | Read the opponent | Read a body tell and pick the counter; feints mean hold |

## Camera timing

Turn on **Camera timing** and stand the device where the front camera sees your whole body from 2–3 m away. The app compares each video frame with the one before it on a small grayscale copy. It sets a threshold from the ~0.8 s of stance just before each cue, then logs your reaction time as the first moment motion clears that threshold on two frames in a row. Moves under 100 ms count as anticipation, and any movement on a No-Go cue counts as a fault. Times include roughly 30–80 ms of camera delay, so compare sessions with each other. All processing happens on the device. No video is recorded or sent anywhere.

## Install on iPhone

Open the site in Safari → Share → **Add to Home Screen**. It then launches full screen and works offline after the first load.

## Development

It's a single static page with no build step.

```sh
python3 -m http.server 8000   # then open http://localhost:8000
```

When you change `index.html`, bump `VERSION` in `sw.js` so installed copies pick up the update.
