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

- **"Vanguard" character** — a fully rigged, armored character (body + glowing visor) with Mixamo-driven animation, standing at the edge of a platform
- **Concentric ring tunnel** — a huge domed structure built from a single mesh using Array + Build + Solidify modifiers, creating the receding ring/segment pattern
- **Volumetric core glow** — a massive enclosing cube shaded with a pure Principled Volume material, producing the warm red/orange atmospheric haze
- **Platform ledge** — a simple cube-based platform the character stands on, lit in cool blue to contrast against the warm tunnel glow
- **Point-light rig** — three point lights shaping the character and platform lighting against the volumetric backdrop
- **Animated camera** — a full camera animation with additional subtle motion layered on top, moving through the scene across all 85 frames

## 🎨 Look & Style

Split cool/warm lighting (blue platform vs. red-orange tunnel glow), heavy volumetric atmosphere, and a lone armored silhouette — aiming for a cinematic, concept-art-style sci-fi reveal shot.

## ⚙️ Technical Details

- **Render engine:** Cycles
- **Objects:** 12 (character mesh + visor, armature, ring-tunnel dome, volume cube, platform cube, camera, empties, 3 point lights)
- **Materials:** 6, including a dedicated volumetric shader for the core glow
- **Modifier stack (tunnel structure):** Array → Build → Solidify on a single dome mesh
- **Character animation:** Mixamo-sourced armature action

## 📸 Deliverables in This Repo

- **`SciFiEnvironment.mkv`** — final rendered animation (frames 1–85)
- **`SciFiEnvironment.png`** — key still frame
- `README.md` — this file

The full Blender project file (`.blend`) is available on request.

---

Made with 🧡 in Blender.