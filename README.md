# Automatic Airsoft Video Machine

Heart rate, GPS route, shots and story cards on your airsoft helmet-cam videos — a live HUD, a multitrack editor,
cards and titles, and a finished movie out.

**Download page:** https://uusitalo.github.io/airsoft-video-machine/

| | Latest | Needs |
|---|---|---|
| Windows | [Releases](../../releases) (tags `windows-v…`) | Windows 10/11 64-bit, nothing to install |
| Mac | [Releases](../../releases) (tags `mac-v…`) | macOS 14+, Apple silicon |

Projects are the same format on both: a project made on a Mac opens on Windows and the other way round.

<!-- avm-previews:start -->
## Effects preview

Made by the app itself (AVM Windows 0.28.0 / AVM Swift 1.6.57). Each logo transition shows your team logo in the middle
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

**Friends on the HUD:** each friend's heart rate and how far they are from you, and their dots on the map - from their own route / heart-rate files (GPX, TCX, a Health export). Shown here with made-up example routes.

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
