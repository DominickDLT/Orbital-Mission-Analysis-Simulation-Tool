# 🛰️ Orbital Mission Analysis & Simulation Tool

**Independent Project** | Python, NumPy, Matplotlib | August 2026 – Present

A modular Python-based orbital mechanics simulation and visualization tool for analyzing spacecraft trajectories and Earth-centered orbital motion.

---

## Overview

This tool was built independently, outside of coursework, to apply orbital mechanics theory to working, visual, interactive code — going beyond hand calculations to build something that can propagate, transform, and visualize real orbital scenarios.

## Features

### Orbit Propagation
- 2D and 3D orbit propagation for arbitrary Earth-centered orbits
- Classical Orbital Element (COE) ↔ state vector conversions

### Maneuver Analysis
- Hohmann transfer calculations between orbits

### Ground Track Generation
- ECI-to-ECEF coordinate transformations accounting for Earth's rotation
- Ground track (latitude/longitude) generation for multiple orbit types:
  - Equatorial
  - Polar
  - Inclined
  - Retrograde
  - Geostationary
  - ISS-like

### Cislunar Analysis
- Earth–Moon Lagrange point calculations

### Visualization
- 3D spacecraft trajectory plots
- Ground track maps
- Transfer orbit visualization
- Earth–Moon Lagrange point plots
- User-selectable mission parameters (orbit type, altitude, inclination, etc.)

![3D Orbit Visualization](images/3d-orbit-plot.png)
![Ground Track Example](images/ground-track-example.png)
*Add: screenshots of your actual tool output*

## Validation

Orbit propagation and transformation outputs were checked against known analytical results and reference orbital parameters (e.g., ISS altitude/inclination, geostationary period) to confirm physical correctness before trusting the tool's output.

## Example Usage

```python
# Add a real usage example once your code structure is finalized, e.g.:
from orbit_sim import OrbitPropagator

orbit = OrbitPropagator(altitude=400, inclination=51.6, orbit_type="ISS-like")
orbit.propagate(duration_hours=24)
orbit.plot_ground_track()
```

## 🛠️ Tools Used
`Python` `NumPy` `Matplotlib`

## 📁 Repo Contents
- `orbit_sim/` — core simulation modules (propagation, transformations, maneuvers)
- `examples/` — example scripts for each orbit type
- `images/` — sample visualizations
- `README.md` — this file
