# CAD Workflow

> How a design moves from CAD software to a print-ready file, including the file formats that matter at each step.

A reliable CAD-to-print workflow ensures the geometry the designer intends is exactly what the machine builds. Errors introduced during modeling or export are a common cause of failed prints and dimensional issues, so a disciplined workflow pays off across the whole [manufacturing process](manufacturing-process.md).

## Workflow Stages

1. **Model** — Create the part in parametric CAD (e.g., SolidWorks, Fusion 360, Onshape, Creo) or a mesh/sculpting tool for organic shapes.
2. **Validate** — Check for a closed, watertight solid: no gaps, non-manifold edges, inverted normals, or self-intersections.
3. **Apply DFM** — Adjust wall thickness, fillets, clearances, and features per [Design for Manufacturing](design-for-manufacturing.md).
4. **Export** — Save to a manufacturing format (STEP for solids, STL/3MF for mesh/print).
5. **Slice** — Import into slicing software to generate toolpaths.
6. **Print** — Send the sliced job to the machine.

## Key File Formats

| Format | Type | Strengths | Notes |
|--------|------|-----------|-------|
| **STEP (.step/.stp)** | Solid (B-rep) | Precise geometry, editable, preserves units | Preferred for exchange and re-editing |
| **STL (.stl)** | Triangle mesh | Universal, simple | No units/color; resolution set at export |
| **3MF (.3mf)** | Mesh + metadata | Units, color, materials, print settings | Modern replacement for STL |
| **OBJ (.obj)** | Mesh + texture | Color/texture support | Common for full-color models |
| **IGES (.igs)** | Solid/surface | Legacy CAD exchange | Less robust than STEP |

## STL Export Tips

STL approximates curved surfaces with flat triangles. Export resolution is controlled by two tolerances:

- **Chord / deviation tolerance** — max distance between the mesh and the true surface. Lower = smoother curves.
- **Angle tolerance** — controls facet density on curvature.

Aim for smooth curves without excessive file size — overly fine meshes slow slicing with no visible benefit. A common guideline is a chord tolerance around 0.01–0.05 mm for detailed parts (general figure, not a guarantee).

## Common Pitfalls

- **Non-watertight meshes** — open edges cause slicing errors; repair before export.
- **Inverted normals** — surfaces face inward, confusing the slicer.
- **Wrong units** — millimeter vs. inch mismatches scale the part; STEP/3MF carry units, STL does not.
- **Over-decimated meshes** — faceting becomes visible on the printed surface.

## Related

- [Design for Manufacturing](design-for-manufacturing.md)
- [Manufacturing Process](manufacturing-process.md)
- [Printing Technologies](printing-technologies.md)
