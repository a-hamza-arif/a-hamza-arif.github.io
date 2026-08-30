# Luxury Perfume Commercial (Blender / Cycles)

A cinematic **luxury perfume product commercial** — a glossy black glass bottle with a brushed-gold cap and engraved gold label text, modeled and rendered entirely in Blender using **Cycles**, cut together from four distinct camera shots in the style of a high-end fragrance ad.

---

## 🎬 Overview

| | |
|---|---|
| **Tool** | Blender, Cycles render engine |
| **Scene** | Single scene, 4-shot edit (camera-marker driven) |
| **Frame Range** | 1–310 |
| **FPS** | 24 |
| **Duration** | ~12.9 sec |
| **Native Render Resolution** | 340×605 (vertical) |
| **Delivered Container** | 1920×1080 (letterboxed) |
| **Audio** | None |

## 🍾 Shot Breakdown

The commercial is cut together from **4 timed camera shots**, switched via timeline markers over a single continuous scene:

| Shot | Frame In | Camera | Description |
|---|---|---|---|
| Macro Reveal | 1 | `Cam_MacroReveal` | Extreme macro open, pulling focus to reveal the bottle and label |
| Dynamic | 96 | `Cam_Dynamic` | Dynamic moving shot around the bottle |
| Material Hero | 161 | `Cam_MaterialHero` | Hero framing highlighting the glass/metal material contrast |
| Orbit | 251 | `Cam_MaterialHero` | Continues on the hero camera for a closing orbiting move |

All cameras track a shared `Cam_Target` empty, keeping the bottle precisely framed through every move.

## 🧴 What's in the Scene

- **Bottle assembly** — `Bottle_Body` and `Bottle_NeckRing`, finished in deep glossy black glass
- **Cap assembly** — `Cap_Body`, `Cap_ShoulderRing`, `Cap_TopRim`, `Cap_NozzleButton`, and `Cap_TopperKnob`, built up from separate parts for a precise brushed/polished gold metal look
- **Label text** — `Label_BrandName`, `Label_ProductName`, and `Label_Type` (e.g. fragrance type/"Eau de Parfum"-style line), engraved in gold on the bottle face
- **Showcase pedestal** — a dedicated reflective surface (`Showcase_Pedestal`) the bottle sits on, giving the moody mirror reflection seen throughout
- **5-light studio rig** — `Key_Light`, `Fill_Light`, `Rim_Light`, a dedicated `Label_Accent_Light` for making the gold text pop, and a `Floor_Light` for the pedestal reflection

## ⚙️ Technical Details

- **Render engine:** Cycles
- **Objects:** 20 (bottle/cap parts, label meshes, pedestal, 3 cameras + target empty, 5 lights)
- **Materials:** 8 — dedicated shaders for the glass, gold metal, and pedestal surface
- **Editing method:** Blender timeline markers bound to cameras (`Cut_MacroReveal`, `Cut_Dynamic`, `Cut_MaterialHero`, `Cut_Orbit`) — Blender automatically switches the active render camera at each marker

## ▶️ How to Open / Render

1. Open `Project10_Luxury_Perfume_Commercial.blend` in Blender.
2. The full edit runs frames **1–310** at 24fps (~12.9s) — camera switching happens automatically via the timeline markers.
3. `Render → Render Animation` to reproduce the full 4-shot sequence in one pass.
4. Native scene resolution is **340×605** (vertical/story-style aspect); the delivered `.mkv` in this repo is exported into a 1920×1080 letterboxed container.
5. No audio track — this is a silent product render; a voiceover/music track would typically be added in post for the final ad.

## 📁 Repo Contents

```
.
├── Project10_Luxury_Perfume_Commercial.blend   # Main Blender project file (4-shot edit)
├── 0001-0310.mkv                                  # Rendered animation (frames 1–310)
├── frames/                                          # Rendered image sequence
└── README.md
```



Made with 🧡 in Blender.
