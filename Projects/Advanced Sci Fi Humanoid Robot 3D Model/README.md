# Advanced Sci-Fi Humanoid Robot — 3D Model & Cinematic Reveal (Blender / Cycles)

A cinematic **model showcase/reveal** for an original sci-fi humanoid robot — modeled, rigged, and rendered entirely in Blender using **Cycles**, cut together from six distinct camera shots in the style of a game-asset or product cinematic trailer.

---

## 🎬 Overview

| | |
|---|---|
| **Tool** | Blender, Cycles render engine |
| **Scene** | Single scene, 6-shot edit (camera-marker driven) |
| **Frame Range** | 1–511 |
| **FPS** | 24 |
| **Duration** | ~21.3 sec |
| **Resolution** | 1920×1080 |
| **Audio** | None |

## 🤖 Shot Breakdown

| Shot | Frame In | Camera | Description |
|---|---|---|---|
| 01 — Detail Open | 1 | `Cam_01_DetailOpen` | Opening macro close-up on the glowing chest reactor core |
| 02 — Full Reveal | 60 | `Cam_02_FullReveal` | Pulls back to reveal the complete robot |
| 03 — Dynamic | 169 | `Cam_03_Dynamic` | Dynamic moving shot around the character |
| 04 — Detail Hip | 210 | `Cam_04_DetailHip` | Close-up detail pass on the hip/leg thruster assembly |
| 05 — Hero Final | 267 | `Cam_05_HeroFinal` | Final hero framing |
| 06 — Orbit 360 | 362 | `Cam_06_Orbit360` | Full 360° orbit around the completed model |

## 🪶 What's in the Scene

- **Fully rigged robot character** — boxy, heavy-armor sci-fi humanoid design, driven by an armature for subtle idle/reveal posing
- **Glowing reactor core** — chest-mounted emissive core used as the visual focal point of the opening shot
- **Detailed material library** — brass thrusters, gunmetal jointing (3 variants), red power-accent panels, and painted chassis armor
- **Studio environment** — a simple studio floor material and lighting rig for a clean, focused presentation
- **6-light rig** — 6 area lights, a point light, and a sun lamp shaping the moody rim-lit look

## ⚙️ Technical Details

- **Render engine:** Cycles
- **Objects:** 82 (robot mesh parts, armature, 6 cameras, camera-rig helpers, 5 environment/light objects, curves)
- **Meshes:** 55
- **Materials:** 10, purpose-built and named per component
- **Scene organization:** cleanly split into `01_Robot_Model`, `02_Cameras`, `03_Lights`, `04_Camera_Rig`, and `05_Environment` collections

## 📸 Deliverables in This Repo

- **`Advanced Sci Fi Humanoid Robot 3D Model.mkv`** — final rendered animation (frames 1–511)
- **`Advanced Sci Fi Humanoid Robot 3D Model.png`** — key still frame
- `README.md` — this file

The full Blender project file (`.blend`) is available on request.

---

Made with 🧡 in Blender.