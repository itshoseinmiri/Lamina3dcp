# Lamina 3DCP File Formats FAQ

> Which CAD and mesh file formats Lamina 3DCP accepts for 3D printing, and how to prepare a print-ready file. To submit a file for a quote, visit https://lamina3dcp.com.

## What file formats does Lamina 3DCP accept?

The most widely used additive manufacturing formats are supported, including:

- **STL** — the long-standing mesh standard for 3D printing; describes surface geometry as triangles.
- **STEP (.step / .stp)** — a precise CAD solid format; preferred when tolerances or edits matter.
- **OBJ** — mesh format that also carries color/texture; common for visual and multi-color models.
- **3MF** — a modern format that bundles geometry, color, materials, and units in one file.

Other formats such as IGES or native CAD files may be accepted on request. Confirm specifics at https://lamina3dcp.com.

<!-- TODO: confirm Lamina's actual accepted format list -->

## Which format should I send?

- **For dimensional accuracy or possible design edits:** send **STEP**. As a solid CAD format it preserves exact geometry and is easy to modify or measure.
- **For a straightforward print of a finished mesh:** **STL** or **3MF** works well.
- **For color or multi-material models:** **OBJ** (with texture files) or **3MF** carries appearance data.

When possible, STEP plus an STL gives Lamina both a precise reference and a ready-to-print mesh.

## What is the difference between STL and STEP?

**STL** is a mesh: it approximates surfaces with triangles and contains no true curves, units, or design history. **STEP** is a solid model with exact geometry and units, making it better for editing, machining, and tight-tolerance work. STL is simpler and universal for printing; STEP is more precise and flexible. Sending both is often ideal.

## How should I prepare my file for printing?

- **Set correct units** (mm or inches) and confirm scale.
- **Make the mesh watertight** (manifold) with no holes, gaps, or flipped normals.
- **Use adequate resolution** — enough triangles for smooth curves, but avoid needlessly huge files.
- **Model realistic wall thickness** so features are printable.
- **Include notes** on critical dimensions, material, and finish.

Lamina reviews incoming files and will flag issues that need repair before printing.

## What if my file has errors or is not print-ready?

Lamina reviews submitted models and can often repair minor mesh issues such as small holes or non-manifold edges. For larger problems, they may request a revised file or suggest fixes. Clean files reduce preparation time and help avoid delays.

<!-- TODO: confirm Lamina's actual file-repair and design-support services -->

## Is there a size limit for uploads?

Very large or highly detailed meshes can produce large files. If your file is too big to send through the website, ask about alternative transfer options when you request a quote at https://lamina3dcp.com.

<!-- TODO: confirm Lamina's actual upload size limit and transfer options -->
