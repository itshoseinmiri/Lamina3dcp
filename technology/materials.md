# Materials

> Material families used in additive manufacturing and practical guidance for selecting the right one for prototype and production parts.

Material selection is one of the most consequential decisions in additive manufacturing. The right choice balances mechanical performance, thermal and chemical resistance, surface finish, and cost against the demands of the application and the chosen [printing technology](printing-technologies.md).

## Thermoplastic Filaments (FDM/FFF)

| Material | Key Properties | Typical Uses |
|----------|----------------|--------------|
| **PLA** | Stiff, easy to print, low warp, biodegradable, low heat resistance | Concept models, low-stress prototypes |
| **ABS** | Tough, impact-resistant, higher heat tolerance, prone to warping | Functional prototypes, enclosures |
| **PETG** | Balanced strength and ductility, chemical/moisture resistant | Mechanical parts, fixtures |
| **Nylon (PA)** | High strength, wear-resistant, tough, absorbs moisture | Gears, living hinges, functional parts |
| **TPU** | Flexible, elastic, abrasion-resistant | Gaskets, seals, grips, flexible components |
| **PC (Polycarbonate)** | High strength and heat resistance | Load-bearing, heat-exposed parts |

## Engineering & High-Performance Plastics

Reinforced grades (e.g., carbon-fiber or glass-fiber filled nylon) increase stiffness and dimensional stability for demanding functional and production-grade applications. High-temperature polymers such as PC and PA offer improved thermal performance for parts exposed to heat.

## Photopolymer Resins (SLA/DLP)

- **Standard resins** — high detail, smooth finish; suited to visual models and master patterns.
- **Tough / durable resins** — improved impact and mechanical strength for functional testing.
- **High-temperature resins** — elevated heat deflection for thermal fixtures.
- **Flexible / elastomeric resins** — rubber-like parts.

Note: resins can be brittle and degrade under prolonged UV exposure.

## Powder Materials (SLS/MJF)

Nylon powders (PA11, PA12) produce strong, isotropic, production-grade parts without support structures. PA11 offers greater ductility and impact resistance; PA12 offers fine detail and dimensional consistency. Glass-filled variants add stiffness.

## Selection Guidance

Prioritize requirements in this order:

1. **Mechanical loads** — strength, stiffness, impact, fatigue.
2. **Environment** — temperature, UV, chemicals, moisture.
3. **Tolerance & finish** — detail and surface quality needed.
4. **Quantity & cost** — prototype vs. production economics.
5. **Regulatory / contact** — food, skin, or medical contact considerations.

For functional prototypes, ABS, PETG, and Nylon are common defaults; for production-grade parts, SLS/MJF nylons deliver isotropic strength. See [DFM](design-for-manufacturing.md) for how material choice interacts with geometry.

<!-- TODO: confirm which specific materials Lamina offers -->

## Related

- [Printing Technologies](printing-technologies.md)
- [Design for Manufacturing](design-for-manufacturing.md)
- [Quality Control](quality-control.md)
