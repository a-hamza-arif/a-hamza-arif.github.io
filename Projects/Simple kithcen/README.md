# Simple Kitchen & Coffee Beans Animation (Blender / Cycles)

An architectural-interior animation of a modern kitchen, closing in on an espresso machine and a coffee canister filled via a **baked rigid-body simulation of 800+ individually tumbling coffee beans**. Modeled and rendered entirely in Blender using **Cycles**.

---

## 🎬 Overview

| | |
|---|---|
| **Tool** | Blender, Cycles render engine |
| **Scene** | Single scene, multi-camera edit |
| **Frame Range** | 1–432 |
| **FPS** | 24 |
| **Duration** | 18 sec |
| **Resolution** | 1920×1300 |
| **Audio** | None |

## ☕ What's in the Scene

- **Modern kitchen interior** — full white-cabinetry kitchen with a dark stone island/countertop, pendant lighting, glass-front upper cabinets, a stainless-steel fridge, built-in oven, wine rack, and bar stools, all sitting on a glossy hardwood floor
- **Espresso machine** — a detailed stainless-and-black countertop espresso maker as the camera's detail-shot subject
- **Coffee canister ("Coffer")** — a ceramic storage canister with a wooden lid, used as the landing point for the bean simulation
- **814 individually simulated coffee beans** — a full **rigid-body physics simulation** baked to per-object keyframed animation (each bean has its own baked action), giving realistic tumbling/settling motion as the beans fill the canister
- **Multi-camera sequence** — 3 cameras covering the wide kitchen establishing view, the espresso-machine detail move, and the coffee-bean close-up, with additional handheld-style shake layered on the camera motion for a more organic, commercial feel

## ⚙️ Technical Details

- **Render engine:** Cycles
- **Objects:** 899 total — 814 of which are individual coffee bean meshes, plus kitchen architecture/furniture, appliances, 3 cameras, and 8 lights
- **Actions:** 841 (the bulk being the per-bean baked rigid-body simulation animation)
- **Materials:** 50
- **Physics:** Blender Rigid Body World simulation, baked to keyframes for reliable/portable playback without needing to re-simulate
- **Collections:** organized into `Kitchen`, `Coffee maker`, `Coffer`, `Teapot`, `Beans`, `Camera`, `RigidBodyWorld`/`RigidBodyConstraints`, and `Plane`/`Group` helper collections

## ▶️ How to Open / Render

1. Open `Final.blend` in Blender.
2. The full sequence runs frames **1–432** at 24fps (18s exactly).
3. The bean simulation is already **baked to keyframes**, so it will play back and render correctly without needing to re-run or re-bake the physics.
4. `Render → Render Animation` to reproduce the full sequence, or scrub the timeline and `Render → Render Image` for a single still.
5. No audio track — this is a silent architectural/product animation; add music/SFX in post if desired.

## 📁 Repo Contents

```
.
├── Final.blend         # Main Blender project file (kitchen + baked bean simulation)
├── 0001-0432.mkv          # Rendered animation (frames 1–432)
├── frames/                  # Rendered image sequence
└── README.md
```


Made with 🧡 in Blender.
