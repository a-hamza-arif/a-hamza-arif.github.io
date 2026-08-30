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

The animation is cut together from **4 timed camera shots**, switched via timeline markers over a single continuous scene:

| Shot | Frame In | Camera | Description |
|---|---|---|---|
| 1 — Establish | 1 | `Cam_Establish` | Wide establishing shot on a dark reflective surface |
| 2 — Reveal | 100 | `Cam_Reveal` | Camera move revealing the creature's full segmented body |
| 3 — Macro | 220 | `Cam_Macro` | Close-up macro pass on the head and glowing joints |
| 4 — Hero | 300 | `Cam_Establish` | Returns to the establishing camera for a final hero beat |

## 🦾 What's in the Scene

- **Denis Targaroff (the creature)** — a segmented robotic serpent with a faceted, geometric head, glowing red visor/eye elements, and an articulated body of luminous ring-jointed segments
- **22-bone armature (`Snake_Rig`)** — drives the full body's serpentine motion
- **Curve-driven body** — the creature's spine follows a dedicated `Snake_Path` curve, with paired `Hose_Left` / `Hose_Right` curves for additional cabling/detail running along the body
- **Instanced tail segments** — a `Tail_Instancing` collection of beveled curve segments builds up the tapering tail
- **Emissive material set** — dedicated `Snake_Emission_Red`, `Snake_Emission_White`, `Snake_Emission_02`, and a `Snake_Emission_Projector` material, all layered over a dark `Snake_Base` shader for the glowing-in-the-dark look
- **Reflective ground plane** — a simple dark glossy surface that mirrors the creature and light sources, reinforcing the moody, minimal presentation

## ⚙️ Technical Details

- **Render engine:** Cycles
- **Objects:** 47 (creature body/head parts, 22-bone armature, curves, tail-instance segments, 3 cameras, 5 lights, ground plane)
- **Materials:** 6, purpose-built for the creature's glow (`Snake_Base` + 4 emission variants) plus a `Ground` material
- **Collections:** organized into `Head`, `Tail`, `Tail_Instancing`, `Snake` (rig/body), `Enviroment`, and `Snake_Scene`
- **Editing method:** Blender timeline markers bound to cameras (`Shot1_Establish`, `Shot2_Reveal`, `Shot3_Macro`, `Shot4_Hero`) — Blender automatically switches the active render camera at each marker

## ▶️ How to Open / Render

1. Open `Denis Targaroff.blend` in Blender.
2. The full edit runs frames **1–360** at 30fps (12s exactly) — camera switching happens automatically via the timeline markers.
3. `Render → Render Animation` to reproduce the full 4-shot sequence in one pass.
4. To review or adjust an individual shot, jump to its marker frame and work with that shot's camera directly.
5. No audio track — this is a silent creature reveal; music/SFX would typically be added in post for a final social cut.
6. **Note:** the render is vertical (1080×1920) — built specifically for short-form/mobile video platforms.

## 📁 Repo Contents

```
.
├── Denis Targaroff.blend   # Main Blender project file (4-shot edit)
├── Denis_Targaroff.mkv       # Rendered animation (frames 1–360)
├── frames/                     # Rendered image sequence
└── README.md
```


Made with 🧡 in Blender.
