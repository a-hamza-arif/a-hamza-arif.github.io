# Sci-Fi Environment — Vanguard at the Core (Blender / Cycles)

A moody **sci-fi environment shot** — an armored character standing at the edge of a platform overlooking a vast, ring-lined structure that recedes toward a glowing volumetric core. Built and rendered entirely in Blender using **Cycles**.

---

## 🎬 Overview

| | |
|---|---|
| **Tool** | Blender, Cycles render engine |
| **Scene** | Single scene, single animated camera |
| **Frame Range** | 1–85 |
| **FPS** | 12 |
| **Duration** | ~7 sec |
| **Resolution** | 1920×1080 |
| **Audio** | None |

## 🚀 What's in the Scene

- **"Vanguard" character** — a fully rigged, armored character (body + glowing visor) with Mixamo-driven animation, standing at the edge of a platform looking out into the structure
- **Concentric ring tunnel** — a huge domed structure built from a single mesh using **Array + Build + Solidify** modifiers, creating the receding ring/segment pattern that lines the tunnel walls
- **Volumetric core glow** — a massive enclosing cube shaded with a pure **Principled Volume** material, producing the warm red/orange atmospheric haze and glowing core light that fills the whole structure
- **Platform ledge** — a simple cube-based platform the character stands on, lit in cool blue to contrast against the warm tunnel glow
- **Point-light rig** — three point lights shaping the character and platform lighting against the volumetric backdrop
- **Animated camera** — a full camera animation (`CameraAction`) with additional subtle motion layered on top, moving through the scene across all 85 frames

## 🎨 Look & Style

Split cool/warm lighting (blue platform vs. red-orange tunnel glow), heavy volumetric atmosphere, and a lone armored silhouette — aiming for a cinematic, concept-art-style sci-fi reveal shot.

## ⚙️ Technical Details

- **Render engine:** Cycles
- **Objects:** 12 (character mesh + visor, armature, ring-tunnel dome, volume cube, platform cube, camera, empties, 3 point lights)
- **Materials:** 6, including `VanguardBodyMat`, `Vanguard_VisorMat`, and a dedicated volumetric shader for the core glow
- **Modifier stack (tunnel structure):** Array → Build → Solidify on a single dome mesh
- **Character animation:** Mixamo-sourced armature action

## ▶️ How to Open / Render

1. Open `SciFiEnvironment.blend` in Blender (Cycles-capable GPU strongly recommended — the volumetric shader is render-intensive).
2. Scene runs frames **1–85** at 12fps (~7s) — the camera move plays out across the full range.
3. `Render → Render Animation` to reproduce the sequence, or scrub the timeline and `Render → Render Image` for a single still (great for a hero/cover shot).
4. No audio track — this is a silent visual piece; add music/SFX in post if desired.

## 📁 Repo Contents

```
.
├── SciFiEnvironment.blend   # Main Blender project file
├── Final.mkv                  # Rendered animation (frames 1–85)
├── frames/                     # Rendered image sequence
└── README.md
```

Made with 🧡 in Blender.
