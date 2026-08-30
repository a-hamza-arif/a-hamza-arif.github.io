# 3D Lyrics — Animated Lyric Video (Blender)

A short 3D-animated lyric video built in **Blender**, rendered with **Eevee**. The piece follows a character through four connected scenes — a bedroom wake-up, a close-up transition, and a night walk through a city street — synced to music.

---

## 🎬 Overview

| | |
|---|---|
| **Tool** | Blender 5.2.0 LTS |
| **Render Engine** | Eevee |
| **Runtime** | ~2 min 45 sec |
| **Output** | 1920×1080, 30fps, H.264 |
| **Scenes** | 4 |
| **Character rig / animation** | Mixamo (auto-rigged, retargeted) |

## 🗂️ Scene Breakdown

The project is split into **4 separate Blender scenes**, each with its own camera, lighting, and collection setup — a common workflow for keeping lyric-video sequences modular and easy to re-render independently.

1. **Scene_001 — Bedroom**
   Character wake-up / room intro. Fully modeled bedroom: bed, cabinet, desk with drawers, potted plant, wall posters, door, and window. (2560×1440, 30fps, 430 frames)

2. **Scene_002 — Close-up / Transition**
   A tighter, simplified scene used as a visual transition beat between the bedroom and the street. (1920×1080, 24fps, 170 frames)

3. **Scene_003 — Night Street Walk**
   Character walks down a city sidewalk lined with brownstone-style buildings, road markings, and streetlight ambience. (1920×1080, 24fps, 340 frames)

4. **Scene_004 — Street Continued**
   Extended outdoor environment with trees, plants, clouds, and additional background props. (1920×1080, 24fps, 200 frames)

## 🧱 What's in the Scenes

- **furniture & props**: bed, cabinet/drawers, desk, plant pot, books, stationery (pen, eraser), wall art/posters
- **PBR texture sets**: fabric, wood flooring, wood paneling, tile — sourced from Textures.com / similar libraries
- **HDRI environment lighting** (`paul_lobe_haus`)
- **Mixamo-based character animation** (6 armatures, multiple retargeted actions across scenes)
- **Procedural sky / cloud elements** for the outdoor scenes
- Decorative wall art referencing classic paintings (*The Great Wave*, *The Persistence of Memory*, *Starry Night*, *The Last Supper*) alongside anime posters

## ⚙️ Requirements

- Blender **5.2.0 LTS** or newer (project uses current Eevee; may work on 4.x with minor adjustments)
- ~120 MB of texture/asset data (packed into the `.blend`)

## ▶️ How to Open / Render

1. Open `Final.blend` in Blender.
2. Use the **Scene** dropdown (top-right of the timeline) to switch between `Scene_001`–`Scene_004`.
3. Each scene has its own camera and frame range — hit `Render → Render Animation` per scene, or batch-render all four and stitch them together (e.g. with FFmpeg) in scene order to reproduce the final cut.
4. Audio is synced externally — combine the rendered output with the music track using your NLE of choice (or FFmpeg) to reproduce the final lyric video (see the pre-rendered copy in this repo for reference).

## 📁 Repo Contents

```
.
├── Final.blend           # Main Blender project file (all 4 scenes, packed assets)
├── 3d_lyrics.mp4          # Final rendered lyric video (with audio)
└── README.md
```

## 🙏 Credits

- Character animation: [Mixamo](https://www.mixamo.com/)
- HDRI: Poly Haven-style HDRI environment
- Textures: Textures.com / similar PBR libraries

---

Made with 🧡 in Blender.