# Denis Targaroff — Robotic Serpent Creature (Blender / Cycles)

A short, moody **creature reveal** — "Denis Targaroff," a segmented robotic/bio-mechanical serpent lit by its own glowing red joints and visor, modeled, rigged, and rendered entirely in Blender using **Cycles**. Framed vertically for short-form video (Reels/TikTok/Shorts).

---

## 🎬 Overview

| | |
|---|---|
| **Tool** | Blender, Cycles render engine |
| **Scene** | Single scene, 4-shot edit (camera-marker driven) |
| **Frame Range** | 1–360 |
| **FPS** | 30 |
| **Duration** | 12 sec |
| **Resolution** | 1080×1920 (vertical) |
| **Audio** | None |

## 🐍 Shot Breakdown

| Shot | Frame In | Camera | Description |
|---|---|---|---|
| 1 — Establish | 1 | `Cam_Establish` | Wide establishing shot on a dark reflective surface |
| 2 — Reveal | 100 | `Cam_Reveal` | Camera move revealing the creature's full segmented body |
| 3 — Macro | 220 | `Cam_Macro` | Close-up macro pass on the head and glowing joints |
| 4 — Hero | 300 | `Cam_Establish` | Returns to the establishing camera for a final hero beat |

## 🦾 What's in the Scene

- **Denis Targaroff (the creature)** — a segmented robotic serpent with a faceted, geometric head, glowing red visor/eye elements, and an articulated body of luminous ring-jointed segments
- **22-bone armature (`Snake_Rig`)** — drives the full body's serpentine motion
- **Curve-driven body** — the creature's spine follows a dedicated curve, with paired hose curves for additional cabling/detail
- **Instanced tail segments** — a collection of beveled curve segments builds up the tapering tail
- **Emissive material set** — dedicated red/white emission variants layered over a dark base shader for the glowing-in-the-dark look
- **Reflective ground plane** — a simple dark glossy surface that mirrors the creature and light sources

## ⚙️ Technical Details

- **Render engine:** Cycles
- **Objects:** 47 (creature body/head parts, 22-bone armature, curves, tail-instance segments, 3 cameras, 5 lights, ground plane)
- **Materials:** 6, purpose-built for the creature's glow, plus a ground material
- **Collections:** organized into `Head`, `Tail`, `Tail_Instancing`, `Snake` (rig/body), `Enviroment`, and `Snake_Scene`

## 📸 Deliverables in This Repo

- **`Denis_Targaroff.mkv`** — final rendered animation (frames 1–360)
- **`Denis_Targaroff.png`** — key still frame
- `README.md` — this file

The full Blender project file (`.blend`) is available on request.

---

Made with 🧡 in Blender.