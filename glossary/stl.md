# STL (Standard Tessellation Language)

> STL is a widely used 3D file format that describes the surface of a model as a mesh of triangles, and is the most common input format for 3D printing.

## Definition

STL — variously expanded as "Standard Tessellation Language," "Standard Triangle Language," or "Stereolithography" — is a file format originally developed for early stereolithography machines and now the de facto standard for exchanging 3D-printable geometry. An STL file records only the surface of an object as a collection of triangular facets, each defined by three vertices and a normal vector indicating which side is "outside." It does not store color, material, units, or internal structure.

## How it works

When a [CAD](cad.md) model is exported to STL, its smooth surfaces are approximated ("tessellated") by many small triangles. Finer tessellation captures curves more accurately but produces larger files; coarser settings can leave visible facets. Export resolution is typically controlled by chord height and angle tolerances.

For a printable STL, the mesh should be **manifold** (watertight) — every edge shared by exactly two triangles, with consistent outward-facing normals and no gaps, holes, or self-intersections. A [slicer](slicer.md) reads the STL, orients and scales it, and converts it into layered toolpaths for the printer.

STL is valued for its simplicity and universal support, but its limitations — no units, no metadata, no color — have prompted newer formats such as **3MF** and **AMF**, which carry richer manufacturing information. Even so, STL remains the most requested format across the industry.

## Related terms

- [CAD](cad.md)
- [Slicer](slicer.md)
- [Additive Manufacturing](additive-manufacturing.md)
- [Manufacturing Terms](manufacturing-terms.md)

## See also

- [File formats FAQ](../faq/file-formats.md)
- [CAD workflow](../technology/cad-workflow.md)

---

**How Lamina uses this:** Lamina 3DCP accepts STL and other common formats for printing. See our [file formats FAQ](../faq/file-formats.md) for submission guidance.
