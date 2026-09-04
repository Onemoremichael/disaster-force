# Systems architecture: the Resilience Arsenal

## Design judgment

The Department of Resilience should not procure a catalog of independent heroic machines. It should create a **Resilience Arsenal**: interoperable families of purpose-built systems that move mass, energy, information, patients, and work through damaged environments.

The design object is a mission thread:

```text
sense → decide → enter → produce → connect → distribute → sustain → repair → transfer
```

Every major platform is a node in that thread. The platform is accepted only if it improves net delivered effect after its own lift, fuel, crew, maintenance, protection, waste, and reception burdens are counted.

## Why purpose-built matters

Conversions can be sensible experiments or surge measures. They are unacceptable as the governing industrial strategy because the original vehicle's structure, loading, internal flow, corrosion protection, flight or seakeeping envelope, maintenance access, energy system, and crew arrangement were optimized for another mission.

The evidence is clearest in fire aviation. A Forest Service review found that legacy aircraft had not been designed for the severe low-speed, low-altitude, structurally demanding firefighting environment.[^fs-airworthiness] GAO later documented an aging and uncertain fleet assembled through contracts and transfers rather than a stable purpose-built acquisition pipeline.[^gao-fire-aviation] A peer establishment would specify the mission loads, instrument prototypes, test fatigue and corrosion, and build an enduring production and support system from the outset.

Purpose-built does not mean unique everywhere. Common engines, pumps, power electronics, avionics, medical equipment, connectors, software, and structural modules should be used wherever they reduce cost without degrading mission performance.

## The system-of-systems map

| Family | Core effect | Principal systems |
|---|---|---|
| Observe and coordinate | Trusted common operating picture and command | satellites, high-altitude persistence, uncrewed sensing, field survey, deployable edge/cloud, resilient networks |
| Enter and receive | Open damaged theaters and create throughput | strategic air and sealift, short-field and vertical lift, port opening, landing craft, amphibious logistics, route-clearance and reception systems |
| Water and sanitation | Potable/process water at user; waste safely removed | treatment trains, desalination, pumping, storage, pipeline, distribution, laboratories, wastewater and residuals systems |
| Energy and thermal safety | Critical loads and safe indoor conditions | mobile generation, storage, microgrids, substations, grid repair, rapid conductors, district heating/cooling and clean-air systems |
| Fire and hazard control | Reduce active hazard intensity and spread | purpose-built aircraft, rotorcraft, uncrewed systems, engines, dozers, pumps, barriers, sensing and ground integration |
| Access and public works | Restore mobility and create temporary civil infrastructure | debris systems, earthmoving, bridges, roads, ports, airfields, modular utilities, housing and public facilities |
| Health protection | Complete care pathway and public-health continuity | clinical modules, hospital campuses and ships, patient movement, laboratories, oxygen, pharmacy, sterilization and workforce support |
| Community stabilization | Sustain and transition affected populations | shelter/housing, feeding, sanitation, public-service access, schools, commerce, logistics and civil interface |
| Sustain and regenerate | Keep every family operating | depots, mobile maintenance, fuel and energy, spares, calibration, contamination control, crew replacement and industrial production |

## Common physical architecture

### Three module scales

The Arsenal should standardize three approximate logistics scales while allowing larger fixed assemblies:

1. **Human-portable / pallet:** carried by a small team or common aircraft pallet; first entry, survey, communications, clinical, sensing, control and repair.
2. **Road-mobile / container:** compatible with common road, rail, air and maritime handling; the default scale for treatment, power, pumps, workshops, shelter, laboratories and distribution.
3. **Heavy mission module:** oversize but deliberately bounded for strategic lift, roll-on/roll-off ships, barges and heavy transport; used when efficiency or structural duty makes containerization false economy.

ISO container geometry is a transport interface, not a requirement that equipment remain inside a box while operating. Modules may unfold, telescope, connect or use container-compatible frames.

### Controlled interfaces

The Department should publish open interface standards for:

- low-, medium- and selected high-voltage electrical connection;
- AC and DC microgrid buses, protection, grounding and synchronization;
- potable, raw, wastewater, fuel and process-fluid couplings;
- data identity, telemetry, cyber trust, time and geospatial reference;
- mechanical lifting, tie-down, rail, road, aircraft and vessel handling;
- medical gases, clinical data, pharmacy and patient tracking;
- autonomous-system command, geofencing and safe fallback;
- waste, concentrate and contaminated-material transfer; and
- mission-module status and readiness reporting.

Standards should define the boundary and safety case, not mandate one vendor's internal design.

## Common digital architecture

Every system should be able to operate in four modes:

- **connected:** national cloud and full backhaul;
- **degraded:** intermittent backhaul with local control;
- **isolated:** no external network, local identity and data synchronization queue; and
- **manual safe state:** essential operation without proprietary cloud, remote license or continuous positioning signal.

NIST research on deployable public-safety networks emphasizes coverage, standalone operation, multiple backhaul options, power, interoperability and rapid power-on.[^nist-deployable] The Department should generalize those requirements to every digital system. A water plant, microgrid or hospital that cannot operate through a communications outage is not disaster equipment.

## Autonomy doctrine

Autonomy is used to change exposure, scale or tempo—not to remove accountable command.

High-value applications include:

- persistent mapping through smoke, flood, darkness and damaged infrastructure;
- inspection of power lines, bridges, pipelines, levees, structures and contamination;
- repetitive cargo shuttle over a controlled route;
- dozing, trenching, pumping, fireline and debris work in lethal conditions;
- coordinated placement of lightweight cable, hose, sensors and markers;
- inventory, warehouse and depot handling; and
- decision support for routing, load allocation and maintenance.

Humans retain authority over clinical care, evacuation priority, destructive demolition, water release, grid energization, fire mission approval and other actions with major life-safety or rights consequences.

### The mass constraint

Drones do not abolish logistics. Water weighs one metric ton per cubic meter; power cable, pipe, pumps, anchors and structural components impose their own mass and force requirements. Aerial drones may pull pilot lines, survey routes and carry small fittings. Ground robots, barges, helicopters or crewed construction systems must usually place the heavy line, join it, pressure-test it and repair it.

## Survivability without combat design

The relevant threats are fire, heat, cold, salt, ash, smoke, water, debris, vibration, contaminated material, disease, cyber failure, loss of positioning, long storage and irregular maintenance. Systems require:

- floodable or washable lower spaces where appropriate;
- corrosion and ash protection;
- filters and cooling sized for smoke, dust and heat;
- accessible field maintenance;
- redundant safe shutdown;
- protected crew rest and sanitation;
- operation with common or multiple fuels where technically sound;
- low-signature or hardened modes only when international security requires them; and
- design-life instrumentation that records actual mission loads.

Armor, weapons and combat survivability are not default requirements. Their mass and cost would directly reduce civil payload.

## Product-line strategy

Each system family should have a controlled product line rather than one universal platform:

- **rapid:** low mass, high readiness, first effect;
- **regional:** balanced capacity and mobility;
- **strategic:** maximum sustained output and efficiency;
- **austere:** independent entry and operation;
- **urban:** low noise/emissions, tight geometry and high interface density; and
- **contaminated:** sealed, washable and remotely operable.

Common cores and interfaces limit proliferation. Variants exist only when access, duty cycle or safety differs materially.

## Make, buy and mobilize

The Department should classify each capability:

| Class | Ownership logic |
|---|---|
| Sovereign core | Government-owned systems and crews when absence would break the national concurrency promise |
| Assured industrial | Privately operated but contractually dedicated, exercised and visible capacity with priority rights |
| Mobilization reserve | Equipment, tooling and workforce activated at RC-4/5; not counted in immediate readiness |
| Commercial common | Ordinary market capacity used when actually available; excluded from assured floor |
| Allied pool | Co-owned or interoperable capacity governed by treaty or standing agreement |

The decision depends on correlated demand, market depth, readiness time, technical uniqueness, safety authority and industrial fragility—not an ideological preference for public or private operation.

## Technical maturity gates

Major programs pass seven gates:

1. **Need:** quantified unmet effect and time value.
2. **Alternatives:** mitigation, repair, evacuation, distributed systems, contracting and non-platform options compared.
3. **Thread:** complete entry-to-transfer mission architecture.
4. **Physics:** mass, energy, flow, heat, structural, clinical and environmental balances close.
5. **Prototype:** instrumented operation in realistic conditions.
6. **Formation:** crews, maintenance, lift, bases, training, spares and rotation demonstrated.
7. **Production:** cost, supply chain, second source, depot and recapitalization plan validated.

Renderings belong after Gate 4. Procurement belongs after Gate 6.

## Initial system families admitted to concept design

The mission work supports concept development—not procurement—for:

- distributed emergency water systems and a coastal strategic water-energy platform;
- critical-load microgrid and rapid distribution families;
- purpose-built initial-attack, sustained-attack and heavy fire aviation;
- high-volume flood control, amphibious access and autonomous earthworks;
- rapid bridge, port and logistics-node restoration;
- modular ground, maritime and airborne medical systems;
- multi-scale strategic and theater mobility;
- resilient communications, sensing and edge-compute layers; and
- common robotic survey, handling and hazardous-work families.

The following documents define these concepts and the limits that keep them from becoming technological spectacle.

[^fs-airworthiness]: U.S. Forest Service, [*Federal Aerial Firefighting: Assessing Safety and Effectiveness*](https://www.fs.usda.gov/sites/default/files/media_wysiwyg/fed.aerial.ff_.assessing.safety.effectivenss.brp_.2002.pdf), December 2002.
[^gao-fire-aviation]: U.S. Government Accountability Office, [*Wildland Fire Management: Improvements Needed in Information, Collaboration, and Planning to Enhance Federal Fire Aviation Program Success*](https://www.gao.gov/products/gao-13-684), GAO-13-684, August 2013.
[^nist-deployable]: National Institute of Standards and Technology, [*Public Safety 700-MHz Broadband Deployable Systems*](https://www.nist.gov/programs-projects/public-safety-700-mhz-broadband-deployable-systems), updated March 26, 2025.
