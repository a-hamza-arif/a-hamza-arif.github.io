# Ghế Ngồi Inox — Stainless Steel Stool Visualization (Blender / Eevee)

A clean, studio-style **product visualization** for a stainless-steel wire-frame stool ("Ghế Ngồi Inox" — Vietnamese for *stainless steel stool*), modeled and rendered entirely in Blender using **Eevee**. The piece plays the same stool design twice side-by-side — once multiplied into a dense stack of coiled wire legs, and once as the final, resolved stool — for a striking "many-into-one" visual effect.

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
- **Ghế Ngồi Inox.001** — a second copy of the same stool, but with an added **Array modifier**, multiplying its legs into a dense, cage-like stack of coiled wire — used as the "before/process" visual counterpart to the clean, final stool beside it
- **Sàn Nhà** ("floor") — a simple studio floor plane grounding both objects
- **Tracked camera** — the camera uses a `Track To` constraint on a `LookTarget` empty, animated to move through the scene while staying locked on the stools
- **6-light studio rig** — `Key_Light`, `Fill_Light`, `Soft_Fill`, `Rim_Hero`, `Top_Strip`, and `Floor_Kick`, giving the glossy steel its clean highlights and edge definition against the dark studio backdrop

## ⚙️ Technical Details

- **Render engine:** Eevee
- **Objects:** 12 (2 stool meshes, floor, camera, look-target/empty, 6 lights)
- **Materials:** 5 — `Thép Bóng` (polished steel), `Thép Đục` (matte steel), `Nhựa Xám` (gray plastic), plus supporting materials
- **Modifier stack (finished stool):** Solidify (`Rắn Hóa`) → Subdivision Surface (`Phân Hóa`)
- **Modifier stack (stacked/process stool):** Solidify → Subdivision Surface → **Array** (`Mảng`) — the array is what produces the dense coiled-leg look
- **Camera:** animated, `Track To` constraint on an animated look-target empty

## ▶️ How to Open / Render

1. Open `Gh Ngi Inox.blend` in Blender (original filename has stripped diacritics from *Ghế Ngồi Inox*).
2. Scene runs frames **1–250** at 24fps (~10.4s) — the animated camera move plays out across the full range.
3. `Render → Render Animation` to reproduce the sequence, or scrub the timeline and `Render → Render Image` for a single still (square format — great for a feed post).
4. No audio track — this is a silent product visualization; add music in post if desired.

## 📁 Repo Contents

```
.
├── Gh Ngi Inox.blend      # Main Blender project file
├── 0001-0250.mkv             # Rendered animation (frames 1–250)
├── frames/                     # Rendered image sequence
└── README.md
```


Made with 🧡 in Blender.
