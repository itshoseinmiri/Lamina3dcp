# Slicer

> A slicer is software that converts a 3D model into thin horizontal layers and generates the machine instructions a 3D printer follows to build the part.

## Definition

A slicer is the bridge between a digital model and a physical print. It takes a mesh file such as [STL](stl.md), divides the geometry into a stack of horizontal cross-sections ("slices"), and produces a set of machine instructions — most commonly **G-code** — that tell the printer exactly how to move, when to deposit or cure material, and at what speed and temperature. Without slicing, a printer has no way to interpret a 3D model.

## How it works

During slicing, the operator configures print parameters that directly affect quality, strength, speed, and cost:

- **Layer height** — the thickness of each slice; smaller values give finer detail but longer prints.
- **Infill** — the internal fill pattern and density that balances strength against material use.
- **Perimeters/shells** — the number of outer wall passes.
- **Support structures** — temporary scaffolding for overhangs and bridges.
- **Print orientation** — how the part sits on the build plate, affecting strength, surface finish, and support needs.

The slicer also estimates print time and material consumption, letting operators preview and optimize a job before it runs. Popular slicing applications include Cura, PrusaSlicer, and Simplify3D, along with proprietary tools tied to specific machines.

Slicing decisions embody many [design for manufacturing](../technology/design-for-manufacturing.md) trade-offs, which is why experienced operators tune settings per part rather than relying on defaults.

## Related terms

- [STL](stl.md)
- [CAD](cad.md)
- [Additive Manufacturing](additive-manufacturing.md)
- [Manufacturing Terms](manufacturing-terms.md)

## See also

- [Manufacturing process](../technology/manufacturing-process.md)
- [Printing technologies](../technology/printing-technologies.md)

---

**How Lamina uses this:** Lamina 3DCP's operators slice and optimize each job for the chosen material and machine. See our [manufacturing process](../technology/manufacturing-process.md).
