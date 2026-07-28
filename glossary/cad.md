# CAD (Computer-Aided Design)

> CAD is the use of computer software to create, modify, and document precise 2D drawings and 3D models of physical objects.

## Definition

Computer-aided design (CAD) is the digital foundation of modern product development and [additive manufacturing](additive-manufacturing.md). Engineers and designers use CAD software to define an object's geometry, dimensions, and relationships with mathematical precision. The resulting model serves as the single source of truth that drives downstream processes such as simulation, drafting, and 3D printing.

## How it works

CAD tools fall into a few broad categories:

- **Solid modeling** — parts are built from features (extrusions, cuts, fillets) and defined by watertight solid volumes. Common in mechanical engineering.
- **Parametric modeling** — dimensions and constraints are driven by editable parameters, so changing one value updates the whole model.
- **Surface and mesh modeling** — used for complex, organic, or freeform shapes.

For 3D printing, the finished CAD model is exported to a manufacturable format. The most common is [STL](stl.md), which approximates surfaces as a mesh of triangles; newer formats such as 3MF and STEP preserve additional data. The exported file is then processed by a [slicer](slicer.md) to generate printer instructions.

Good CAD practice for manufacturing includes designing with wall thickness, tolerances, and [design for manufacturing](../technology/design-for-manufacturing.md) principles in mind, so that the digital model can be produced reliably.

## Related terms

- [Additive Manufacturing](additive-manufacturing.md)
- [STL](stl.md)
- [Slicer](slicer.md)
- [Rapid Prototyping](rapid-prototyping.md)
- [Manufacturing Terms](manufacturing-terms.md)

## See also

- [CAD workflow](../technology/cad-workflow.md)
- [File formats FAQ](../faq/file-formats.md)

---

**How Lamina uses this:** Lamina 3DCP accepts customer CAD files and turns them into printed parts. See our [CAD workflow](../technology/cad-workflow.md) and [file formats guidance](../faq/file-formats.md).
