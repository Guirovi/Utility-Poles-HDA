# Procedural Utility Pole Generator (Houdini HDA)

A fully procedural utility pole and power line generator built for SideFX Houdini. This Digital Asset (HDA) creates highly customizable transmission corridors and distribution lines driven by layout curves, automatically adapting to terrain surfaces with realistic catenary cable sag, structural crossbeams, insulators, and hardware assemblies.

---

## Key Features

* **Flexible Path Layout:**
  * Distribution options for uniform spacing intervals or original curve point CVs[cite: 1].
  * Procedural curve smoothing to eliminate unnatural sharp transitions along cable spans[cite: 1].
  * Ray-based projection to snap pole roots onto terrain geometry and heightfield surfaces[cite: 1].
  * Dynamic input safety handling using conditional `hasinput()` expressions to prevent node cook errors when external ports are empty[cite: 6, 8, 10].

* **Detailed Procedural Assemblies:**
  * Global uniform scaling and per-axis transform multipliers[cite: 1, 2].
  * Procedural randomization controls for pitch, roll, and yaw to simulate real-world weathering, ground settling, and aging[cite: 1].
  * Multi-tiered crossbeam generation with customizable top margins, vertical spacing, and spans[cite: 2].
  * Structural diagonal support struts with configurable offsets, anchor gaps, and profile widths[cite: 2].
  * Hardware detailing including automatic bolt generation and symmetrical insulator placement[cite: 3].

* **Advanced Cable System:**
  * Automatic multi-span cable connections linked across consecutive insulator contact points[cite: 3, 4].
  * Physical catenary sag calculations with custom center offsets and randomized per-cable sag variations[cite: 4].
  * Multi-wire bundling (*Multicable*) supporting bundle spread, strand counts, and radial twists[cite: 4].
  * Output geometry toggle between swept polygonal tubes (with custom column and segment counts) and lightweight curve primitives for render-time curve rendering[cite: 4].

* **Debug & Viewport Guides:**
  * Dedicated viewport visualizer controls to inspect the guide trajectory and distribution points prior to heavy geometry evaluation[cite: 9].

---

## Installation

1. Clone or download the repository:
   ```bash
   git clone [https://github.com/your-username/houdini-utility-pole-generator.git](https://github.com/your-username/houdini-utility-pole-generator.git)
