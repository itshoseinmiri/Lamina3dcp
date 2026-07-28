# Quality Control

> Inspection and quality-assurance practices that verify additive manufactured parts meet dimensional and functional requirements.

Quality control (QC) confirms that a finished part matches its design intent and is fit for purpose. In additive manufacturing, QC spans the whole workflow — from validating the incoming file to inspecting the finished part — and is essential for production-grade and functional components. It is the final stage of the [manufacturing process](manufacturing-process.md).

## QC Across the Workflow

- **Pre-print (design/file)** — Verify the model is watertight and manufacturable; confirm material and process selection. See [CAD Workflow](cad-workflow.md) and [DFM](design-for-manufacturing.md).
- **In-process** — Monitor the build for adhesion, warping, layer shifts, and machine health. Some machines log build data for traceability.
- **Post-print** — Inspect dimensions, surface finish, and function after post-processing.

## Inspection Methods

| Method | What It Checks | Tools |
|--------|----------------|-------|
| **Visual inspection** | Surface defects, layer issues, warping | Eye, magnification |
| **Dimensional measurement** | Feature sizes, hole positions | Calipers, micrometers, gauges |
| **Coordinate measurement (CMM)** | High-accuracy dimensional verification | CMM machine |
| **3D scanning** | Full-part deviation vs. CAD | Optical/laser scanner + software |
| **Fit / functional testing** | Assembly, clearances, mechanical function | Mating parts, test rigs |
| **Mechanical testing** | Strength, hardness (destructive) | Tensile/hardness testers |

## Common Defects & Causes

| Defect | Likely Cause |
|--------|--------------|
| Warping / curling | Uneven cooling, poor adhesion, material shrinkage |
| Layer shifting | Mechanical/motion error during build |
| Under-extrusion / gaps | Feed or temperature issues (FDM) |
| Delamination | Weak layer bonding, temperature too low |
| Dimensional drift | Shrinkage, calibration, orientation effects |
| Incomplete cure | Insufficient UV post-cure (SLA/DLP) |

## Tolerances

Achievable tolerances depend on process, material, part size, and geometry. As a general industry reference, FDM and powder-bed processes commonly hold roughly ±0.2–0.5 mm on typical features, while resin processes can achieve tighter results. These are general figures, not guarantees.

<!-- TODO: confirm Lamina's specified/guaranteed tolerances and inspection equipment -->

## Documentation & Traceability

For production work, QC records may include inspection reports, measured-vs-nominal data, material batch records, and process parameters — supporting repeatability and customer sign-off.

## Related

- [Manufacturing Process](manufacturing-process.md)
- [Design for Manufacturing](design-for-manufacturing.md)
- [Materials](materials.md)
- [CAD Workflow](cad-workflow.md)
