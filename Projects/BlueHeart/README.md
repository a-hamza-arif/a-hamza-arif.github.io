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

- **Wireframe icosahedron shell** — an icosphere built up with **Wireframe + Bevel + Subdivision Surface** modifiers, giving the faceted metallic-edge/cage look
- **Cracked inner core** — a second icosphere layered inside, carrying the cracked/fractured glass-like surface material visible through the shell's open faces
- **Small inner icosphere** — a compact third object nested at the center (a "core" element)
- **Ground plane** — large (18×18) textured plane with a matching cracked-surface material, grounding the object in the shot
- **Enclosing cube** — a large (27³) surrounding cube, used for backdrop/environment framing
- **Cold blue area light** — a single area light (RGB ≈ 0.18, 0.52, 1.0) driving the entire moody, cinematic blue lighting
- **Animated camera** — one camera animation (`CameraAction`) driving the full reveal move across all 132 frames

## ⚙️ Technical Details

- **Render engine:** Eevee
- **Objects:** 7 (3 icospheres, plane, cube, camera, light)
- **Materials:** 6, including the wireframe shell material and the cracked/fractured surface material
- **Modifier stack (main shell):** Wireframe → Bevel → Wireframe → Subdivision Surface

## ▶️ How to Open / Render

1. Open `Final.blend` in Blender.
2. Scene runs frames **1–132** at 24fps (~5.5s) with the animated camera doing the full reveal.
3. `Render → Render Animation` to reproduce the sequence, or scrub the timeline and `Render → Render Image` for a single still.
4. No audio track — this is a silent visual piece; add music/SFX in post if desired.

## 📁 Repo Contents

```
.
├── Final.blend       # Main Blender project file
├── Final.mkv           # Rendered animation (frames 1–132)
├── frames/              # Rendered image sequence
└── README.md
```

Made with 🧡 in Blender.
