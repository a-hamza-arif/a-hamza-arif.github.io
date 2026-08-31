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

- **Modern kitchen interior** — full white-cabinetry kitchen with a dark stone island/countertop, pendant lighting, glass-front upper cabinets, a stainless-steel fridge, built-in oven, wine rack, and bar stools
- **Espresso machine** — a detailed stainless-and-black countertop espresso maker as the camera's detail-shot subject
- **Coffee canister ("Coffer")** — a ceramic storage canister with a wooden lid, used as the landing point for the bean simulation
- **814 individually simulated coffee beans** — a full rigid-body physics simulation baked to per-object keyframed animation, giving realistic tumbling/settling motion
- **Multi-camera sequence** — 3 cameras covering the wide kitchen establishing view, the espresso-machine detail move, and the coffee-bean close-up

## ⚙️ Technical Details

- **Render engine:** Cycles
- **Objects:** 899 total — 814 of which are individual coffee bean meshes, plus kitchen architecture/furniture, appliances, 3 cameras, and 8 lights
- **Actions:** 841 (the bulk being the per-bean baked rigid-body simulation animation)
- **Materials:** 50
- **Physics:** Blender Rigid Body World simulation, baked to keyframes for reliable/portable playback

## 📸 Deliverables in This Repo

- **`Simple kithcen.mkv`** — final rendered animation (frames 1–432)
- **`Simple kithcen.png`** — key still frame
- `README.md` — this file

The full Blender project file (`.blend`) is available on request.

---

Made with 🧡 in Blender.