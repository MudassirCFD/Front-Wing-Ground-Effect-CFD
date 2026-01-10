# CAD Preparation Notes

This directory contains the geometry used for the CFD investigation of a
multi-element front wing operating in ground effect.

The CAD preparation focused on producing a watertight, consistently scaled
geometry suitable for meshing with OpenFOAM snappyHexMesh.

## Original geometry
- Full multi-element front wing CAD model
- Geometry required minor repair operations prior to CFD use
- Initial geometry scale was inconsistent and required correction
- Used as the baseline reference for all subsequent modifications

## Cleaned geometry
- Geometry repaired to ensure a fully watertight surface
- Scaled consistently into SI units (meters)
- Simplified where necessary to improve mesh robustness
- Prepared specifically for snappyHexMesh surface and volume meshing

## Notes
- No aerodynamic features were intentionally modified during cleaning
- Geometric changes were limited to repair and scaling operations
- Further simplification may be applied if mesh quality issues arise

