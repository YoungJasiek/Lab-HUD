# Lab HUD (2D / HUD / GUI Editor)

[![Engine: Lab](https://img.shields.io/badge/Engine-Lab-blue?style=for-the-badge)](https://github.com/YoungJasiek/Lab)
[![Docs](https://img.shields.io/badge/Docs-Online-green?style=for-the-badge)](https://youngjasiek.github.io/Lab/labhud.html)
[![Repository](https://img.shields.io/badge/GitHub-Lab--HUD-blueviolet?style=for-the-badge)](https://github.com/YoungJasiek/Lab-HUD)

**Lab HUD** is a standalone visual 2D / HUD / GUI layout editor for the **Lab Engine**, featuring an authentic **LabStudio** dark industrial Hammer-style interface, project management, canvas manipulation, transparency support, and native `.labhud` serialization.

---

## 📖 Features & Workflow

### 1. Project Selection
- Instant project switcher upon startup: select existing projects (e.g. **Frozen-Life HUD**), open external `.labhud` files, or create new layouts.

### 2. Interactive 2D Canvas
- Grid snapping, multi-selection (marquee rectangle selection), 8-point bounding box resizing, drag-and-drop widget manipulation, zoom and canvas panning.

### 3. Comprehensive Widget Library
- **Basic**: `Rect`, `Label`, `Image` (custom textures / bitmap assets).
- **HUD**: `HealthBar`, `AmmoCounter`, `Crosshair`, `Icon`.
- **UI**: `Button`, `Card`, `Panel`, `ProgressBar`.

### 4. Property Inspector & Transparency
- Complete control over position, dimensions, RGB color, **alpha / opacity (0.0 – 1.0)**, borders, typography, alignment anchors (`HUDAnchor`), and runtime game data bindings (`player.health`, `player.armor`, `weapon.clip`).

### 5. Custom Asset Browser
- Built-in browser scanning `assets/hud_assets/` for custom sprites and textures with real-time thumbnail previews.

### 6. Plain-Text Serialization
- Native read and write of `.labhud` files using the Lab Engine section-based token format (`METADATA`, `ASSETS`, `ELEMENTS`).

---

## 🚀 Building and Running

```powershell
cd apps/labhud
mkdir build
cd build
cmake .. -A x64
cmake --build . --config Debug
.\Debug\LabHUD.exe
```

---

## 👤 Author & Acknowledgments
* **Creator & Architect:** [YoungJasiek](https://github.com/YoungJasiek)
* **Special Thanks:** Sincere gratitude to **Valve Corporation** for their iconic Source Engine and Hammer tool philosophy inspiring LabStudio and Lab HUD.
