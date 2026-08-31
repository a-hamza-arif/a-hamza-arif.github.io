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
- **Studio environment** — a curved cyclorama-style backdrop with a patterned feature wall behind a neutral studio floor
- **Studio lighting** — a professional 3-point+ setup (top softbox, side left, side right, and a highlight sun)
- **Orbiting camera** — the camera follows a Bezier circle path around the car for a smooth 360°-style reveal, with subtle organic shake layered on top

## ⚙️ Technical Details

- **Render engine:** Cycles
- **Objects:** 27 (car body, 4 wheels, mirror, interior, backdrop planes, cube, camera, curve path, 8 lights, empties)
- **Materials:** 46
- **Camera rig:** `Follow Path` constraint (Bezier circle) + additional location/rotation constraints for subtle handheld-style motion
- **Lighting:** softbox + dual side lights + highlight sun, plus supplementary scene lights

## 📸 Deliverables in This Repo

- **`Car.mkv`** — final rendered animation (frames 1–120)
- **`Car.png`** — key still frame
- `README.md` — this file

The full Blender project file (`.blend`) is available on request.

---

Made with 🧡 in Blender.