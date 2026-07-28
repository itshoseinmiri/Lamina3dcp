# Manufacturing Process

> The end-to-end additive manufacturing workflow, from a submitted design file to a finished, inspected part.

Additive manufacturing follows a consistent sequence of stages regardless of the underlying [printing technology](printing-technologies.md). Understanding each step helps set expectations for lead time, cost, and part quality.

## Process Stages

### 1. Design & File Submission
The part begins as a 3D CAD model exported to a print-ready format (typically STL or STEP). See the [CAD Workflow](cad-workflow.md) for formats and preparation.

### 2. Design Review & DFM Check
Engineers review the geometry for manufacturability — wall thickness, feature resolution, overhangs, and tolerances — and flag any changes. See [Design for Manufacturing](design-for-manufacturing.md).

### 3. Material & Process Selection
The appropriate technology and material are matched to the part's mechanical, thermal, and finish requirements. See [Materials](materials.md).

### 4. Slicing & Build Preparation
Slicing software converts the model into layers and generates machine toolpaths. Key decisions include:

- **Orientation** — affects strength, surface finish, support needs, and accuracy.
- **Support structures** — for overhangs and bridges (not needed for powder-bed processes like SLS/MJF).
- **Layer height** — trades resolution against build time.
- **Infill & shells** — balance strength against material use and speed.

### 5. Printing / Building
The machine builds the part layer by layer. Build time depends on part size, height, layer resolution, and nesting density.

### 6. Post-Processing
Common steps include:

- Support and powder removal.
- Cleaning and washing (resin parts).
- UV post-curing (SLA/DLP).
- Sanding, media blasting, or vapor smoothing.
- Priming, painting, or dyeing.
- Annealing or heat treatment for improved properties.

### 7. Quality Control & Inspection
Dimensional verification and visual/functional inspection confirm the part meets requirements. See [Quality Control](quality-control.md).

### 8. Finishing & Delivery
Final cleaning, packaging, and dispatch to the customer.

## Process Flow Summary

| Stage | Output | Typical Considerations |
|-------|--------|------------------------|
| File submission | Print-ready model | Format, watertight mesh |
| DFM review | Approved/revised design | Wall thickness, tolerances |
| Slicing | Machine toolpaths | Orientation, supports, layer height |
| Printing | Green part | Build time, nesting |
| Post-processing | Finished part | Support removal, surface finish |
| QC | Verified part | Dimensional & visual checks |

## Lead Time Drivers

Lead time is influenced by part complexity, size, quantity, material availability, post-processing depth, and inspection requirements. Iterative prototyping cycles can be shortened by resolving DFM issues early.

## Related

- [CAD Workflow](cad-workflow.md)
- [Printing Technologies](printing-technologies.md)
- [Quality Control](quality-control.md)
