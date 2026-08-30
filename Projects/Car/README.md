# Car Showcase — Studio Render (Blender / Cycles)

A cinematic **studio car showcase animation** — an original concept sedan modeled and rendered in Blender using **Cycles**, presented on a turntable-style orbiting camera, in the style of a product/automotive commercial.

---

## 🎬 Overview

| | |
|---|---|
| **Tool** | Blender, Cycles render engine |
| **Scene** | Single scene, single camera |
| **Frame Range** | 1–120 |
| **FPS** | 24 |
| **Duration** | ~5 sec |
| **Resolution** | 1920×1080 |
| **Audio** | None |

## 🚗 What's in the Scene

- **Car model** — a full sedan build (body shell, 4 detailed wheels/rims, mirror, interior fill), finished in a glossy black studio paint material
- **Studio environment** — a curved cyclorama-style backdrop with a patterned feature wall (crackle/hex tile pattern) behind a neutral studio floor
- **Studio lighting** — a professional 3-point+ setup (top softbox, side left, side right, and a highlight sun) for the classic glossy automotive-photography look and clean paint reflections
- **Orbiting camera** — the camera follows a Bezier circle path around the car for a smooth 360°-style reveal, with subtle organic shake layered on top for a more handheld-commercial feel rather than a static turntable

## ⚙️ Technical Details

- **Render engine:** Cycles
- **Objects:** 27 (car body, 4 wheels, mirror, interior, backdrop planes, cube, camera, curve path, 8 lights, empties)
- **Materials:** 46
- **Camera rig:** `Follow Path` constraint (Bezier circle) + additional location/rotation constraints for subtle handheld-style motion
- **Lighting:** softbox + dual side lights + highlight sun, plus supplementary scene lights

## ▶️ How to Open / Render

1. Open `Car.blend` in Blender (Cycles-capable GPU recommended).
2. Scene runs frames **1–120** at 24fps (~5s) — the camera completes its orbit + shake pass across the full range.
3. `Render → Render Animation` to reproduce the sequence, or scrub the timeline and `Render → Render Image` for a single still (great for a hero/cover shot).
4. No audio track — this is a silent showcase piece; add music/SFX in post if desired.

## 📁 Repo Contents

```
.
├── Car.blend         # Main Blender project file
├── Final.mkv           # Rendered animation (frames 1–120)
├── frames/              # Rendered image sequence
└── README.md
```


Made with 🧡 in Blender.
