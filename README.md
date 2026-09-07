# Engine Connecting Rod — SolidWorks CAD Design

A complete mechanical design project: parametric 3D modeling, assembly, and manufacturing drafting of a diesel engine connecting rod, built in SolidWorks.

![Exploded View](images/exploded_view.png)

## Overview

This project models a connecting rod for a medium-duty diesel engine, designed using standard mechanical design proportion ratios. It covers the full CAD workflow — individual part modeling, assembly with proper mates, material assignment, and a dimensioned 2D manufacturing drawing.

## Components

| Part | Description |
|------|-------------|
| **Small End** | Hollow bushing (40mm OD, 28mm bore) — connects to the piston pin |
| **Shank** | I-section beam (30×34mm cross-section) — connects small end to big end, sized for buckling resistance under compressive load |
| **Big End** | Split ring (80mm OD, 55mm bore) — split into rod and cap halves with bolt holes, designed to assemble around the crankshaft journal |

## Key Design Decisions

- **I-section shank**: Chosen over a solid round/rectangular section for the best strength-to-weight ratio, resisting buckling under combustion-driven compressive loads while minimizing reciprocating mass.
- **Split big end**: The big end must wrap around a continuous crankshaft journal, so it's split into a rod half and a bolted cap half — a closed ring couldn't be assembled around the shaft.
- **Assembly mates**: Concentric mates align the circular axes between the shank's stub features and the small/big end bores, Coincident mates fix axial position, and Lock rotation prevents free spinning — resulting in a fully constrained ("Fully Defined") assembly.

## Specifications

- **Material**: Plain Carbon Steel
- **Assembly mass**: ~1.74 kg
- **Overall length**: 160 mm

## Files

- `parts/` — Individual SolidWorks part files (.SLDPRT)
- `assembly/` — Assembly file (.SLDASM)
- `drawings/` — Dimensioned manufacturing drawing with Bill of Materials (.SLDDRW)
- `images/` — Renders and screenshots

## Drawing

![Manufacturing Drawing](images/drawing_sheet.png)

## Tools Used

- SolidWorks (Design Standard, 2026)

## Status

Design and assembly complete. Structural stress analysis (Ansys) in progress.

## Author

Deepak Singh — Mechanical Engineering, KNIT Sultanpur
