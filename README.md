# Automatic Airsoft Video Machine

Heart rate, GPS route, shots and story cards on your airsoft helmet-cam videos — a live HUD, a multitrack editor,
cards and titles, and a finished movie out.

**Download page:** https://uusitalo.github.io/airsoft-video-machine/

| | Latest | Needs |
|---|---|---|
| Windows | [Releases](../../releases) (tags `windows-v…`) | Windows 10/11 64-bit, nothing to install |
| Mac | [Releases](../../releases) (tags `mac-v…`) | macOS 14+, Apple silicon |

Projects are the same format on both: a project made on a Mac opens on Windows and the other way round.

## Starting it
- **Windows:** unzip, double-click `AVM.exe`. "Windows protected your PC" → More info → Run anyway (not signed).
- **Mac:** unzip, drag *AVM Swift* to Applications, right-click › Open the first time (not signed by Apple).
  If it says "damaged": `xattr -dr com.apple.quarantine "/Applications/AVM Swift.app"`

## Included in the Windows build
FFmpeg (GPL, gyan.dev builds — licence in the `ffmpeg` folder), a person-finder model from torchvision (BSD 3-Clause),
ONNX Runtime (MIT), fonts Inter, Lora, Share Tech Mono, Orbitron, Rajdhani (SIL Open Font License).
