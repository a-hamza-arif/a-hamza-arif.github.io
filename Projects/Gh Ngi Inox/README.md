# Ghế Ngồi Inox — Stainless Steel Stool Visualization (Blender / Eevee)

A clean, studio-style **product visualization** for a stainless-steel wire-frame stool ("Ghế Ngồi Inox" — Vietnamese for *stainless steel stool*), modeled and rendered entirely in Blender using **Eevee**. The piece plays the same stool design twice side-by-side — once multiplied into a dense stack of coiled wire legs, and once as the final, resolved stool.

---

## 🎬 Overview

| | |
|---|---|
| **Tool** | Blender, Eevee render engine |
| **Scene** | Single scene, single animated camera |
| **Frame Range** | 1–250 |
| **FPS** | 24 |
| **Duration** | ~10.4 sec |
| **Resolution** | 1920×1920 (square — social feed format) |
| **Audio** | None |

## 🪑 What's in the Scene

- **Ghế Ngồi Inox** — the finished stool: a wire-leg stainless-steel frame with a padded circular seat, finished in polished and matte steel with a gray plastic seat cap
- **Ghế Ngồi Inox.001** — a second copy of the same stool with an added Array modifier, multiplying its legs into a dense, cage-like stack of coiled wire
- **Sàn Nhà** ("floor") — a simple studio floor plane grounding both objects
- **Tracked camera** — uses a `Track To` constraint on a look-target empty, animated to move through the scene
- **6-light studio rig** — giving the glossy steel its clean highlights and edge definition

## ⚙️ Technical Details

- **Render engine:** Eevee
- **Objects:** 12 (2 stool meshes, floor, camera, look-target/empty, 6 lights)
- **Materials:** 5 — polished steel, matte steel, gray plastic, plus supporting materials
- **Modifier stack (finished stool):** Solidify → Subdivision Surface
- **Modifier stack (stacked/process stool):** Solidify → Subdivision Surface → Array — the array is what produces the dense coiled-leg look

## 📸 Deliverables in This Repo

- **`Gh Ngi Inox.mkv`** — final rendered animation (frames 1–250)
- **`Gh Ngi Inox.png`** — key still frame
- `README.md` — this file

The full Blender project file (`.blend`) is available on request.

---

Made with 🧡 in Blender.