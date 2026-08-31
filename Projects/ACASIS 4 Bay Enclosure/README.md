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

| Shot | Frame In | Camera | Description |
|---|---|---|---|
| 01 — Hero Reveal | 1 | `CAM_01_HERO` | Opening reveal of the full enclosure |
| 02 — Detail Macro | 305 | `CAM_02_DETAIL` | Close-up macro pass over ports and surface detailing |
| 03 — Orbit | 420 | `CAM_03_ORBIT` | Orbiting move around the product |
| 04 — Final Hero | 570 | `CAM_04_FINAL` | Closing hero shot |

Each camera has its own independent animation, and each targets a dedicated tracking empty so framing stays locked onto the product through every move.

## 📦 What's in the Scene

- **ACASIS 4-Bay Enclosure model** — the full product mesh, including individually modeled ports (USB-A/USB-C), brushed-metal grille detailing, and branding
- **Studio cyclorama backdrop** — seamless curved studio floor/wall for a clean product-photography backdrop
- **4-point studio lighting** — dedicated Key, Fill, and dual Rim (left/right) lights
- **Materials** — a detailed material library including brushed/base metal, copper, glossy black plastic, USB-A plastic, and rubber/soft-touch shaders

## ⚙️ Technical Details

- **Render engine:** Eevee
- **Objects:** 14 (product mesh, cyclorama, 4 lights, 3 camera-target empties, 4 shot cameras + 1 master camera)
- **Materials:** 16
- **Cameras:** 5 total — 4 individually animated shot cameras plus a master camera used for final output switching
- **Editing method:** Blender timeline markers bound to cameras — Blender automatically switches the active render camera at each marker

## 📸 Deliverables in This Repo

- **`ACASIS 4 Bay Enclosure.mkv`** — final rendered animation (frames 1–621)
- **`ACASIS 4 Bay Enclosure.png`** — key still frame
- `README.md` — this file

The full Blender project file (`.blend`) is available on request.

---

Made with 🧡 in Blender.