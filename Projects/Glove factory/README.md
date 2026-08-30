# Glove Factory — Industrial Production Line (Blender / Cycles)

A fully 3D-modeled and animated **industrial factory production line**, built and rendered in Blender using **Cycles**. The animation visualizes an end-to-end manufacturing process — from raw material through multiple processing machines, packaging, robotic palletizing, and forklift pickup.

---

## 🎬 Overview

| | |
|---|---|
| **Tool** | Blender (Cycles render engine) |
| **Scene** | Single scene, single continuous camera move |
| **Frame Range** | 1–2000 (this render covers frames 1–1120) |
| **FPS** | 24 |
| **Resolution** | 1920×1080 |
| **Audio** | None — visual-only industrial animation |

## 🏭 What's in the Scene

A single large factory-floor scene containing:

- **Production machine lines** — multiple rows of identical processing units (roll-fed material machines) arranged in a symmetric factory layout
- **Conveyor systems** — belt conveyors moving individual product units and finished cartons between stations
- **Robotic arms** — industrial pick-and-place robots (KUKA-style) loading/unloading pallets, plus **Robotiq 2F-140** two-finger grippers for precision handling
- **Case packing / carton sealing station** — automated box erecting, filling, and sealing equipment
- **Palletizing area** — robotic arms stacking finished cartons onto wooden pallets
- **Forklift truck** — animated forklift moving completed pallets out of the production area
- **Human characters** — MetaHuman-based factory workers walking the floor for scale and realism
- **Full factory environment** — floor, walls, and lighting set up for a clean industrial-visualization look

This is the kind of animation typically used for **industrial equipment marketing, machine-manufacturer showcases, or process-visualization/explainer videos**.

## ⚙️ Technical Details

- **Render engine:** Cycles
- **Scene complexity:** ~25,000 objects, ~3,000 meshes, 140 materials, 325 textures/images
- **Rigging:** 8 armatures (robotic arms + character rigs)
- **Node setup:** Extensive procedural material node groups (PBR textures, anti-tiling, edge wear, reflection/fresnel utility nodes, logic-gate driver setups for machine-state animation)

## ▶️ How to Open / Render

1. Open `Glove_factory.blend` in Blender (Cycles-capable GPU recommended given the scene density).
2. The full scene is on frame range **1–2000**; this repo's rendered video/frames cover **1–1120**.
3. `Render → Render Animation` to reproduce the sequence, or render a still with `Render → Render Image` at any frame for a preview.
4. No audio track — the render is a silent visualization, ready to have a soundtrack or voiceover added in post if needed.

## 📁 Repo Contents

```
.
├── Glove_factory.blend    # Main Blender project file (single scene)
├── 0001-1120.mp4           # Rendered animation, frames 1–1120
├── frames/                  # Rendered image sequence (frames 1–1120)
└── README.md
```

Made with 🧡 in Blender.
