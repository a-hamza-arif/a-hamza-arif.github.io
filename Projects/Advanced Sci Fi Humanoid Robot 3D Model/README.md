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

The animation is cut together from **6 timed camera shots**, switched via timeline markers over a single continuous scene:

| Shot | Frame In | Camera | Description |
|---|---|---|---|
| 01 — Detail Open | 1 | `Cam_01_DetailOpen` | Opening macro close-up on the glowing chest reactor core |
| 02 — Full Reveal | 60 | `Cam_02_FullReveal` | Pulls back to reveal the complete robot |
| 03 — Dynamic | 169 | `Cam_03_Dynamic` | Dynamic moving shot around the character |
| 04 — Detail Hip | 210 | `Cam_04_DetailHip` | Close-up detail pass on the hip/leg thruster assembly |
| 05 — Hero Final | 267 | `Cam_05_HeroFinal` | Final hero framing |
| 06 — Orbit 360 | 362 | `Cam_06_Orbit360` | Full 360° orbit around the completed model |

Each camera has an individually keyframed animation, and several are paired with their own dedicated **shake-target** action for subtle handheld-style motion on top of the base move.

## 🦾 What's in the Scene

- **Fully rigged robot character** — boxy, heavy-armor sci-fi humanoid design, driven by an armature for the subtle idle/reveal posing seen across the shots
- **Glowing reactor core** — chest-mounted emissive core (`Reactor_Core_Glow` + `Reactor_Bezel` materials) used as the visual focal point of the opening shot
- **Detailed material library** — brass thrusters, gunmetal jointing (3 variants), red power-accent panels, and painted chassis armor, giving the model a layered, mechanical look
- **Studio environment** — a simple studio floor material and lighting rig for a clean, focused presentation (no distracting background)
- **6-light rig** — 6 area lights, a point light, and a sun lamp shaping the moody rim-lit look across every shot

## ⚙️ Technical Details

- **Render engine:** Cycles
- **Objects:** 82 (robot mesh parts, armature, 6 cameras, camera-rig helpers, 5 environment/light objects, curves)
- **Meshes:** 55 (indicating a heavily part-based hard-surface build rather than a single merged mesh)
- **Materials:** 10, purpose-built and named per component (`Brass_Thruster`, `Chassis_Armor`, `Gunmetal_Joint` A/B/C, `Power_Accent_Red`, `Reactor_Core_Glow`, `Reactor_Bezel`, `Studio_Floor_Mat`)
- **Scene organization:** cleanly split into `01_Robot_Model`, `02_Cameras`, `03_Lights`, `04_Camera_Rig`, and `05_Environment` collections
- **Editing method:** Blender timeline markers bound to cameras — Blender automatically switches the active render camera at each marker, reproducing the full 6-shot cut from a single render pass

## ▶️ How to Open / Render

1. Open `Advanced Sci Fi Humanoid Robot 3D Model.blend` in Blender.
2. The full edit runs frames **1–511** at 24fps (~21.3s) — camera switching happens automatically via the timeline markers.
3. `Render → Render Animation` to reproduce the full 6-shot sequence in one pass.
4. To review or adjust an individual shot, jump to its marker frame and work with that shot's camera directly.
5. No audio track — this is a silent model showcase; music/SFX would typically be added in post for a final trailer cut.

## 📁 Repo Contents

```
.
├── Advanced Sci Fi Humanoid Robot 3D Model.blend   # Main Blender project file (6-shot edit)
├── 0001-0511.mkv                                      # Rendered animation (frames 1–511)
├── frames/                                              # Rendered image sequence
└── README.md
```



Made with 🧡 in Blender.
