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
- **Exterior campus** — access roads, landscaped grass areas, and a row of external generator/battery enclosures
- **Electrical substation** — a fully modeled switchyard with transformers, insulator stacks, switchgear structures, overhead conductor lines, and perimeter security fencing
- **Server hall interior** — long aisles of server racks under an extensive overhead structural grid carrying cable tray and busway runs
- **Mechanical/cooling piping systems** — built from a dense, professional-grade MEP component library (seamless steel pipe runs, ductwork, copper piping, insulation, fittings, support hardware, transformer lines, cable trenches)

This level of detail reflects a proper MEP/engineering-visualization pipeline rather than a purely stylized render.

## ⚙️ Technical Details

- **Render engine:** Cycles
- **Objects:** 4,230 (1,336 unique meshes, heavily instanced/duplicated across the piping and support-hardware systems)
- **Materials:** 81
- **Images/textures:** 155
- **Camera:** a single animated camera performing the full flythrough across all 1,730 frames, with additional subtle motion layered on top for a more organic, cinematic feel

## 📸 Deliverables in This Repo

- **`AI_Data_Center.mp4`** — final rendered animation (frames 0–1730)
- **`AI_Data_Center.png`** — key still frame
- `README.md` — this file

The full Blender project file (`.blend`, ~1GB with 4,000+ objects) is available on request.

---

Made with 🧡 in Blender.