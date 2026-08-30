# AI Data Center — Facility Visualization (Blender / Cycles)

A large-scale, engineering-detailed **AI data center visualization** — a full facility flythrough covering the exterior campus, server hall interior, mechanical/cooling infrastructure, and the on-site electrical substation. Modeled and rendered entirely in Blender using **Cycles**.

---

## 🎬 Overview

| | |
|---|---|
| **Tool** | Blender, Cycles render engine |
| **Scene** | Single scene, single continuous camera flythrough |
| **Frame Range** | 0–1730 |
| **FPS** | 24 |
| **Duration** | 72 sec |
| **Resolution** | 1920×1080 |
| **Audio** | None |

## 🏢 What's in the Scene

This is a genuinely large, engineering-grade build — **4,230 objects** across **1,336 meshes**, covering the full site:

- **Data center building** — the main facility shell with roof-mounted cooling/condenser units and building services
- **Exterior campus** — access roads, landscaped grass areas, and a row of external generator/battery enclosures on outdoor pads
- **Electrical substation** — a fully modeled switchyard with transformers, insulator stacks, switchgear structures, overhead conductor lines, and perimeter security fencing
- **Server hall interior** — long aisles of server racks under an extensive overhead structural grid carrying cable tray and busway runs
- **Mechanical/cooling piping systems** — the model is built from a dense, professional-grade MEP component library, including:
  - Seamless steel pipe runs, rectangular and round ductwork, and copper piping (thousands of individual segments)
  - Insulated pipe/duct sections (K-Flex insulation components)
  - Standardized CAx pipe fittings — elbows, T-pieces, flanges, transitions, and nozzles
  - Real-world pipe support hardware (Müpro anchor/expansion clamps, brackets, and wall-hanger channels)
  - Transformer lines, power modules, and cable trenches (Caniveau)

This level of detail reflects a proper MEP/engineering-visualization pipeline rather than a purely stylized render — the piping, ductwork, and support hardware are modeled to match real manufacturer component geometry.

## ⚙️ Technical Details

- **Render engine:** Cycles
- **Objects:** 4,230 (1,336 unique meshes, heavily instanced/duplicated across the piping and support-hardware systems)
- **Materials:** 81
- **Images/textures:** 155
- **Camera:** a single animated camera performing the full flythrough across all 1,730 frames, with additional subtle motion layered on top for a more organic, cinematic feel rather than a locked architectural pan

## ▶️ How to Open / Render

1. Open `AI_Data_Center.blend` in Blender. **Note:** this is a ~1GB file with 4,000+ objects — expect longer load and viewport times, and a capable GPU is strongly recommended for Cycles rendering at this scene density.
2. The full flythrough runs frames **0–1730** at 24fps (72s exactly).
3. `Render → Render Animation` to reproduce the full sequence, or scrub the timeline and `Render → Render Image` for a single still (the substation and server-hall interior shots make particularly strong stills).
4. No audio track — this is a silent facility visualization; a voiceover/music track would typically be added in post for a final presentation cut.

## 📁 Repo Contents

```
.
├── AI_Data_Center.blend   # Main Blender project file (full facility model + flythrough)
├── AI_Data_Center.mkv       # Rendered animation (frames 0–1730)
├── frames/                    # Rendered image sequence
└── README.md
```


Made with 🧡 in Blender.
