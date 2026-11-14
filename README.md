# 🪐 Virtual Solar System (Blender 3D Simulation)

**Course:** Mobile Virtual Reality and Artificial Intelligence  
**Assignment:** SWAYAM Extra Project  
**Project No. & Title:** Project 13 — *Virtual Solar System: Explore planets revolving around the Sun with interactive information.*  
**Platform:** macOS  
**Software:** Blender 5.3  

---

## 📖 Project Overview

This project is a 3D animated model of our Solar System created in **Blender**. It visually demonstrates the Sun, all eight major planets (Mercury, Venus, Earth, Mars, Jupiter, Saturn, Uranus, Neptune), Earth's Moon, Saturn's rings, and their circular orbital paths.

The animation is powered entirely by **native Blender keyframes** and linear interpolation. When you press **`Spacebar`**, the planets revolve around the Sun at proportional speeds (inner planets revolving faster than outer planets, reflecting Keplerian motion) while rotating on their own tilted axes.

---

## 📂 Project Structure

```
Virtual_Solar_System/
├── Virtual_Solar_System.blend     # Main editable Blender 3D project file
├── README.md                      # Project overview and instructions
├── VIVA_PREPARATION.md            # Viva questions, concepts, and presentation script
├── renders/                       # High-resolution rendered preview images
│   ├── solar_system_overview_0001.png
│   └── solar_system_frame50_0050.png
├── animation/                     # Rendered animation frame sequence
│   └── frame_0001.png ... frame_0012.png
└── scripts/                       # Internal build automation script
    └── build_solar_system.py
```

---

## 🌟 Features Included

1. **Main Celestial Objects:**
   * **The Sun**: Central warm glowing sphere with an internal omnidirectional Point Light source illuminating the planets.
   * **8 Major Planets**: Mercury, Venus, Earth, Mars, Jupiter, Saturn, Uranus, and Neptune, with distinct radii and surface colors.
   * **Earth's Moon**: Orbits Earth along with Earth's revolution around the Sun.
   * **Saturn's Rings**: 3D flat circular ring disc with procedural banded transparency.
   * **Circular Orbit Trajectories**: Glowing circular path lines showing each planet's orbit.
   * **3D Planet Labels**: Clean glowing text labels above each planet for immediate identification.
   * **Space Environment**: Dark deep-space world with stars.

2. **Animation (Standard Blender Keyframes):**
   * **Orbital Revolution**: Each planet is childed to a central pivot empty with keyframed Z-rotation and linear cyclic extrapolation.
   * **Axial Rotation (Day/Night)**: Each planet rotates around its own local axis, including retrograde spin for Venus and Uranus.
   * **Axial Tilts**: Realistic tilts (Earth at 23.4°, Uranus on its side at 97.8°, Saturn at 26.7°).

3. **Camera & Presentation:**
   * **`Main_Camera`**: Elevated isometric perspective view capturing the entire system.
   * **Timeline Markers**: Labeled markers at the bottom timeline to quickly jump between celestial bodies.

---

## 🚀 How to Open and Demonstrate in Blender

1. **Open the File:**
   Double-click [**`Virtual_Solar_System.blend`**](file:///Users/adityaarora/Documents/Virtual_Solar_System/Virtual_Solar_System.blend) to open it in Blender.
2. **Viewport Shading:**
   The file is pre-configured to **Material Preview** mode. If needed, click the Material Preview sphere icon at the top-right of the 3D viewport.
3. **Play the Animation:**
   Press the **`Spacebar`** (or click the **`▶` Play button** on the timeline at the bottom).
   All planets will begin revolving smoothly around the Sun.
4. **Inspect Individual Planets:**
   In the top-right Outliner list, click on any planet (e.g. `Planet_Earth` or `Planet_Saturn`), then press **Numpad `.` (Period)** or go to **View > Frame Selected** to zoom in up close.
5. **Timeline Markers:**
   Click on the timeline markers at the bottom (`☀️ Sun`, `🌍 Earth`, `♄ Saturn`) to jump directly to specific points in time.
