# ACASIS 4-Bay Enclosure — Product Commercial (Blender / Eevee)

A clean, studio-style **product commercial** for the ACASIS 4-Bay drive enclosure — modeled and rendered entirely in Blender using **Eevee**, cut together from four distinct camera shots in the style of a real product-launch video.

---

## 🎬 Overview

| | |
|---|---|
| **Tool** | Blender, Eevee render engine |
| **Scene** | Single scene, 4-shot edit (camera-marker driven) |
| **Frame Range** | 1–621 |
| **FPS** | 24 |
| **Duration** | ~25.9 sec |
| **Resolution** | 3840×2160 (4K) |
| **Audio** | None |

## 🎥 Shot Breakdown

The animation is cut together from **4 timed camera shots**, switched via timeline markers over a single continuous scene — the same technique used in real commercial production pipelines:

| Shot | Frame In | Camera | Description |
|---|---|---|---|
| 01 — Hero Reveal | 1 | `CAM_01_HERO` | Opening reveal of the full enclosure |
| 02 — Detail Macro | 305 | `CAM_02_DETAIL` | Close-up macro pass over ports and surface detailing |
| 03 — Orbit | 420 | `CAM_03_ORBIT` | Orbiting move around the product |
| 04 — Final Hero | 570 | `CAM_04_FINAL` | Closing hero shot |

Each camera has its own independent animation, and each targets a dedicated tracking empty (`CAM_TARGET_PRODUCT`, `CAM_TARGET_DETAIL`, `CAM_TARGET_HERO`) so framing stays locked onto the product through every move.

## 📦 What's in the Scene

- **ACASIS 4-Bay Enclosure model** — the full product mesh, including individually modeled ports (USB-A/USB-C), brushed-metal grille detailing, and branding
- **Studio cyclorama backdrop** — seamless curved studio floor/wall for a clean product-photography backdrop
- **4-point studio lighting** — dedicated Key, Fill, and dual Rim (left/right) lights for classic glossy product-shot lighting and edge separation
- **Materials** — a detailed material library including brushed/base metal, copper, glossy black plastic, USB-A plastic, and rubber/soft-touch shaders for realistic port and housing detail

## ⚙️ Technical Details

- **Render engine:** Eevee
- **Objects:** 14 (product mesh, cyclorama, 4 lights, 3 camera-target empties, 4 shot cameras + 1 master camera)
- **Materials:** 16
- **Cameras:** 5 total — 4 individually animated shot cameras (`CAM_01_HERO`, `CAM_02_DETAIL`, `CAM_03_ORBIT`, `CAM_04_FINAL`) plus a master camera used for final output switching
- **Editing method:** Blender timeline markers bound to cameras (`SHOT_01_HERO_REVEAL`, `SHOT_02_DETAIL_MACRO`, `SHOT_03_ORBIT`, `SHOT_04_FINAL_HERO`) — Blender automatically switches the active render camera at each marker

## ▶️ How to Open / Render

1. Open `ACASIS 4 Bay Enclosure.blend` in Blender.
2. The full edit runs frames **1–621** at 24fps (~25.9s) — camera switching happens automatically via the timeline markers, no manual camera changes needed.
3. `Render → Render Animation` to reproduce the full 4-shot sequence in one pass.
4. To review/adjust an individual shot, jump to its marker frame and switch to that shot's camera directly.
5. No audio track — this is a silent product render; a voiceover/music track and text overlays would typically be added in post for the final commercial.

## 📁 Repo Contents

```
.
├── ACASIS 4 Bay Enclosure.blend   # Main Blender project file (4-shot edit)
├── 0001-0621.mkv                    # Rendered animation (frames 1–621)
├── frames/                           # Rendered image sequence
└── README.md
```


Made with 🧡 in Blender.
