# ⚡ Kamehameha App

A real-time browser app that lets you charge and fire Goku's Kamehameha using your webcam and hand gestures — no installation required.

![Kamehameha](https://img.shields.io/badge/powered%20by-MediaPipe%20Hands-blue) ![HTML](https://img.shields.io/badge/built%20with-HTML%20%2F%20JS-yellow) ![No Install](https://img.shields.io/badge/no%20install-just%20open%20in%20browser-green)

---

## 🎮 How It Works

| Step | Gesture | Effect |
|------|---------|--------|
| 1 | Show both hands to the camera | App detects your hands |
| 2 | Bring both hands close together | Energy orb starts charging |
| 3 | Hold position to reach 100% charge | Orb grows with electric arcs |
| 4 | Quickly thrust both hands upward | **KAMEHAMEHA fires!** ⚡ |

---

## 🚀 Getting Started

No installation, no dependencies, no server needed.

1. Download `kamehameha.html`
2. Open it in **Google Chrome** or **Microsoft Edge**
3. Click **▶ Start Camera** and allow camera access
4. Strike your pose!

> **Note:** Firefox has limited support for the MediaPipe camera utils library. Chrome or Edge is recommended for best experience.

---

## 🛠 Tech Stack

- **[MediaPipe Hands](https://google.github.io/mediapipe/solutions/hands)** — Real-time hand landmark detection (21 keypoints per hand) running fully in-browser via WebAssembly
- **HTML5 Canvas** — All visual effects (energy orb, beam, particles) rendered frame-by-frame
- **Vanilla JavaScript** — Zero frameworks, zero build tools
- **CSS animations** — UI polish and aura effects

---

## ✨ Features

- 🙌 Detects up to 2 hands simultaneously in real-time
- 🔵 Dynamic energy orb that grows as you charge
- ⚡ Electric arc animations around the orb
- 💥 Full-screen beam with particle explosion at the tip
- 📊 Power charge bar with live percentage
- 🌊 Screen flash on firing
- 🪞 Mirrored camera for natural feel
- 📱 Works on any device with a webcam

---

## 📁 Project Structure

```
kamehameha.html   # Entire app in a single self-contained file
README.md
```

---

## 🔧 Customization

Open `kamehameha.html` in any text editor to tweak:

| Variable | Location | What it controls |
|----------|----------|-----------------|
| `W * 0.3` | `loop()` | Max hand distance to trigger charging |
| `H * 0.06` | `loop()` | Thrust sensitivity to fire |
| `firingTimer = 100` | `loop()` | How long the beam lasts (frames) |
| `beamProgress + 0.035` | `drawBeam()` | Beam travel speed |
| `power > 0.25` | `loop()` | Minimum charge % needed to fire |

---

## 🌐 Browser Support

| Browser | Status |
|---------|--------|
| Chrome 90+ | ✅ Full support |
| Edge 90+ | ✅ Full support |
| Firefox | ⚠️ Camera utils may not work |
| Safari | ⚠️ Limited WebAssembly support |

---

## 📜 License

MIT — free to use, modify, and share.

---

> *"Kame... Hame... HA!"* — Son Goku
