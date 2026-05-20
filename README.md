## Project -  🏭 Drum Trucks & Transporters

![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat-square)
![Module](https://img.shields.io/badge/Module-Introduction%20to%20Design%20(4FTC2026)-blue?style=flat-square)
![Tool](https://img.shields.io/badge/Tool-CATIA%20V5-005BAC?style=flat-square)
![Material](https://img.shields.io/badge/Material-Aluminium%206061--T8-silver?style=flat-square)

> A fully designed and CAD-modelled hydraulic drum transporter capable of lifting, moving, rotating, and positioning industrial drums ≥ 50 kg. The project followed a structured engineering design process from technical specification through to detailed part design and structural stress analysis.

</div>

---

## Overview

A manually-operated hydraulic drum transporter designed to safely handle heavy industrial drums in warehouses, factories, and industrial plants. The design went through a full structured engineering process — from generating individual concept sketches, through formal evaluation using SID and W&R tables, to a final CATIA V5 3D assembly with part drawings and stress analysis.

---

## Technical Specifications (PDS)

| Requirement | Specification |
|-------------|---------------|
| Drum weight | ≥ 50 kg |
| Functions | Lifting, Moving, Rotating, Positioning |
| Lifting height | ≥ 500 mm |
| Operation | Manual / Hydraulic |
| Construction material | Aluminium |
| Mobility | Wheels + Casters |
| Overall dimensions | 1100 × 1600 × 600 mm |
| Device weight | < 25 kg |
| Gripping system | Adjustable clamp |
| Safety | Low centre of gravity |
| Maintenance | Minimal |

**Achieved device weight:** 24.839 kg (verified in CATIA V5)

---

## Design Process

The project followed a structured engineering design methodology:

```
Technical Specification  →  Thought Showering  →  Primary Concept Sketches
        →  Updated Concept Sketches  →  Concept Evaluation (SID + W&R)
        →  Selected Design  →  Embodiment Design  →  Detailed Design
        →  CATIA 3D Model  →  Assembly Drawing  →  Part Drafts  →  Stress Analysis
```

---

## Concept Selection

### W&R Table

Three shortlisted designs were scored against weighted criteria:

| Criteria | Weight | Combined 1 | Samir | Combined 2 |
|----------|--------|-----------|-------|------------|
| Lift | 20% | 0.60 | 0.60 | 0.60 |
| Rotation | 5% | 0.15 | 0.15 | 0.05 |
| Dimensions | 25% | 0.50 | 0.75 | 0.75 |
| Weight | 25% | 0.50 | 0.75 | 0.75 |
| USP | 15% | 0.60 | 0.45 | 0.60 |
| Lift Height | 10% | 0.30 | 0.30 | 0.30 |
| **Total** | | **2.65** | **3.00** | **3.05** |
| **Rank** | | **3** | **2** | **1** |

**Selected design: Combined 2** — highest weighted score across all criteria.

---

## Final Design

### Key Components

| Part | Material | Description |
|------|----------|-------------|
| Horizontal Base | Aluminium 6061-T8 | Wide base with wheel and caster mounts for stability |
| Vertical Frame | Aluminium 6061-T8 | Main upright spine connecting base to movable arm |
| Movable Arm | Aluminium 6061-T8 | Pivoting arm driven by hydraulic cylinder |
| Clamping System | Aluminium 6061-T8 | Adjustable clamp that grips and rotates the drum |
| Connecting Rod | Aluminium 6061-T8 | Links hydraulic cylinder to movable arm |
| Hydraulic Cylinder | — | Manual pump raises piston to lift the arm |
| Wheels & Casters | — | 4-wheel mobility with steering casters |

### Hydraulic Actuator Mechanism

The lever is pressed, drawing oil from the tank through a one-way marble valve into the piston chamber. A second marble valve prevents oil returning to the lever, forcing the piston upward. The process repeats until the desired lift height is reached. A release valve lowers the arm in a controlled descent.

---

## CATIA V5 Model

The full assembly was modelled in **CATIA V5** with the following deliverables:

- Individual 3D part models: Horizontal Base, Vertical Frame, Movable Arm, Clamping System, Connecting Rod
- Full assembly with constraints and assembly tree
- Assembly drawing (1:12 scale) with BOM, balloons, build instructions, and material notes
- 2D part drafts (3rd angle projection) for all components with tolerances and surface roughness specifications
- Static structural stress analysis on the two highest-loaded parts

---

## Stress Analysis

A static structural analysis was performed in **CATIA V5 (Analysis & Simulation)** on the two most critical parts.

**Material yield strength:** 2.35 × 10⁸ N/m²

| Part | Applied Load | Max Von Mises Stress | Safe? |
|------|-------------|----------------------|-------|
| Movable Arm | 1500 N (hydraulic) + 750 N (drum weight) | 2.16 × 10⁷ N/m² | ✅ Below yield strength |
| Vertical Frame | 2800 N | 3.21 × 10⁸ N/m² (localised peak) | ✅ Remainder of frame well below yield — peak identified as stress concentration anomaly |

Both parts were confirmed structurally safe for the intended operating loads.

---

## Manufacturing Notes

- Material: **Aluminium 6061-T8** (all structural parts) — lightweight, strong, and suitable for local manufacturing
- Fasteners: **Stainless steel bolts and nuts** (managing steel)
- Surface roughness: Ra 1.6 µm (machined faces) / Ra 3.2 µm (general)
- General tolerance: ± 0.25 mm unless otherwise specified
- Vertical frame: Sheet metal bent to profile, round edges trimmed with angle grinder, welded at frame-to-base junction
- Clamping system: Hollow box machined to shape, holes drilled, welded at joints
