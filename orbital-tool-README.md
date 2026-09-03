# 🛰️ Orbital Mission Analysis & Simulation Tool

**Independent Project** | Python, NumPy, Matplotlib | August 2026 – Present

A modular Python-based orbital mechanics simulation and visualization tool for analyzing spacecraft trajectories, orbital maneuvers, ground tracks, and Earth–Moon orbital dynamics.

---

## 🚀 Overview

This project was developed independently outside of coursework to apply orbital mechanics theory to working, interactive software.

The goal is to move beyond hand calculations by implementing the mathematics behind orbital motion, coordinate transformations, maneuver analysis, and cislunar dynamics in Python while providing clear engineering visualizations of the results.

The tool allows users to define or select orbital scenarios, perform orbital calculations, and visualize spacecraft motion through an interactive menu-driven interface.

---

## ✨ Features

### 🌎 2D Orbit Simulation

- Simulates Earth-centered two-dimensional orbital trajectories
- Supports circular and custom tangential-velocity initial conditions
- Calculates orbital characteristics from user-defined inputs
- Checks spacecraft velocity against local escape velocity
- Provides example orbital scenarios for demonstration and testing

### 🛰️ 3D Orbit Simulation

- Generates three-dimensional Earth-centered spacecraft trajectories
- Accepts user-defined Classical Orbital Elements (COEs):
  - Semi-major axis
  - Eccentricity
  - Inclination
  - Right Ascension of the Ascending Node (RAAN)
  - Argument of periapsis
  - True anomaly
- Supports preset equatorial, inclined, polar, and retrograde orbits
- Performs Classical Orbital Element (COE) ↔ state vector conversions
- Visualizes orbital geometry relative to Earth

### 🔥 Hohmann Transfer Analysis

- Calculates Hohmann transfers between circular Earth-centered orbits
- Determines transfer-orbit geometry from initial and final orbital radii
- Visualizes the initial orbit, transfer trajectory, and destination orbit

### 🌐 Ground Track Analysis

- Converts spacecraft position from the Earth-Centered Inertial (ECI) frame to the Earth-Centered Earth-Fixed (ECEF) frame
- Accounts for Earth's rotation during orbital propagation
- Converts spacecraft position into latitude and longitude
- Generates ground-track visualizations over Earth's surface
- Supports multiple orbit types:
  - Equatorial
  - 45° inclined
  - Polar
  - Retrograde
  - Geostationary
  - ISS-like
- Allows ground tracks to be propagated over multiple orbital periods

### 🌕 Earth–Moon Lagrange Point Analysis

- Calculates the five Earth–Moon Lagrange points in the rotating barycentric reference frame
- Determines the collinear L1, L2, and L3 locations
- Determines the triangular L4 and L5 locations
- Visualizes the Earth, Moon, and Lagrange-point geometry in the rotating frame

### 📊 Engineering Visualization

The project includes visualization tools for:

- 2D orbital trajectories
- 3D Earth-centered orbits
- Hohmann transfer trajectories
- Spacecraft ground tracks
- Earth–Moon Lagrange points
- Orbital geometry and reference positions

Visualizations are generated using Matplotlib to make the underlying orbital mechanics easier to interpret and verify.

---

## 🧭 Interactive Interface

The program uses a menu-driven interface that allows users to select different mission-analysis capabilities without modifying the source code for each simulation.

Current analysis options include:

1. 2D Orbit Simulation
2. Hohmann Transfer Analysis
3. 3D Orbit Simulation
4. Ground Track Analysis
5. Earth–Moon Lagrange Point Analysis

Individual analysis modes provide additional presets and custom-input options depending on the selected simulation.

---

## ✅ Validation

Orbital calculations and coordinate transformations are checked against analytical relationships and known orbital scenarios to verify physical consistency.

Validation performed during development includes:

- Circular-orbit velocity calculations
- Escape-velocity comparisons
- Orbital-period calculations
- Classical Orbital Element (COE) ↔ state vector conversion checks
- Inclination recovery from calculated state vectors
- Geostationary orbital behavior
- ISS-like altitude and inclination scenarios
- Earth–Moon Lagrange-point geometry

Additional numerical validation and comparison testing will continue as new capabilities are added.

---

## 🛠️ Tools & Technologies

- **Python** — simulation logic and user interface
- **NumPy** — vector operations, coordinate transformations, and numerical calculations
- **Matplotlib** — 2D/3D orbital and mission visualization
- **Orbital Mechanics** — trajectory, maneuver, reference-frame, and cislunar calculations

---

## 📁 Project Structure

```text
Orbital-Mission-Analysis-Simulation-Tool/
│
├── main.py
├── orbit.py
├── constants.py
├── visualization.py
├── groundtrack.py
├── images/
└── README.md
```

### `main.py`
Controls the interactive program interface and connects the different mission-analysis tools.

### `orbit.py`
Contains core orbital mechanics calculations, orbital propagation functions, state-vector operations, and maneuver-related calculations.

### `constants.py`
Stores physical and orbital constants used throughout the simulation.

### `visualization.py`
Contains plotting and visualization functions for orbital trajectories and mission-analysis results.

### `groundtrack.py`
Handles ECI-to-ECEF transformations and spacecraft ground-track calculations.

### `images/`
Contains selected output plots and visualizations generated by the program.

---

## 📸 Example Visualizations

### 3D Orbit + Ground Track Analysis/Visualization

![3D Orbit Visualization](images/3d-orbit-plot.png)

### Hohmann Transfer
![Hohmann Transfer]()

### J2 Perturbation
![Hohmann Transfer]()

### Propellant Analysis
![Propellant Analysis]()

### Earth-Moon Mission Analysis
![Earth-Moon Mission Analysis]()


### 


Additional Hohmann transfer and Earth–Moon Lagrange-point visualizations will be added as the project documentation develops.

---

## 🔧 Current Development

The Orbital Mission Analysis & Simulation Tool is actively being expanded.

Current and planned development areas include:

- Expanded orbital maneuver analysis
- Improved numerical orbit propagation
- Additional validation and error analysis
- Expanded cislunar mission-analysis capabilities
- Improved 3D orbital visualization
- Additional mission scenarios and orbital presets
- Improved user interaction and output reporting

---

## 🎯 Project Motivation

This project was created to strengthen my understanding of orbital mechanics by translating analytical equations and spacecraft dynamics into functional engineering software.

Rather than treating orbital mechanics only as a set of equations, the project focuses on connecting the underlying physics with numerical implementation, coordinate systems, visualization, and mission-analysis applications.

The long-term goal is to continue developing the tool into a broader spacecraft mission-analysis environment while strengthening my skills in orbital mechanics, spacecraft systems engineering, and scientific programming.

---

## 👤 Author

**Dominick De La Torre**  
B.S. Aerospace Engineering — University of Central Florida  
Expected Graduation: May 2027
