# Quantum Computer — Cryostat Visualization (Blender / Cycles)

A studio-style **3D visualization of a quantum computer's dilution refrigerator** — the iconic gold "chandelier" of stacked thermal-stage plates, coiled coaxial wiring, and a qubit chip, modeled and rendered in Blender using **Cycles**.

---

## 🎬 Overview

| | |
|---|---|
| **Tool** | Blender, Cycles render engine |
| **Scene** | Single scene, single animated camera |
| **Frame Range** | 0–305 |
| **FPS** | 24 |
| **Duration** | ~12.75 sec |
| **Resolution** | 2560×1440 |
| **Audio** | None |

## 🧊 What's in the Scene

- **Cryostat stack** — multiple gold-toned thermal-stage plates (mixing chamber down to the outer vacuum can) mounted on a central support column, in the classic dilution-refrigerator "chandelier" arrangement
- **Coiled coax cabling** — dozens of spiral-wound signal cables and control loops running between the plates, modeled with curve/spiral geometry for an accurate, dense wiring look
- **Qubit chip** — a dedicated chip object with two material states, **"qubit off"** and **"1 qubit on"** (emissive), used to visually highlight an active qubit against the inactive chip
- **Studio lighting** — a soft three-point setup (key, fill, rim) against a dark neutral studio background for a clean, editorial/product-visualization look
- **Animated camera** — the camera moves along an animated path while tracking a focus point, giving a smooth guided reveal through the cryostat stages rather than a static shot

## ⚙️ Technical Details

- **Render engine:** Cycles
- **Objects:** 47 (stage plates, spiral coils, curves/wiring, support column, qubit chip variants, camera, focus/track empties, lights)
- **Materials:** 11, including dedicated `Gold.Steel`, `Chip` / `Chip2`, `Ion trap metal`, `Qubit off`, and `emissive` materials
- **Camera rig:** `Track To` constraint following a focus-point empty, animated along a camera path (`CameraAction.001`) for the full 306-frame reveal
- **Collections:** scene is organized into `Quantum_Comp` (hardware), a `qubits` sub-collection (on/off chip states), lighting, background, and spare-parts collections for easy toggling

## ▶️ How to Open / Render

1. Open `Quantum Computer.blend` in Blender (Cycles-capable GPU recommended).
2. Scene runs frames **0–305** at 24fps (~12.75s) — the animated camera completes its full reveal move across this range.
3. `Render → Render Animation` to reproduce the sequence, or scrub the timeline and `Render → Render Image` for a single still (great for a hero/cover shot).
4. No audio track — this is a silent visualization; add music/voiceover in post if desired.

## 📁 Repo Contents

```
.
├── Quantum Computer.blend   # Main Blender project file
├── Final.mkv                  # Rendered animation (frames 0–305)
├── frames/                     # Rendered image sequence
└── README.md
```


Made with 🧡 in Blender.
