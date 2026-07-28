# Manufacturing Terms

> A quick-reference glossary of common terms used in additive manufacturing and 3D printing.

## Definition

This page collects short definitions of frequently used terms in [additive manufacturing](additive-manufacturing.md). Each entry is a concise, neutral explanation intended as a starting point; follow the [related terms](#related-terms) links for fuller treatment of major concepts.

## DFM (Design for Manufacturing)

The practice of designing a part so it can be produced reliably, economically, and with good quality. In 3D printing, DFM covers wall thickness, overhangs, orientation, and feature sizes suited to the chosen process.

## Infill

The internal structure of a printed part, expressed as a pattern (grid, gyroid, honeycomb) and a density percentage. Higher infill increases strength and weight; lower infill saves material and time.

## Layer height

The thickness of each printed layer, typically 0.05–0.3 mm. Smaller layer heights yield finer detail and smoother surfaces but longer print times.

## Support structures

Temporary scaffolding printed beneath overhangs and bridges to hold material that would otherwise sag or fall. Supports are removed during [post-processing](#post-processing) and can affect surface finish where they attach.

## Tolerance

The allowable deviation between a part's specified dimension and its actual measured dimension. Achievable tolerances depend on the process, material, and part geometry. See the [tolerances FAQ](../faq/tolerances.md).

## Post-processing

Any finishing step performed after printing — support removal, sanding, painting, dyeing, vapor smoothing, machining, or curing — to improve appearance, accuracy, or material properties.

## Build volume

The maximum size of part a printer can produce, defined by the X, Y, and Z dimensions of its build chamber. Parts larger than the build volume must be split and joined.

## Anisotropy

The tendency of printed parts to have different mechanical properties in different directions, usually weaker along the layer (Z) axis because layers are bonded rather than continuous.

## Overhang

A downward-facing surface that extends beyond the layer below it. Steep overhangs (typically past 45°) often require support structures.

## Warping

Distortion caused by uneven cooling and internal stress, where corners or edges lift away from the build plate. Managed through bed adhesion, heating, and material choice.

## Resolution

A measure of the finest detail a printer can reproduce, influenced by layer height (Z) and the smallest movement or spot size in the X–Y plane.

## Related terms

- [Additive Manufacturing](additive-manufacturing.md)
- [Rapid Prototyping](rapid-prototyping.md)
- [CAD](cad.md)
- [STL](stl.md)
- [Slicer](slicer.md)

## See also

- [Design for manufacturing](../technology/design-for-manufacturing.md)
- [Tolerances FAQ](../faq/tolerances.md)
- [Materials](../technology/materials.md)

---

**How Lamina uses this:** Lamina 3DCP applies these principles when reviewing designs and finishing parts. See our [design for manufacturing](../technology/design-for-manufacturing.md) and [quality control](../technology/quality-control.md) pages.
