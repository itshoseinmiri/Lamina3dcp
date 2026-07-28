# 3D Printing Technologies

> Overview of the additive manufacturing (AM) processes used across the industry, how they build parts layer by layer, and where each excels.

Additive manufacturing builds parts by depositing or solidifying material one layer at a time directly from a 3D model. Unlike subtractive machining, no material is cut away, which enables complex geometries, internal channels, and rapid iteration. Different AM processes trade off speed, accuracy, surface finish, and material properties.

## Major Process Families

- **FDM / FFF (Fused Deposition Modeling / Fused Filament Fabrication)** — Extrudes molten thermoplastic filament along a toolpath. Cost-effective, robust engineering plastics, good for functional prototypes and jigs. Visible layer lines; anisotropic strength (weaker along the Z axis).
- **SLA (Stereolithography)** — Cures liquid photopolymer resin with a UV laser. Excellent fine detail and smooth surfaces; ideal for master patterns and visual models. Resins can be brittle and UV-sensitive.
- **DLP (Digital Light Processing)** — Similar to SLA but flashes an entire layer at once using a digital projector, so it is faster than laser-based SLA at comparable resolution.
- **SLS (Selective Laser Sintering)** — Fuses nylon-based powder with a laser. No support structures needed (the powder bed self-supports), producing strong, isotropic, production-grade parts.
- **MJF (Multi Jet Fusion)** — Jets fusing and detailing agents onto a powder bed, then applies heat. Fast, consistent, strong nylon parts with fine feature control; a strong choice for functional end-use production.
- **Material Jetting (PolyJet)** — Jets and cures resin droplets, enabling multi-material and full-color parts with very smooth finishes.

## Comparison Table (general industry figures)

| Process | Materials | Typical Layer Height | Relative Accuracy | Surface Finish | Best For |
|---------|-----------|----------------------|-------------------|----------------|----------|
| FDM/FFF | Thermoplastics (PLA, ABS, PETG, Nylon, TPU) | 0.1–0.3 mm | Medium | Layer lines visible | Functional prototypes, jigs, low cost |
| SLA | Photopolymer resins | 0.025–0.1 mm | High | Smooth | Fine detail, master patterns |
| DLP | Photopolymer resins | 0.025–0.1 mm | High | Smooth | Detail at higher speed |
| SLS | Nylon powders (PA11, PA12) | 0.1 mm | High | Slightly grainy | Strong, isotropic functional parts |
| MJF | Nylon powders | 0.08 mm | High | Consistent, grainy | Production runs, functional parts |
| Material Jetting | Resins (multi-material) | 0.014–0.03 mm | Very high | Very smooth | Multi-color, multi-material models |

*Values are typical industry ranges, not guarantees.*

<!-- TODO: confirm which of these processes Lamina offers in-house -->

## Selecting a Process

Choose based on required accuracy, mechanical loads, surface finish, quantity, and budget. See [Materials](materials.md) for material-driven selection and [Design for Manufacturing](design-for-manufacturing.md) for process-specific design rules.

## Related

- [Materials](materials.md)
- [Manufacturing Process](manufacturing-process.md)
- [Design for Manufacturing](design-for-manufacturing.md)
