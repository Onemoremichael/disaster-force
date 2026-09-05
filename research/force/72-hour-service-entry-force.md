# The 72-hour Service Entry Force

> **Configuration note:** this paper establishes the six-cell architecture. Pass 28's [public-service pod configuration](service-entry-pod-configuration.md) supersedes its continuously divisible mass timing with whole-pod credit: bridge/reuse closes the worst two-cell-loss case at hour 63, independent-essential at hour 71, and full substitution fails at hour 72.

## Executive judgment

Pass 26 found that Cascadia campaign failure concentrates in the first 72 hours. A cellular mesh improved modeled campaign closure from 5.8 percent to 84.2 percent, but seventy-five of its seventy-nine failed trials first broke at day-three force closure. This paper therefore asks a narrower and harder question: **what standing force must exist if the first complete public-service package is required to survive the loss of any two entry formations and still close within 72 hours?**

The answer is not a fleet of heroic platforms. It is a **six-cell Service Entry Force**: two independently originated upland cells, two air cells and two offshore cells. Each cell carries 30 percent of every service effect in the Pass 25 first wave, plus its own command, responder base, energy, data, repair, safety authority and civil interface. Any four surviving cells therefore provide 120 percent of the reference effect.

The modeled force contains 177,670 tonnes across six cells, or 29,612 tonnes per cell. Under the declared throughput assumptions, all fifteen two-cell-loss cases close the balanced service package by hour 60 on a six-hour decision grid. Upland cells complete by hour 30.4, air cells by hour 62.2 and offshore cells by hour 65.2. The timing result depends on a consequential new technology: **service-kernel packaging**, in which every arriving tranche carries a proportional share of all essential effects. Without it, tonnes delivered are not a defensible proxy for services restored.

The architecture allocates a maximum 15-percent loss probability to each genuinely independent cell and 0.2 percent to campaign-wide common-mode loss. Under a simple binomial independence model, those allocations yield 95.076-percent campaign assurance. That number is a requirement budget, not a forecast. It is deliberately narrow and should be withdrawn if origins, crews, fuel, software, parts, technical authorities or providers are found to create hidden covariance.

This force cannot be assembled from mature commercial equipment. It implies a civil X-plane capable of a 120-tonne average mission payload into austere operations; ready sea lifters built around service-kernel loads; sustained 1,100-tonne-per-hour no-pier transfer; autonomous cross-docking and damaged-network distribution; rapid machine-assisted inspection and lawful release; and cell-scale deployable utility islands. NASA is already researching automation, vehicles, landing infrastructure and airspace for emergency advanced air mobility, but at a much smaller mission scale. DARPA's completed Liberty Lifter research explicitly examined ship-scale disaster response at air speed, yet stopped after simulation and materials work without a demonstrator. The technology frontier is therefore plausible enough to investigate and immature enough to demand a national mission-science program. See [NASA's emergency advanced-air-mobility work](https://www.nasa.gov/aeronautics/advanced-air-mobility-for-emergencies/) and [DARPA's Liberty Lifter program record](https://www.darpa.mil/research/programs/liberty-lifter).

The attributable planning frame is $471.125 billion in new capital and $70.706 billion in mature annual operations. When nested with the Pass 25 Cascadia baseline, the regional attribution becomes $844.565 billion and $104.906 billion per year. These are scale hypotheses in constant 2026 dollars, not cost estimates. Pass 27 supersedes the provisional Pass 26 assurance increment; it must not be stacked on top of it.

The accompanying [72-hour Service Entry Force workbook](../../models/72-hour-service-entry-force-model.xlsx) exposes the module mass, service requirements, cell design, delivery timeline, all two-cell-loss cases, reliability allocation, workforce, capital, operating cost, industrial architecture and falsification gates.

## Why 72 hours is a distinct force-design problem

The first three days are not a compressed version of the later campaign. They have a different topology.

- Damage and need are only partially observed.
- Ports, airfields, bridges, water systems and grids may be physically repairable but not yet inspected or lawfully released.
- Local workforces are themselves disaster survivors.
- Commercial distribution systems may retain inventory while losing dispatch, fuel, communications or labor.
- Responders increase food, water, shelter, sanitation, medical and power demand before they produce net public effect.
- Every routing decision is exposed to aftershocks, fire, flood, debris, congestion and incomplete maps.
- A late shipment of one missing service can invalidate a large mass of otherwise useful cargo.

FEMA's Community Lifelines doctrine correctly frames response around stabilization of interdependent services rather than restoration of individual assets. It identifies safety and security; food, hydration and shelter; health and medical; energy; communications; transportation; hazardous materials; and water systems as the fundamental services that enable society to function. This study adopts that outcome logic, then pushes it into force design: a formation receives credit only for a service effect delivered by a deadline, not for equipment dispatched or tonnes moved. See [FEMA's Community Lifelines](https://www.fema.gov/emergency-managers/practitioners/lifelines).

Pass 25's first wave supplied the concrete service package. It comprised sixteen modules and 88,130 tonnes: civil command, degraded communications, reconnaissance, medical stabilization, search and rescue, air/port/littoral/route opening, responder basing, water, critical power, sanitation, food, shelter and fuel. It was the smallest complete operating layer in that campaign model.

Pass 27 changes its assurance rule. Rather than assigning individual modules to different paths, it replicates a fractional copy of the *whole service package* across independently supported cells. This is expensive, but it removes the fatal sequencing dependency in which access arrives without utilities, medicine arrives without power, food arrives without sanitation, or machinery arrives without crews and authority.

## The service kernel

### Definition

A **service kernel** is a configuration-controlled, fractionally complete public-service package. Every tranche contains the same proportional mix of effects and enabling layers. A ten-percent tranche should therefore be able to produce roughly ten percent of each declared effect, within a bounded tolerance, rather than one hundred percent of one service and none of another.

The kernel is not a universal shipping container. It is a scheduling, interface and readiness standard spanning containers, vehicles, personnel, data, energy and authorities. Some elements cannot be divided physically—a surgical team, airfield survey unit or command node, for example—so the force uses multiple discrete instances whose aggregate approximates the declared fraction.

The Pass 27 kernel uses 30 percent of every Pass 25 R1 module in each cell:

| Effect family | Reference capacity | Capacity per cell | Four-cell capacity | Hour-72 requirement |
| --- | ---: | ---: | ---: | ---: |
| Command | 9 service islands | 2.7 | 10.8 | 9 |
| Access | 30,000 t/day | 9,000 | 36,000 | 25,000 |
| Responder basing | 30,000 people | 9,000 | 36,000 | 25,000 |
| Water | 20,000 m³/day | 6,000 | 24,000 | 18,000 |
| Food | 2.6M people/day | 780,000 | 3.12M | 2.4M |
| Shelter | 500,000 people | 150,000 | 600,000 | 450,000 |
| Sanitation | 500,000 users | 150,000 | 600,000 | 450,000 |
| Critical power | 650 MW | 195 | 780 | 500 |
| Communications | 2.8M users | 840,000 | 3.36M | 2.4M |
| Health | 600 staffed beds | 180 | 720 | 500 |
| Hazard control | 120 route-equivalent km/day | 36 | 144 | 100 |

Four cells exceed every threshold. The margin varies because the reference wave itself carried different headroom by service. This is useful: the architecture does not pretend that a single scalar “percent complete” captures all public outcomes.

### The independence payload

Each cell contains 26,439 tonnes of direct effect modules and a 12-percent, 3,173-tonne independence allowance, for 29,612 tonnes total. That allowance represents cell-specific command, workforce support, repair parts, data, energy, technical authority and civil interface. It is not yet an engineered bill of materials. Its purpose is to make the hidden support burden explicit and falsifiable.

An independence allowance should ultimately be replaced by component-level designs. If the real support package is heavier, the cell grows or the service share falls. If automation or multi-use systems reduce it, the saved mass should remain visible rather than silently absorbed as payload growth.

### Why uniform mixing matters

The model permits delivered mass to stand in for delivered service only because it assumes uniform kernel mixing. That is a demanding requirement. Cargo planning must continuously solve for balanced effects while respecting indivisible teams, hazardous-material separation, temperature, security, maintenance, sequence and destination constraints.

This creates a new industrial product: the **autonomous service-kernel load system**. It combines a common cargo data model, machine-readable effect content, robotic cross-docking, dynamic reallocation, manual override and proof that partial delivery remains clinically, electrically, hydraulically and operationally coherent. The most important first demonstrator may therefore be a loading and scheduling system rather than a dramatic vehicle.

## Six cells, three entry families

### Upland North and Upland South

The two upland cells originate outside the correlated hazard footprint in separate infrastructure and labor catchments. Each begins receiving movement at hour 6. A 1,500-tonne-per-hour gross handling system, multiplied by 90-percent availability and a 90-percent handling factor, yields 1,215 net tonnes per hour. A cell completes at hour 30.4.

“Upland” is an origin and support concept, not a commitment to intact highways. Each cell owns a portfolio of road, rail, inland-water and vertical-transfer options; autonomous inspection; route opening; mobile bridges and surfaces; cross-docks; energy; and alternate reception points. The modeled throughput is at the cell boundary. Detailed path feasibility remains an open evidence gate.

### Air North and Air South

Each air cell begins at hour 18 after reconnaissance, repair and technical release. Its attributable fleet is 105 SAC-120 aircraft, including reserve. The model assumes:

- 120 tonnes average mission payload;
- a twelve-hour round-trip mission cycle;
- 75-percent campaign availability; and
- an 85-percent payload/handling factor.

Those assumptions yield 669.375 net tonnes per hour per cell and cell completion at hour 62.2. The fleet requirement is 210 aircraft across two cells.

This is deliberately beyond the current benchmark. The Air Force lists the C-17's *maximum* payload as 77,519 kilograms and notes its ability to use a 3,500-foot by 90-foot runway. SAC-120 requires approximately 55 percent more payload as an average planning load, while preserving austere access and radically shortening turn time. It should therefore be treated as an X-plane and industrial-base program, not a derivative procurement. See the [U.S. Air Force C-17 fact sheet](https://www.af.mil/About-Us/Fact-Sheets/Display/Article/1529726/c-17-globemaster-iii/).

The aircraft is only one layer. The air cell also needs runway sensing, repair, release authority, fuel or alternative energy, autonomous loading, airspace management, weather decision support, crews, maintenance, spares and onward distribution. Current rapid-airfield-repair work shows how much equipment and sequencing even a bounded repair mission requires; the Air Force's expeditionary repair demonstration targeted eighteen craters in 24–36 hours and constrained one repair kit to four C-130 loads. Pass 27 scales the operating problem up and adds civil safety release, persistent high tempo and public-service cargo. See the [Air Force expeditionary airfield-damage-repair account](https://www.af.mil/News/Article-Display/Article/2517186/just-enough-just-in-time-afcec-targets-rapid-airfield-repair-solution/).

### Offshore North and Offshore South

Each offshore cell is preloaded and already beyond the correlated hazard footprint. Transfer begins at hour 30. A no-pier chain rated at 1,100 gross tonnes per hour, with 85-percent availability and a 90-percent handling factor, produces 841.5 net tonnes per hour and completes a cell at hour 65.2.

The modeled force assigns four 12,000-tonne RSL-12 sea lifters to each offshore cell, including reserve, and six NPO-1100 no-pier systems to each cell. These are not hospital ships or surplus sealift vessels. The RSL-12 is organized around high-readiness service kernels, distributed maintenance, independent data and power, and rapid transfer into multiple shallow or damaged reception points. The NPO-1100 is a sustained production system spanning dynamic hydrography, stabilized transfer, debris avoidance, autonomous surf transit, temporary terminals and local onward movement.

The Navy's logistics-over-the-shore portfolio demonstrates that causeways, ferries, floating cranes, amphibious connectors and liquid transfer can bypass unavailable ports. It is an important analog, but its equipment, readiness system and mission priorities are not equivalent to a purpose-built civil service-entry chain. See [NAVFAC's Logistics Over-the-Shore program](https://www.navfac.navy.mil/PEO-Infrastructure-and-Expeditionary/PMO-314-LOTS/).

## Loss cases and time closure

There are fifteen distinct ways to remove two cells from a six-cell force. The workbook evaluates all of them at six-hour intervals.

| Lost cell family | Representative survivors | Grid closure |
| --- | --- | ---: |
| Both upland | two air + two offshore | hour 60 |
| One upland + one air | one upland + one air + two offshore | hour 60 |
| One upland + one offshore | one upland + two air + one offshore | hour 60 |
| Both air | two upland + two offshore | hour 54 |
| One air + one offshore | two upland + one air + one offshore | hour 54 |
| Both offshore | two upland + two air | hour 48 |

The worst case is loss of early-arriving upland capacity. It still closes by hour 60 because air and offshore service contributions rise together after hour 30. The twelve-hour margin to the declared deadline is not spare capacity available for optimism; it is the current allowance for finer sequencing, inspection queues, uneven service conversion and model error.

The result proves only a deterministic proposition: if the six cells are as independent and productive as declared, losing any two does not break the 72-hour package. It does not prove that their loss probabilities are independent, that weather and damage permit the throughput, or that public effects scale linearly with delivered modules.

## Reliability as a design budget

For six independent cells with identical loss probability \(p\), and closure with at least four survivors, the architecture reliability is:

```text
P(cell architecture closes)
  = (1-p)^6
  + 6p(1-p)^5
  + 15p²(1-p)^4
```

At \(p = 0.15\), the cell architecture closes with probability 95.266 percent. Multiplying by \(1-q\) for a campaign-wide common-mode loss allocation of \(q = 0.002\) yields 95.076 percent.

That narrow clearance is useful because it prevents the target from becoming ceremonial. The Department has almost no common-risk margin. It must treat shared software, suppliers, fuel, communications, workforce catchments, depots, technical authorities and origin infrastructure as quantified configuration attributes. Two cells cannot receive full independence credit merely because they have different names or vehicles.

This suggests a formal **Campaign Assurance Authority** with powers analogous to system safety, test and configuration control. It would own the covariance budget, approve independence credit, run seeded-loss exercises and require disclosure of common components and labor dependencies. It must be institutionally separate from the operating services and acquisition executives whose programs it judges.

## The complete cell

A cell is an operating system with nine inseparable layers:

1. **Service effect:** the fractional water, power, health, shelter, food, sanitation, communications, access and hazard-control capacity.
2. **Protected origin:** stocks, loading, energy, labor, alternate sites and dispatch outside the principal hazard correlation domain.
3. **Strategic movement:** air, maritime or upland portfolio, including crews and maintenance.
4. **Entry and onward distribution:** inspection, repair, technical release, handling and movement to service nodes.
5. **Zero-host-utility base:** power, water, sanitation, food, shelter, clinical support and waste handling for the force itself.
6. **Sovereign information plane:** sensing, identity, dispatch, spectrum, audit, public communication and offline operation.
7. **Repair and regeneration:** diagnostic authority, parts, field repair, depot reachback and replacement crews.
8. **Technical authority:** lawful decisions about airworthiness, structures, utilities, water quality, medical practice and environmental consequence.
9. **Civil interface:** legitimate public priorities, protected-population floors, consent, property access, allocation appeals and transfer to local control.

The governing readiness equation is the minimum across those layers. A cell at 90 percent in eight layers and zero in one produces zero credited independent effect.

## Technology programs the mission requires

### 1. SAC-120 strategic-to-austere airlift

The requirement is a 120-tonne average mission payload, twelve-hour cycle, austere operation, rapid roll-through unloading and 75-percent campaign availability. Candidate pathways could include a very large conventional transport, distributed propulsion, blended-wing cargo architecture, ground-effect transition, or multiple aircraft classes operating behind a common payload interface. The Department should fund rival concepts until representative missions discriminate among them.

### 2. RSL-12 ready sea lifter and NPO-1100 no-pier chain

The maritime problem is not ship speed alone. It is high readiness, preloaded mixed effects, safe rough-water persistence, transfer without a port, dynamic bathymetry, debris tolerance, shallow distribution and rapid reconfiguration among service nodes. DARPA's Liberty Lifter work is evidence that the boundary between airlift and sealift merits continued research, not evidence that a specific vehicle is ready.

### 3. ASK autonomous service-kernel logistics

The kernel system must know what public effects every pallet, crew, vehicle and data package can produce. It must recompose loads when an aircraft, landing point or service node disappears, and it must preserve safety, accessibility and protected-population floors. This is a national logistics operating standard with human override, not a fleet-management app.

### 4. ARE-18 reconnaissance, repair and release

The target is not simply a patched runway or inspected bridge. It is a machine-readable safety case delivered to a named authority early enough to permit lawful use. The program combines remote sensing, autonomous survey, nondestructive evaluation, rapid materials, digital twins, residual-risk estimation and degraded-mode certification.

### 5. MICRO-195 utility island

Each cell carries effects equivalent to 195 MW of critical power and 6,000 cubic metres per day of water, plus sanitation and thermal relief. Current portable systems establish useful building blocks but not the necessary scale. DOE has demonstrated a container-sized 250-kW portable microgrid capable of black start, while EPA's Water on Wheels cart produces up to ten gallons per minute. Pass 27 is orders of magnitude larger and therefore requires modular grid-forming generation, high-throughput treatment, deployable conductors and pipe, storage, wastewater control and rapid utility interconnection. See the [DOE portable microgrid demonstration](https://www.energy.gov/cmei/water/articles/portable-microgrid-technology-can-bolster-small-town-hydropower-during-power) and [EPA Water on Wheels research](https://www.epa.gov/emergency-response-research/water-wheels-mobile-water-treatment-system-wow-cart).

### 6. Sovereign degraded-mode mission command

Six nominal cells can collapse into one common failure domain if they depend on the same cloud, map, identity provider, spectrum service or software update. The data architecture must run locally, synchronize opportunistically, reveal confidence and provenance, accept human dispatch, and survive removal of two providers plus the central cloud. NASA's current emergency-aviation research on portable airspace management and beyond-visual-line-of-sight operation is an important adjacent foundation. See [NASA's Advanced Air Mobility Pathfinders](https://www.nasa.gov/directorates/armd/aosp/amp/about-aamp/).

## Workforce and force generation

The model places 7,500 people in each deployed cell:

| Function | People per cell | Six-cell deployed force |
| --- | ---: | ---: |
| Command and civil interface | 350 | 2,100 |
| Health and human services | 1,500 | 9,000 |
| Infrastructure and utilities | 1,700 | 10,200 |
| Mobility and autonomous handling | 1,600 | 9,600 |
| Responder base and sustainment | 1,300 | 7,800 |
| Data, communications and sensing | 600 | 3,600 |
| Safety, test and technical authority | 450 | 2,700 |
| **Total** | **7,500** | **45,000** |

A 4.2 rotational factor produces 189,000 cell-force billets. Aviation, maritime, origin, depot, training, science and institutional elements add a provisional 60,000, for 249,000 attributable people. This is not a volunteer surge roster. It is a standing profession with recurring full-mission exercises, degraded-mode certifications, medical and occupational readiness, family support, relief crews and public accountability.

The workforce model reveals an important autonomy principle. Automation should not be justified by a generic desire to remove people. It should reduce the occupations most exposed to dangerous, repetitive, low-information work; preserve scarce licensed judgment; and lower the responder-base burden that otherwise competes with public demand. Every autonomy program should report which crew demand it changes and which new maintainers, supervisors and technical authorities it creates.

## Command and civil legitimacy

Speed without lawful priority is not stabilization. The force therefore carries authority deadlines alongside cargo deadlines:

- by hour 6, the civil incident authority defines service outcomes and protected populations;
- by hour 6, Joint Deployment Command activates and routes independent cells;
- by hour 18, technical authorities release entry infrastructure within declared risk envelopes;
- by hour 24, a civil service board allocates scarce effects using published rules;
- by hour 36, cross-cell substitution can be accepted under predelegated authority; and
- by hour 72, the civil authority—not the logistics commander—decides whether lifelines are stabilized.

If communications fail, bounded delegations and public service floors remain in force. Every consequential decision creates an auditable artifact. The Department's sovereign capability is not freedom from civil constraint; it is the ability to execute civil decisions under conditions that disable ordinary administration.

## Industrial architecture

The Service Entry Force requires “Lockheed Martin–level” industrial seriousness without reproducing monopoly dependence or proprietary lock-in. The mature market should have five features.

**Government-owned mission architecture.** The Department owns the service-effect ontology, payload envelopes, data standards, safety-evidence schema, digital reference missions and test scenarios. Firms compete inside an interface architecture they cannot privately redefine.

**Competing implementations.** At least two design and production teams remain viable for every critical mobility class and common-mode-sensitive subsystem. Competition is maintained through planned technology insertion, block upgrades, test articles and export variants—not a single winner-take-all production decision.

**Public depots and independent test.** Government depots hold the ability to inspect, repair, modify and reproduce essential interfaces. Independent test authorities own ranges, instrumentation, seeded-loss campaigns and public evidence records.

**Readiness as a purchased outcome.** Long-horizon contracts pay for configured availability, trained crews, exercised suppliers and surge production—not merely units delivered. Readiness measures include origin separation, common-part exposure, software diversity and time since representative full-mission proof.

**Exportable cell standards.** Allies and partner nations can buy, build or contribute compatible service kernels without importing the entire U.S. institution. Common interfaces allow allied cells to federate while preserving national control, local labor and locally appropriate clinical, utility and legal modules.

## Fiscal frame

The $376.9-billion capital subtotal contains:

| Program element | Planning amount |
| --- | ---: |
| Six mission-equipment sets | $44.4B |
| Six independent origin complexes | $30.0B |
| 210 SAC-120 aircraft | $115.5B |
| Eight RSL-12 sea lifters | $24.0B |
| Twelve NPO-1100 systems | $9.0B |
| Autonomous cargo and inspection craft | $15.0B |
| Autonomous handling systems | $12.0B |
| Six micro-utility/base packages | $27.0B |
| Sovereign mission systems | $15.0B |
| Depots, schools and test ranges | $25.0B |
| Technology and full-mission test | $60.0B |

A 25-percent pre-reference-design reserve adds $94.225 billion, producing $471.125 billion incremental. The largest line is purpose-built heavy airlift, followed by the technology and test program. That is appropriate at this stage: the architecture should spend heavily to discover which platform pathways are real before it commits to long production runs.

Mature incremental operations are provisionally $70.706 billion per year, of which $44.82 billion is the loaded 249,000-person workforce and $12.6 billion is the SAC-120 fleet. These amounts are not optimized. They expose the recurrent cost of maintaining a standing sovereign capability rather than treating catastrophe response as free episodic labor.

## Evidence gates and falsification

The design should fail early if its premises are wrong. Ten gates remain open:

1. Demonstrate that each ten-percent kernel tranche produces ten percent ±2 percent of every declared effect.
2. Sustain 1,215 net tonnes per hour through an upland cell under damaged-network, no-grid and degraded-labor conditions.
3. Sustain 669 net tonnes per hour through an air cell in a representative sortie campaign.
4. Sustain 842 net tonnes per hour through an offshore cell with surf, debris and damaged reception.
5. Show that no shared dependency can remove two credited cells.
6. Bound cell loss at 15 percent and common-mode loss at 0.2 percent with empirical joint distributions.
7. Operate all six cells through three workforce rotations without host services.
8. Show household-level service floors for protected and hard-to-reach populations.
9. Meet every civil and technical authority deadline in degraded communications.
10. Produce independent P50/P80 cost and schedule ranges from reference designs.

A green formula check is not evidence that any gate has passed. It means only that the declared architecture is internally consistent.

## What this changes in the larger Department

Pass 27 sharpens the Department of Resilience in four ways.

First, the basic force element becomes the **complete cell**, not a functional battalion or platform squadron. Services retain professional ownership of medicine, utilities, mobility and hazard control, but readiness is certified jointly at cell level.

Second, acquisition begins with **effect interfaces and representative missions**. A platform program cannot claim success until it closes a public-service chain under seeded loss.

Third, national posture is reported as an **assured cell portfolio**. Counts are discounted for shared origins, software, components, crews, authorities and suppliers.

Fourth, industrial policy becomes part of operational design. Supplier diversity, public depot rights, data portability, workforce catchments and surge tooling are independence parameters, not economic side notes.

The result is more ambitious than preserving existing institutions. It is a new national operating system whose strategic output is the rapid creation of temporary public-service capacity in places where ordinary systems have failed.

## Research limits and next decision

This pass is a functional configuration, not a vehicle configuration. It does not close aircraft aerodynamics, runway bearing strength, ship stability, sea-state operability, utility thermodynamics, pipe and conductor deployment, clinical staffing ratios, detailed hazardous-material compatibility, local last-mile distribution or lifecycle environmental effects. Its probability model is deliberately simple. Its cost factors are planning assumptions.

The next pass should attack **service-kernel composition and physical interfaces**. It should decompose one 29,612-tonne cell into indivisible teams, equipment, consumables, power, water, data, maintenance and cargo tranches; solve the loading and sequencing problem across air, sea and upland variants; and identify which “common” modules must actually differ to preserve independence. Only after that work should exterior platform geometry begin.

Renderings therefore remain blocked.
