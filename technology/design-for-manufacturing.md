# Design for Manufacturing (DFM) for Additive

> Design principles that make parts printable, reliable, and cost-effective in additive manufacturing.

Design for Manufacturing (DFM) adapts a design to the realities of the production process. In additive manufacturing, good DFM reduces failed prints, minimizes post-processing, improves strength, and lowers cost — while preserving the part's intended function. The right rules depend on the chosen [printing technology](printing-technologies.md) and [material](materials.md).

## Core DFM Principles

### Wall Thickness
Walls must be thick enough to print reliably and carry load. Too thin, and features fail to form or break during handling. Typical minimums are around 0.8–1.0 mm for FDM and 0.7–1.0 mm for SLS/MJF (general industry figures, not guarantees).

### Overhangs & Support
Overhangs steeper than roughly 45° from vertical usually need support in FDM/SLA. Powder-bed processes (SLS/MJF) self-support and avoid this constraint. Minimize supports to reduce post-processing and surface marks.

### Bridging
Unsupported horizontal spans should be kept short; long bridges sag. Add chamfers or redesign to avoid them.

### Orientation Awareness
FDM and SLA parts are anisotropic — weaker between layers (Z axis). Orient critical loads along the layer plane, and place important surfaces where finish is best.

### Holes & Clearances
Printed holes tend to come out undersized; add tolerance or plan to ream. For assemblies, allow clearance (commonly 0.3–0.5 mm) between mating parts, adjusted for material shrinkage.

### Fillets & Stress Relief
Round sharp internal corners to reduce stress concentration and improve part strength.

### Fine Features
Text, ribs, and pins have minimum printable sizes tied to process resolution. Embossed features print more reliably than engraved ones on FDM.

## Quick Reference (general figures)

| Feature | FDM Guideline | SLS/MJF Guideline |
|---------|---------------|-------------------|
| Min wall thickness | ~0.8–1.0 mm | ~0.7–1.0 mm |
| Min feature size | ~1.0 mm | ~0.5 mm |
| Overhang without support | ≤ 45° | Not required |
| Assembly clearance | ~0.3–0.5 mm | ~0.3–0.5 mm |
| Embossed/engraved detail | ≥ 0.5 mm wide | ≥ 0.3 mm wide |

*Values are typical industry ranges and vary by machine, material, and geometry.*

## Cost-Reduction Strategies

- Reduce part volume and use appropriate infill instead of solid bodies.
- Consolidate assemblies into fewer printed parts.
- Design self-supporting geometry to cut support removal time.
- Nest and orient efficiently to shorten build height.
- Avoid over-tight tolerances that require secondary machining.

## Related

- [Printing Technologies](printing-technologies.md)
- [Materials](materials.md)
- [CAD Workflow](cad-workflow.md)
- [Quality Control](quality-control.md)
