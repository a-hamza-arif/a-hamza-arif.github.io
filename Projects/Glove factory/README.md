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

- **Production machine lines** — multiple rows of identical processing units arranged in a symmetric factory layout
- **Conveyor systems** — belt conveyors moving individual product units and finished cartons between stations
- **Robotic arms** — industrial pick-and-place robots (KUKA-style) loading/unloading pallets, plus two-finger grippers for precision handling
- **Case packing / carton sealing station** — automated box erecting, filling, and sealing equipment
- **Palletizing area** — robotic arms stacking finished cartons onto wooden pallets
- **Forklift truck** — animated forklift moving completed pallets out of the production area
- **Human characters** — MetaHuman-based factory workers walking the floor for scale and realism
- **Full factory environment** — floor, walls, and lighting for a clean industrial-visualization look

This is the kind of animation typically used for **industrial equipment marketing, machine-manufacturer showcases, or process-visualization/explainer videos**.

## ⚙️ Technical Details

- **Render engine:** Cycles
- **Scene complexity:** ~25,000 objects, ~3,000 meshes, 140 materials, 325 textures/images
- **Rigging:** 8 armatures (robotic arms + character rigs)
- **Node setup:** Extensive procedural material node groups (PBR textures, anti-tiling, edge wear, reflection/fresnel utility nodes, logic-gate driver setups for machine-state animation)

## 📸 Deliverables in This Repo

- **`Glove_Factory.mp4`** — final rendered animation, frames 1–1120
- **`Glove_Factory.png`** — key still frame
- `README.md` — this file

The full Blender project file (`.blend`) is available on request.

---

Made with 🧡 in Blender.