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

- **Cryostat stack** — multiple gold-toned thermal-stage plates mounted on a central support column, in the classic dilution-refrigerator "chandelier" arrangement
- **Coiled coax cabling** — dozens of spiral-wound signal cables and control loops running between the plates
- **Qubit chip** — a dedicated chip object with two material states, "qubit off" and "1 qubit on" (emissive)
- **Studio lighting** — a soft three-point setup against a dark neutral studio background
- **Animated camera** — the camera moves along an animated path while tracking a focus point, giving a smooth guided reveal through the cryostat stages

## ⚙️ Technical Details

- **Render engine:** Cycles
- **Objects:** 47 (stage plates, spiral coils, curves/wiring, support column, qubit chip variants, camera, focus/track empties, lights)
- **Materials:** 11, including dedicated gold-steel, chip, ion-trap-metal, and emissive materials
- **Camera rig:** `Track To` constraint following a focus-point empty, animated along a camera path for the full 306-frame reveal

## 📸 Deliverables in This Repo

- **`Quantum Computer.mkv`** — final rendered animation (frames 0–305)
- **`Quantum Computer.png`** — key still frame
- `README.md` — this file

The full Blender project file (`.blend`) is available on request.

---

Made with 🧡 in Blender.