# Procedural Utility Pole Generator (Houdini HDA)

A fully procedural utility pole and power line generator built for SideFX Houdini. This Digital Asset (HDA) creates highly customizable transmission corridors and distribution lines driven by layout curves, automatically adapting to terrain surfaces with realistic catenary cable sag, structural crossbeams, insulators, and hardware assemblies.

[![Utility Pole Generator - HDA Houdini](https://img.youtube.com/vi/VqubYc91Zc8/0.jpg)](https://www.youtube.com/watch?v=VqubYc91Zc8)

[link to Video]("[https://example.com/my-link "link title](https://www.youtube.com/watch?v=VqubYc91Zc8)")

---

## Key Features

* **Flexible Path Layout:**
  * Distribution options for uniform spacing intervals or original curve point CVs
  * Procedural curve smoothing to eliminate unnatural sharp transitions along cable spans
  * Ray-based projection to snap pole roots onto terrain geometry and heightfield surfaces
  * Dynamic input safety handling using conditional `hasinput()` expressions to prevent node cook errors when external ports are empty

* **Detailed Procedural Assemblies:**
  * Global uniform scaling and per-axis transform multipliers
  * Procedural randomization controls for pitch, roll, and yaw to simulate real-world weathering, ground settling, and aging
  * Multi-tiered crossbeam generation with customizable top margins, vertical spacing, and spans
  * Structural diagonal support struts with configurable offsets, anchor gaps, and profile widths
  * Hardware detailing including automatic bolt generation and symmetrical insulator placement

* **Advanced Cable System:**
  * Automatic multi-span cable connections linked across consecutive insulator contact points
  * Physical catenary sag calculations with custom center offsets and randomized per-cable sag variations
  * Multi-wire bundling (*Multicable*) supporting bundle spread, strand counts, and radial twists
  * Output geometry toggle between swept polygonal tubes (with custom column and segment counts) and lightweight curve primitives for render-time curve rendering

* **Debug & Viewport Guides:**
  * Dedicated viewport visualizer controls to inspect the guide trajectory and distribution points prior to heavy geometry evaluation

---
