# BlueHeart — Stylized 3D Object Reveal (Blender / Eevee)

A short, moody **3D object-reveal animation** built in Blender and rendered with **Eevee** — a wireframe-shelled icosahedron with a cracked, glass-like inner surface, lit in cold blue tones and slowly revealed by a camera move.

---

## 🎬 Overview

| | |
|---|---|
| **Tool** | Blender, Eevee render engine |
| **Scene** | Single scene, single camera animation (orbit/reveal move) |
| **Frame Range** | 1–132 |
| **FPS** | 24 |
| **Duration** | ~5.5 sec |
| **Resolution** | 1920×1080 |
| **Audio** | None |

## 🔷 What's in the Scene

- **Wireframe icosahedron shell** — an icosphere built up with Wireframe + Bevel + Subdivision Surface modifiers
- **Cracked inner core** — a second icosphere layered inside, carrying a cracked/fractured glass-like surface material
- **Small inner icosphere** — a compact third object nested at the center
- **Ground plane** — large (18×18) textured plane with a matching cracked-surface material
- **Enclosing cube** — a large (27³) surrounding cube used for backdrop/environment framing
- **Cold blue area light** — driving the entire moody, cinematic blue lighting
- **Animated camera** — one camera animation driving the full reveal move across all 132 frames

## ⚙️ Technical Details

- **Render engine:** Eevee
- **Objects:** 7 (3 icospheres, plane, cube, camera, light)
- **Materials:** 6, including the wireframe shell material and the cracked/fractured surface material
- **Modifier stack (main shell):** Wireframe → Bevel → Wireframe → Subdivision Surface

## 📸 Deliverables in This Repo

- **`BlueHeart.mkv`** — final rendered animation (frames 1–132)
- **`BlueHeart.png`** — key still frame
- `README.md` — this file

The full Blender project file (`.blend`) is available on request.

---

Made with 🧡 in Blender.