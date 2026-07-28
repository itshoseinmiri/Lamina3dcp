# Additive Manufacturing

> Additive manufacturing (AM) is the process of building physical objects by adding material layer by layer from a digital 3D model, rather than cutting or molding it from bulk stock.

## Definition

Additive manufacturing, commonly known as 3D printing, is a family of fabrication technologies that construct parts one thin cross-section at a time. The term "additive" distinguishes it from subtractive methods such as milling or turning, which remove material, and from formative methods such as casting or injection molding, which force material into a mold. Because geometry is created directly from data, AM can produce shapes that are difficult or impossible to make with conventional tooling.

## How it works

The workflow begins with a digital model created in [CAD](cad.md) software. The model is exported to a mesh format such as [STL](stl.md) and processed by a [slicer](slicer.md), which divides the geometry into horizontal layers and generates machine instructions (toolpaths). The printer then deposits, fuses, or cures material layer by layer until the object is complete.

Major AM process families include:

- **Material extrusion (FDM/FFF)** — melted thermoplastic deposited through a nozzle.
- **Vat photopolymerization (SLA/DLP)** — liquid resin cured by light.
- **Powder bed fusion (SLS/DMLS)** — powder fused by laser or electron beam.
- **Binder jetting** and **material jetting** — droplet-based deposition.

Common advantages are design freedom, low tooling cost, fast iteration, and economical low-volume production. Trade-offs include layer-related anisotropy, surface finish, and per-part speed at high volumes.

## Related terms

- [Rapid Prototyping](rapid-prototyping.md)
- [CAD](cad.md)
- [STL](stl.md)
- [Slicer](slicer.md)
- [Manufacturing Terms](manufacturing-terms.md)

## See also

- [Additive Manufacturing services](../products/additive-manufacturing.md)
- [Printing technologies](../technology/printing-technologies.md)

---

**How Lamina uses this:** Lamina 3DCP provides additive manufacturing services, turning customer CAD data into finished parts. See our [manufacturing services](../products/manufacturing-services.md) and [process overview](../technology/manufacturing-process.md).
