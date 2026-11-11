# Automatic Airsoft Video Machine

Heart rate, GPS route, shots and story cards on your airsoft helmet-cam videos — a live HUD, a multitrack editor,
cards and titles, and a finished movie out.

**Download page:** https://uusitalo.github.io/airsoft-video-machine/

| | Latest | Needs |
|---|---|---|
| Windows | [Releases](../../releases) (tags `windows-v…`) | Windows 10/11 64-bit, nothing to install |
| Mac | [Releases](../../releases) (tags `mac-v…`) | macOS 14+, Apple silicon |
| Linux | [Releases](../../releases) (tags `linux-v…`) | 64-bit Linux, FFmpeg (`sudo apt install ffmpeg`) |

Projects are the same format on both: a project made on a Mac opens on Windows and the other way round.

<!-- avm-previews:start -->
## Example

Made by the app itself (AVM Windows and Linux 1.6.88 / AVM Swift 1.6.88) from one short test clip, with a made-up route and heart rate.

[![The example film](docs/previews/example-game.jpg)](docs/previews/example-game.mp4)

[▶ The example film (MP4, 35 s)](docs/previews/example-game.mp4)

**Airsoft HUD:** heart rate, time, distance and shots, the satellite map with the field you drew on the Map page, your team's badge turning in the corner (its 3D model when the team has one) and a face that reacts to the game - your own face pictures, or this drawn one. When you are hit, the heartbeat flatlines.

![Airsoft HUD](docs/previews/airsoft-hud.webp)

| Briefing map card (the plan from the Map page) | Gun teardown card (what was wrong, and the fix) |
|:---:|:---:|
| ![Briefing map](docs/previews/briefing-map.webp) | ![Gun teardown](docs/previews/gun-teardown.webp) |

**Drawn cards** (1.6.88): a chronograph reading with the BB's flight, how an HPA gun works, and your kit laid out piece by piece - set the numbers and the gun on the card.

| Chrono and the BB's flight | HPA: how the air gets to the BB |
|:---:|:---:|
| ![Chrono card](docs/previews/card-chrono.jpg) | ![HPA card](docs/previews/card-hpa.jpg) |

![Kit card](docs/previews/card-kit.jpg)

[▶ The three cards as a video (MP4, 27 s)](docs/previews/new-cards.mp4)

**Game events and subtitles:** mission updates, objectives, weapon changes and reloads as they happen, your shots counted from the magazine, and what was said as subtitles (also saved as an .srt file with the movie). Every game style draws them its own way.

![Game events and subtitles](docs/previews/events-subtitles.webp)

## The app

| Timeline | Storyboard |
|:---:|:---:|
| ![Timeline](docs/previews/app-timeline.jpg) | ![Storyboard](docs/previews/app-storyboard.jpg) |
| **Map page: plan the field** | **Edit page: one clip, its cut and its shots** |
| ![Map page](docs/previews/app-map.jpg) | ![Edit page](docs/previews/app-edit.jpg) |

**Cards on the timeline** (here the gun teardown card, with its gun and problem pickers):

![A card on the timeline](docs/previews/app-card.jpg)

## Effects preview

Made by the app itself (AVM Windows and Linux 0.29.1 / AVM Swift 1.6.59). Each logo transition shows your team logo in the middle
of the cut. Pick them on the Timeline: select a piece › Transition.

| Logo on fire | Burning logo (ash & embers) |
|:---:|:---:|
| ![Logo on fire](docs/previews/logo-on-fire.webp) | ![Burning logo](docs/previews/burning-logo.webp) |
| **Smoke logo (smoke from the left)** | **Fire & smoke logo** |
| ![Smoke logo](docs/previews/smoke-logo.webp) | ![Fire and smoke logo](docs/previews/fire-and-smoke-logo.webp) |

**Radio call card:** the clip's sound becomes walkie-talkie sound with clicks and static, a walkie-talkie slides in, radio-style subtitles and a static burst at each call.

![Radio call](docs/previews/radio-call.webp)

**Friends' cameras (Video 2):** picture-in-picture, side by side, and switching to your friend's camera with a transition (one test clip plays as both cameras here).

![Friend views](docs/previews/friend-views.webp)

**Friends on the HUD:** each friend's heart rate and how far they are from you, and their dots on the map - from their own route / heart-rate files (GPX, TCX, a Health export). When you or a friend is hit, the heartbeat flatlines (a heart monitor with HIT and a long beep; their row and map dot go grey). Shown here with made-up example routes.

![Friends on the HUD](docs/previews/friends-hud.webp)

[▶ The friends preview as a video (MP4)](docs/previews/friends-preview.mp4)

**Transitions:** Luma melt, Lens flare wipe, Prism split, Warp zoom, Film roll, Cube turn, Water ripple

![Transitions](docs/previews/transitions.webp)

**Camera effects:** Anamorphic flares, Sun rays, Heat haze, Light leaks

![Camera effects](docs/previews/camera-effects.webp)

[▶ The whole preview as a video (MP4)](docs/previews/effects-preview.mp4)
<!-- avm-previews:end -->

## Starting it
- **Windows:** unzip, double-click `AVM.exe`. "Windows protected your PC" → More info → Run anyway (not signed).
- **Mac:** unzip, drag *AVM Swift* to Applications, right-click › Open the first time (not signed by Apple).
  If it says "damaged": `xattr -dr com.apple.quarantine "/Applications/AVM Swift.app"`

## Included in the Windows build
FFmpeg (GPL, gyan.dev builds — licence in the `ffmpeg` folder), a person-finder model from torchvision (BSD 3-Clause),
ONNX Runtime (MIT), fonts Inter, Lora, Share Tech Mono, Orbitron, Rajdhani (SIL Open Font License).
