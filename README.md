# CFD Investigation of a Front Wing in Ground Effect

## Overview
This project presents a steady-state RANS CFD study of a multi-element front wing operating in ground effect. The work focuses on aerodynamic performance, mesh sensitivity, and force and moment convergence using OpenFOAM.

The study is motivated by motorsport front wing aerodynamics, where downforce generation, drag control, and pitching moment behaviour are critical.



## Objectives
- Analyse front wing downforce and drag characteristics
- Assess mesh sensitivity and solution stability
- Study pitching moment behaviour and convergence
- Investigate flow structures using Q-criterion
- Establish a reliable CFD workflow for motorsport applications


## Geometry
- Multi-element front wing with endplates
- Full wing used for baseline simulations
- Half-wing symmetry model planned for parametric studies
- Non-aerodynamic CAD features identified and removed for CFD suitability



## Computational Setup
- Solver: Steady-state incompressible RANS
- Turbulence model: k-omega SST
- Freestream velocity: 50 m/s
- Reynolds number: ~4.5 × 10^5 (based on mean aerodynamic chord)
- Ground model: Moving ground
- Boundary conditions: Velocity inlet, pressure outlet, no-slip walls



## Mesh
- Hex-dominant mesh generated using snappyHexMesh
- Boundary layer refinement with near-wall resolution suitable for SST
- Mesh sensitivity study performed:
  - Fine mesh: ~7–8 million cells
  - Acceptable mesh quality with minimal illegal cells
- Very large meshes (>1.6 million cells) showed degraded mesh quality due to CAD issues



## Results
Key aerodynamic results from the fine mesh case:
- Downforce coefficient shows stable convergence
- Drag coefficient converges smoothly after initial transients
- Pitching moment dominated by pressure contribution
- Viscous contributions to pitching moment are negligible

Force and moment histories demonstrate stable steady-state behaviour.



## Flow Physics
- Strong suction peaks on the lower surfaces of the elements
- Endplate and junction flows contribute significantly to drag
- Q-criterion visualisation highlights coherent vortex structures
- Ground effect accelerates flow beneath the wing, increasing downforce



## Current Limitations
- CAD surface quality limits mesh scalability
- Full-wing simulations are computationally expensive
- Some small non-manifold features remain in the geometry



## Planned Work
- CAD cleanup and removal of non-aerodynamic features
- Half-wing symmetry simulations
- Parametric study of pitch angle
- Parametric study of ride height
- Cl/Cd trends versus pitch angle and ride height
- Improved mesh independence study
- Further flow structure analysis using Q-criterion



## Tools
- OpenFOAM
- ParaView
- MATLAB/Python (post-processing)
- FreeCAD / SALOME (planned CAD repair)



## Author
Saiyed Mudassir  
Aerodynamicist

