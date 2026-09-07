# Canonical Cargo and Transport Closure

## From formation mass to deployable civil power

### Research state

Pass 61 is the first Department-wide attempt to express the [canonical force](../generation/canonical-force-allocation-and-fiscal-reconciliation.md) as cargo that a carrier, transfer node and receiver could eventually recognize. It replaces the aggregate-tonnage screen retained in the [shared-capacity allocation study](../generation/shared-capacity-allocation-and-claim-denial.md) with 448 formation cargo-position records, 4,480 campaign claims, four mode ledgers and 480 formation-closure records.

The accompanying [`canonical-cargo-and-transport-model.xlsx`](../../../models/force/projection/canonical-cargo-and-transport-model.xlsx) is the arithmetic authority. It preserves the forty-eight canonical formation families and ten simultaneous campaigns, allocates each formation's post-preposition mass across ten external cargo-interface classes, converts physical mass and volume into chargeable demand, applies protected capacity by mode and deadline, and credits a formation only at its weakest required cargo-class line.

This is a **position-class compiler**, not an item-level bill of material, operational load plan, carrier schedule or validated movement estimate. Cargo shares, mass fills, envelopes, compatibility weights, routing priors, deadline fractions and inherited capacity are research hypotheses. No serial item, origin, route, carrier, crew, node slot or receiver release has yet been assigned. A passing transport line would still not establish an operating public service. Those limits are not footnotes; they determine the next research program.

No platform rendering follows from this pass. The result identifies the evidence and requirement envelopes that must precede form.

## Executive judgment

The Department of Resilience cannot design strategic mobility around tonnes alone. A tonne does not reveal whether the burden is a restrained pallet, refrigerated clinical module, hazardous battery enclosure, process tank, flatrack plant, rolling machine, long pipe rack, low-density shelter volume or indivisible outsize structure. It does not identify a safe carrier, a handling system, a node, a release path or a receiving interface. It therefore cannot support a serious clean-sheet aircraft, ship, land-carrier or inland-waterway program.

Pass 61 gives that proposition national scale. After the inherited 25-percent prepositioning credit, the ten campaigns retain **6,677,140 tonnes** of physical source mass. Position count, volume occupancy and mode-specific density floors raise the first chargeable burden to **7,047,691 tonnes**, a **370,551-tonne or 5.55-percent dimensional uplift**. The inherited four-mode enterprise offers 2,462,931 effective tonnes at 72 hours. Protecting 20 percent for a follow-on catastrophe leaves **1,970,345 usable tonnes**.

The deadline allocator can apply only **1,764,353 chargeable tonnes**. Another **205,992 tonnes** of nominally usable capacity is stranded because it exists in the wrong mode or becomes available after the cargo deadline. Converted back to actual cargo, the enterprise delivers **1,702,425 physical tonnes**, or **25.5 percent** of the source mass.

That average is still misleading. A formation produces no complete service when its command loads arrive but its rolling plant does not, or when its treatment equipment arrives but its powered cold chain, tankage or linear works remain behind. Crediting each formation at its weakest required cargo-class coverage yields only **314.5 complete formation equivalents against 2,420 demanded**, or **13.0 percent**. Just **11 of 480** formation–campaign records cross the 95-percent transport threshold. None receives public-effect admission because every receiver remains unquantified.

The result overturns three comfortable intuitions.

First, aggregate 72-hour capacity coverage is not deployment closure. Pass 60's 36.6-percent mass ratio falls to 25.5 percent when capacity is protected, dimensional burden is recognized and deadlines are enforced; it falls again to 13.0 percent when required complements are kept together.

Second, buying the same proportions of every current transport mode would not solve the problem. Early ocean and land capacity are severe constraints while some late air and inland-water capacity remains unused. The force faces a **time–mode–interface mismatch**, not one scalar lift deficit.

Third, the appropriate acquisition object is not an isolated high-payload vehicle. It is a carrier–node–receiver system able to accept a governed portfolio of whole cargo positions, survive damaged access, execute high-rate transfer, preserve cold and hazardous separation, expose its state to the allocation authority, release cargo into operating service and regenerate for a second event.

The mature response should be ambitious. Strategic mobility for civil stabilization should become a core Department enterprise with purpose-built air, ocean, land/rail and inland-water families; rapidly created terminals; automated configuration and handling; common fluid, power, data and mechanical interfaces; and a digital capacity graph that follows each position from readiness through service and regeneration. But the design sequence matters. The Department should compete technologies against complete mission closure, not draw spectacular vehicles and then search for their use.

## 1. Why mass is not the unit of deployable power

### 1.1 The operational object

The Department's governing unit remains a defined population receiving a defined safe service by a stated time and for a stated duration under stated damage. Strategic movement is one serial segment of that obligation. The chain is:

```text
public effect contract
        ↓
formation and sustainment package
        ↓
serial cargo positions at named origins
        ↓
carrier legs and transfer-node slots
        ↓
receiver release and commissioning
        ↓
operating service at the point of use
        ↓
retrograde, repair and regenerated readiness
```

Every arrow is a possible denial. Transport can be physically present and operationally worthless when a position is incompatible, a hazardous segregation rule cannot be met, a route is lost, a node lacks handling power, a receiver cannot connect the module, or the supporting workforce has not arrived. Conversely, some mass can be delayed with little effect when it is genuinely substitutable or belongs to a later sustainment echelon. An adequate model must preserve those differences.

The object presented to the movement system is therefore a **cargo position**:

\[
p=(i,f,k,m,v,g,h,r,d,o,z,c),
\]

where `i` is a persistent identity, `f` the formation and complete-package identity, `k` the external interface class, `m` mass, `v` occupied envelope, `g` center-of-gravity and restraint state, `h` hazard and temperature state, `r` required receiver, `d` service deadline, `o` origin and readiness state, `z` allowable modes and routes, and `c` complement relationships. Pass 61 begins `f`, `k`, `m`, `v`, `r` and `d`. The other coordinates remain gates.

### 1.2 Chargeable demand

Capacity must observe whichever burden binds: actual mass or the volume consumed at a mode's minimum planning density. For cargo position `p` routed through mode `q`, the model uses:

\[
D^{charge}_{p,q}=\max\left(m_{p,q},\;v_{p,q}\rho^{min}_{q}\right).
\]

This is not a tariff. It is a first engineering screen against a model that allows low-density cargo to vanish inside a tonne total. The declared density floors are 0.25 tonnes per cubic metre for air, 0.15 for ocean, 0.20 for land and rail, and 0.18 for inland water. Setting all four floors to zero makes chargeable demand equal physical demand at 6,677,140 tonnes; restoring them returns the 7,047,691-tonne baseline exactly. The result is therefore a real model consequence of the declared dimensional burden, not a hard-coded surcharge.

The uplift is modest in percentage terms and consequential in acquisition terms. A five-percent error applied to a national force can determine hundreds of thousands of tonnes of fleet, node and storage demand. More importantly, the average conceals class extremes. Low-density shelter and food loads, powered cold modules and outsize structures impose different bay, energy, handling and queue requirements even at the same chargeable tonnes.

### 1.3 Complements rather than averages

For formation `f` with required cargo classes `k`, delivered formation credit is bounded by the weakest line:

\[
F^{complete}_{f}=F^{demand}_{f}\min_k\left(\frac{x_{f,k}}{D_{f,k}}\right).
\]

This rule is deliberately stricter than delivered mass. It prevents abundant command pallets or general containers from compensating mathematically for missing rolling machines, tanks, long loads or outsize plant. It also prevents a transport system from being declared successful because it moved what was easiest to carry.

The rule does not assert that every gram assigned to a profile is operationally indispensable. That can be known only after item-level bills of material and mission trials. It does assert the correct burden of proof: a designer seeking substitution or partial service credit must identify the item, effect, acceptable degradation and evidence. The default cannot be that unrelated mass substitutes automatically.

## 2. The external cargo-interface grammar

### 2.1 Ten position classes

Pass 61 introduces ten classes that are broad enough to span the forty-eight formations but specific enough to expose distinct carrier and receiver obligations.

| ID | Position class | Binding feature | Required receiving interface |
|---|---|---|---|
| `APL-45` | Palletized command, sensor and medical load | restrained, high-priority, potentially medical | air-cargo handling system |
| `ISO-18` | Dry ISO-compatible mission load | sealed intermodal position | intermodal transfer node |
| `COL-12` | Cold-chain and controlled clinical load | powered temperature control and biological segregation | powered cold node |
| `BAT-22` | Energy storage and power electronics | hazardous energy, isolation and fire behavior | hazardous-energy pad |
| `TNK-20` | Liquid, treatment and process tank module | fluid compatibility, residuals and manifold connection | fluid-transfer manifold |
| `FLR-24` | Flatrack plant and construction module | lift, tie-down and heavy apron | heavy-handling apron |
| `ROL-30` | Rolling vehicle and self-deploying machine | ramp, axle/ground load and road release | roll-on ramp and verified route |
| `LIN-18` | Long pipe, conductor and linear-works load | awkward length, joint protection and transload | long-load lane |
| `BLK-08` | Low-density shelter, food and support load | volume, weather protection and distribution | covered distribution node |
| `OOG-80` | Outsize plant and mission structure | engineered lift, restraint and route envelope | heavy-lift berth or lane |

These are **external interfaces**, not ten permanent container designs. Their purpose is to let generating services, mobility commands and industry speak a common acquisition language while internal modules evolve. An item may require a more specific subtype. A position may not change class merely to fit the available carrier.

### 2.2 Nine formation profiles

The model assigns each canonical family to one of nine preliminary cargo profiles: command, engineer, aviation, maritime, utility, clinical, population support, mobility and household access. Each profile distributes formation mass across the position classes and reconciles to 100 percent. Zero-share classes are omitted, producing 448 rather than 480 formation-class records.

This method is intentionally conservative about what it proves. It creates a consistent national compiler without pretending that a percentage is a bill of material. A command profile is relatively pallet and container intensive; an engineering profile carries more flatrack, rolling, linear and outsize burden; a clinical profile elevates pallet, dry-container, cold and low-density support; a household-access profile carries unusually high rolling-machine share. Those distinctions are plausible enough to test transport architecture and too coarse to procure against.

The next maturity step is not to refine the percentages by expert taste. It is to select representative formations, assign persistent item and package identities, weigh and measure the actual configuration, then reconcile every item to service, crew, maintenance, safety, sustainment and receiver requirements.

### 2.3 Whole positions and fractional planning flow

The cargo register rounds each formation's required positions upward after applying declared mass fill. This exposes indivisibility and occupied cube. Campaign allocation, however, still applies proportional rates to the class demand. The model can therefore report fractional delivered formation equivalents; it cannot claim that a particular serial position was loaded.

This boundary is important. Proportional flow is useful for national requirement discovery because it shows where capacity coefficients bind. Operational allocation must become integer and serial. It must answer which exact load moved, on which carrier, through which nodes, with which complements, while maintaining which reserve. Gate `G01` therefore requires one complete tagged formation manifest before readiness or allocation can advance.

## 3. National result

### 3.1 Capacity after reserve

The inherited 72-hour capacity screen provides:

| Mode | Gross effective capacity | Capacity after 20% reserve |
|---|---:|---:|
| Air | 160,881 t | 128,705 t |
| Ocean | 596,400 t | 477,120 t |
| Land and rail | 1,183,200 t | 946,560 t |
| Inland water | 522,450 t | 417,960 t |
| **Total** | **2,462,931 t** | **1,970,345 t** |

The reserve is a protected claimant for a second catastrophe, not slack available to the first optimizer. Removing it raises delivered physical mass from 1,702,425 to 2,112,181 tonnes and complete-formation coverage from 13.0 to 16.3 percent. The increase matters, but it does not close the force. Consuming every protected tonne would still leave more than 4.5 million chargeable tonnes outside the 72-hour enterprise and would expose the nation to a follow-on event.

The proper policy question is therefore not whether reserve “wastes” capacity. It is which risk distribution, geographic independence, regeneration time and civil consequence justify the reserve portfolio. That requires a two-event allocation trial, not a single percentage chosen for budget convenience.

### 3.2 Deadline and mode mismatch

Capacity is cumulative at 24, 48 and 72 hours. Demand is assigned to the deadline of its cargo class. The resulting bucket coverage is:

| Mode and deadline | Chargeable demand | Capacity allocated | Bucket coverage |
|---|---:|---:|---:|
| Air, 24 h | 221,999 t | 45,047 t | 20.3% |
| Air, 48 h | 160,688 t | 45,047 t | 28.0% |
| Air, 72 h | 0 t | 0 t | 100.0% |
| Ocean, 24 h | 158,946 t | 23,856 t | 15.0% |
| Ocean, 48 h | 1,633,296 t | 143,136 t | 8.8% |
| Ocean, 72 h | 396,194 t | 310,128 t | 78.3% |
| Land/rail, 24 h | 494,932 t | 189,312 t | 38.3% |
| Land/rail, 48 h | 3,102,258 t | 378,624 t | 12.2% |
| Land/rail, 72 h | 529,536 t | 378,624 t | 71.5% |
| Inland water, 24 h | 18,171 t | 18,171 t | 100.0% |
| Inland water, 48 h | 269,173 t | 169,911 t | 63.1% |
| Inland water, 72 h | 62,498 t | 62,498 t | 100.0% |

Ocean at 48 hours is the lowest-covered bucket; land and rail at 48 hours carries the largest unmet burden. Late air capacity cannot help because no modeled class waits until 72 hours for air. Late inland-water capacity cannot repair a landlocked campaign or move cargo that lacks a feasible water route. Ocean capacity available at 72 hours cannot satisfy clinical, command or other 24–48-hour obligations merely because the national total balances later.

This is the core clean-sheet insight: **activation slope and access geometry can be more valuable than terminal fleet payload**. A vehicle program that maximizes payload at day seven while leaving the 24–48-hour transfer system unchanged may improve the easiest part of the curve and fail the public deadline.

### 3.3 Campaign closure

Every campaign fails the formation-closure standard.

| Campaign | Physical mass coverage | Complete-formation coverage | Passing families / 48 |
|---|---:|---:|---:|
| Grid failure | 25.6% | 13.3% | 0 |
| Gulf–Atlantic hurricane | 28.4% | 15.5% | 0 |
| Cascadia earthquake | 24.8% | 12.3% | 0 |
| Western fire and heat | 24.5% | 12.2% | 5 |
| Urban heat | 23.8% | 12.2% | 5 |
| Inland flood | 32.4% | 18.6% | 1 |
| Tornado sequence | 24.0% | 12.2% | 0 |
| Drought and water | 29.3% | 15.8% | 0 |
| Allied megacity earthquake | 20.8% | 8.8% | 0 |
| Regional flood and displacement | 24.3% | 12.2% | 0 |

The allied megacity earthquake is the most severe formation-closure case because its routing prior places most demand on ocean entry, whose 48-hour coverage is only 8.8 percent. The inland-flood campaign has the highest average and complete coverage because some inland-water buckets clear, but forty-seven of forty-eight family claims still fail. The eleven passing records across all campaigns occur only in the two fire/heat cases and the inland-flood case. They remain transport-only records; no receiver admission exists.

The campaign results should not be interpreted as forecasts of future disasters. They are simultaneous demand envelopes inherited from the canonical allocation, crossed with declared routing and compatibility hypotheses. Their value is comparative and architectural: they expose which combinations a mobility system must survive and prevent a national average from erasing the worst geography.

## 4. What a mature strategic mobility enterprise must become

### 4.1 Strategic Mobility Command

The Department requires a permanent **Strategic Mobility Command**, not an emergency transportation desk. It should own readiness and operational control of purpose-built strategic carriers, coordinate contracted and allied capacity, maintain the movement graph, define activation standards, assign carriers and routes to admitted claims, and preserve protected reserve. It should not own every formation's cargo or decide public priority alone.

Generating services own complete configuration and attest that a package is ready. Entry and distribution commands own ports, airfields, railheads, inland terminals, expeditionary transfer nodes and onward movement. Receiving commands and civil authorities own site admission, utility connection, commissioning and lawful transfer into service. The Joint Capacity Authority arbitrates competing claims and propagates denial. Independent test and evaluation authorities reproduce readiness and mission results.

That separation prevents four failures: a mobility command changing the mission package to improve its utilization statistics; a generating service claiming lift without a carrier reservation; a carrier operator declaring success at discharge; and a political allocator consuming the protected reserve without recording the second-event consequence.

### 4.2 The carrier–node acquisition unit

A carrier should not be acquired on payload, speed or range alone. Its governing score is complete cargo positions released per unit time into a damaged receiver while preserving safety, service deadline, availability and regeneration. At minimum, every candidate should be evaluated on:

- accepted mix of the ten external position classes;
- activation curve and loaded departure rate at 24, 48 and 72 hours;
- whole-position capacity by mass, cube, geometry and hazardous segregation;
- origin loading and destination discharge without intact commercial infrastructure;
- compatibility with common mechanical, electrical, fluid and data interfaces;
- crew, maintenance, energy, spares and turnaround demand;
- route and weather envelope under the target campaign;
- node footprint, queue formation and handling-energy demand;
- degraded operation, manual fallback and safe recovery;
- receiver commissioning time and service release rate; and
- post-use inspection, decontamination, repair and return to reserve.

The acquisition unit should normally pair a carrier cohort with origin and destination nodes, handling systems, control software, training, depot support and a representative cargo package. Otherwise the state buys theoretical mobility and leaves transfer capacity to another budget.

### 4.3 Air family

The air requirement is concentrated at 24 and 48 hours. The force needs reliable activation, rapid configuration change, autonomous or low-labor loading, cold-chain power, hazardous-energy separation and austere discharge more than it needs a single record-setting payload.

A mature program may contain several purpose-built families: a strategic module carrier for repeated high-volume pallet and compatible-container movement; a short-field theater carrier for damaged or improvised runways; and vertical-access systems for teams, patients and bounded priority loads. Common cargo locks, powered-position interfaces, load-state sensing and handling robots may matter more across the portfolio than a common airframe.

The research must test whether oversized air carriage is preferable to designing critical civil modules around more frequent standardized positions. Outsize capability should exist where physical mission function demands it, not because formation design avoided modularity. Air platforms must also be competed against runway repair, forward prepositioning and land-network restoration; the correct answer may change by cargo class and campaign.

### 4.4 Ocean family

Ocean transport carries the largest international and coastal mass opportunity and the sharpest early activation deficit. A mature ocean family should separate high-volume strategic sealift, self-discharging austere access, rolling and flatrack movement, cold and hazardous zones, outsize heavy works, afloat prepositioning, port opening and sustainment. One universal disaster ship would concentrate availability and impose contradictory draft, berth, aviation, clinical and process requirements.

The 8.8-percent ocean 48-hour result pulls technology toward ships and prepositioning concepts that are useful early, not merely capacious after mobilization. Possibilities include permanently ready regional squadrons, high-availability self-discharging carriers, modular lighterage, distributed cargo already packed to formation identity, and purpose-built expeditionary ports. Any nuclear water–energy or hospital platform remains part of a service flotilla and receiver chain; it cannot substitute for the transport system that brings distribution, grid, clinical, residual and workforce complements.

### 4.5 Land and rail family

Land and rail carry 4.127 million chargeable tonnes in this screen, including 3.102 million due at 48 hours. The requirement is not simply more trucks. It is a continental movement and infrastructure-control system able to survive bridge, road, fuel, terminal, signaling and workforce losses while handling rolling, long, tank, battery, flatrack and low-density cargo.

Clean-sheet programs could include optionally crewed high-cycle road trains; common powered and instrumented trailers; disaster rail consists with rapid loading, independent power and field transload; bridge- and pavement-aware route assignment; deployable weigh, inspection and repair nodes; and autonomous convoy support that reduces human exposure without assuming continuous communications. The enterprise must preserve driver and maintainer cycles, public road access, local delivery and reverse logistics.

Rail should not be treated as interchangeable tonne capacity. It requires origin track access, train assembly, network slots, functioning control, destination sidings, transload and onward movement. Road capacity is similarly bounded by axle loads, bridge state, congestion, fuel, crew and discharge. The next model must distinguish those submodes and their nodes.

### 4.6 Inland-water family

Inland water is not a national balancing account. It is a geography-specific operational system with shallow draft, launch, lock, current, debris, bank, mooring and inter-basin constraints. Its apparent late surplus in the model indicates useful capacity where routes exist; it does not erase deficits elsewhere.

The mature family may include road- or rail-deployable craft, modular barges, shallow-draft carriers, powered tow systems, floating transfer nodes and rapid bank interfaces. The most valuable clean-sheet feature may be the ability to create a terminal where no terminal survived. Cargo should cross from water to road, utility or local distribution without requiring a deep-draft port. Inland vessels that carry pumps, linear works, rolling machines or modular utilities should be evaluated with those complete positions and with recovery from debris or current loss.

### 4.7 Nodes as first-class platforms

The model's receiver column is unquantified on every record. That makes node and receiver design at least as important as vehicle design. A mature Department should fund airfield-opening groups, austere ports, rail and road transload sites, inland-water terminals, cold nodes, hazardous-energy pads, fluid manifolds, heavy aprons, long-load lanes and covered distribution nodes as named acquisition programs.

Each node needs a position admission envelope, handling rate, storage dwell, energy balance, workforce cycle, damage tolerance, queue limit, safety case, data boundary and onward-release contract. It also needs a rapid-create variant for places where the permanent node is destroyed or politically unavailable. Carrier throughput should be denied when the node cannot accept the arrival; otherwise the model converts an airborne or afloat queue into fictional delivered service.

## 5. Technology programs pulled by the evidence

The Department should use this failure surface as the military uses operational problems: to sustain long-horizon technology competition. The following programs are not accessories to transport. They could change the decisive coefficients.

### 5.1 Canonical configuration compiler

Every formation needs a machine-readable, versioned compiler connecting public effect, personnel, serial items, cargo position, sustainment, carrier compatibility, receiver interface and regeneration work. It should automatically reject broken complements, duplicate items, expired certifications, impossible centers of gravity, missing hazardous declarations and receiver incompatibility. It must function disconnected and preserve human-readable release authority.

### 5.2 Smart common positions

Pallets, containers, flatracks, tanks, battery enclosures and long-load racks should expose persistent identity, mass, dimensions, restraint state, hazard, temperature, power demand, maintenance status and shock history. Common latching, lifting, data and power interfaces would allow multiple manufacturers and carriers to compete without proprietary lock-in. Sensors should support inspection, not replace it.

### 5.3 Autonomous packing and handling

Machine vision, robotic forklifts, automated restraint verification, self-positioning dollies and high-rate mixed-cargo sequencing could reduce the labor and queue penalties that dominate activation. The proving question is end-to-end throughput under damaged surfaces, poor visibility, mixed legacy cargo, communications loss and manual fallback—not a controlled warehouse demonstration.

### 5.4 Shape-changing low-density systems

The 5.55-percent dimensional uplift creates a direct research target: shelters, ducts, clinical interiors, food systems and distribution structures that fold, nest, compact or manufacture near the point of use without sacrificing safety, setup rate, repairability or service quality. A mass saving that creates excessive assembly labor may worsen closure; the experiment must include the receiver workforce and time.

### 5.5 Universal utility interfaces

Power, water, thermal, fluid, data and waste modules need governed interface families: voltage and frequency bands, protection and grounding, hose and pipe manifolds, water-quality sampling points, residual connections, cyber boundaries and mechanical envelopes. Adaptation remains necessary, but adapter burden must be visible as cargo, labor, failure probability and commissioning time.

### 5.6 Damage-aware multimodal scheduling

The allocation system should treat roads, bridges, ports, airfields, rails, locks, weather and receivers as a changing graph with evidence age and uncertainty. It should preserve public-priority rules and explain why a claim was admitted, rerouted or denied. Optimization cannot be allowed to infer unlawful substitution or hide scarce service behind an aggregate objective.

### 5.7 Mission-aware recomposition

If positions are delayed or lost, software and trained commanders should identify which bounded service can still be produced, which substitutes are authorized and which formations can be recomposed without creating two incomplete packages. This requires experimentally established degradation curves. It must never turn a missing safety-critical complement into nominal readiness.

### 5.8 Regeneration and reverse logistics

Every position and carrier creates a return path: contaminated equipment, clinical waste, damaged batteries, residuals, empty packaging, repairable modules and exhausted crews. The digital record should predict depot work, reserve unavailability and environmental custody before dispatch. A fleet that meets the first event by consuming the next event is not strategically ready.

## 6. Industrial and economic consequence

A coequal mobility enterprise would create more than vehicle production. It would sustain aircraft and ship design, rail and heavy-vehicle engineering, modular utilities, cargo systems, robotics, sensors, cold chain, hazardous-energy handling, terminal construction, software assurance, depots, technical education and regional proving infrastructure.

The industrial design should avoid both a single prime contractor and fragmented commercial purchasing. The Department needs stable multi-decade demand, several competing system integrators, specialist suppliers, public interface standards, government-purpose data rights, independent test capacity and surge paths that do not silently strip the same civil industries needed during catastrophe.

Common position and receiver interfaces create an export opportunity more durable than selling a prestige platform. Allies and cities could procure compatible modules, nodes, carriers and training at different scales while preserving local ownership. A position built by one country could move on another's carrier and commission at a third country's node when safety and authority permit. That is civil interoperability as strategic power.

The economic model must eventually connect four ledgers:

1. development and production capacity;
2. owned and contracted fleet and node inventory;
3. operating, workforce, maintenance and regeneration cost; and
4. measurable reduction in interrupted service, mortality, displacement, recovery time and cascading loss.

Pass 61 does not price a solution. Pricing carriers before serial cargo, node demand and availability targets are known would merely capitalize the current uncertainty. The next financial pass should cost competing **carrier–node portfolios** against the same admitted cargo and campaigns, with explicit reserve and industrial learning, rather than allocate a trillion-dollar headline among vehicle categories.

## 7. Research and acquisition program

### 7.1 Immediate evidence sequence

Thirteen gates remain open:

1. assign serial item and package identity to one representative formation;
2. reconcile a complete bill of material to its modeled mass;
3. measure dimensions, center of gravity and restraint for every position class;
4. establish hazardous and cold-chain classifications;
5. register origin and preposition sites;
6. identify carrier fleets, crews and readiness;
7. define node slots and handling configurations;
8. prove receiver release and operating interfaces at a named site;
9. exercise damage-aware route survival and mode substitution;
10. measure maintenance and regeneration work content;
11. calibrate the protected reserve in a two-event trial;
12. publish and contest public-priority and appeals rules; and
13. close representative missions under independent observation.

The first configuration should be selected for information value: mixed pallet, container, cold, battery, tank, flatrack, rolling and long-load demand; a real origin; more than one carrier mode; and a receiver that requires commissioning. It should not be chosen because it is unusually easy to pack.

### 7.2 Rival reference missions

Once the serial manifest exists, the Department can run rival carrier–node reference missions:

- 24-hour continental entry for command, clinical and priority utility positions;
- 48-hour coastal entry for rolling, flatrack, tank and outsize positions without a functioning port;
- 48-hour land/rail surge through a damaged bridge and terminal network;
- shallow-water movement and bank transfer for inland flood isolation;
- two simultaneous campaigns with a protected third reserve; and
- full retrograde, inspection, repair and readiness restoration.

Each trial should publish cargo admitted, complete formations released, public-service time, queue and handling losses, crew and energy burden, failed positions, substitutions, safety events, maintenance debt and cost. Rival systems should face the same configuration and seeded failures.

### 7.3 Acquisition gates

Concepts may advance from position-class requirement to preliminary platform envelope only after the representative manifest and node trial close. They may advance to rendering only after mass, cube, geometry, interfaces, crew, energy, maintenance, degraded operation and receiver flow are sufficiently bounded to make form informative. They may advance to prototype acquisition only after a safety case, industrial plan and falsifiable full-mission test exist. They may advance to production only after independent trials demonstrate availability and complete service, not component performance alone.

## 8. Decisions carried forward

Pass 61 adopts the ten-class external interface grammar as the Department's first canonical cargo compiler. It requires future force models to report physical mass, chargeable demand, deadline–mode allocation and complete formation equivalents together. It preserves the 20-percent reserve as an explicit claimant pending calibration. It denies receiver and public-effect credit to every current transport record. It holds every cargo profile at hypothesis maturity and blocks platform rendering.

Pass 62's [carrier–node requirements and industrial program](carrier-node-requirements-and-industrial-program.md) supplies the aggregate successor. It carries the common mode–deadline burden into three rival activation, node-release and route-survival architectures. Their required gross 72-hour potential spans 10.048–23.077 million tonnes and their provisional 25-year carrier-and-node programs span $5.222–9.693 trillion. This closes the requirement-envelope method, not the item boundary: road and rail remain combined, coefficients remain hypotheses, receiver admission remains zero and no platform is selected.

The next force-model pass should now construct one **serial representative manifest**. It should tag and measure complete items, preserve complement identity through discrete carrier and node queues, distinguish road from rail, bind routes and origins, and carry arrivals through receiver commissioning under seeded loss. Clean-sheet technology alternatives remain active, but exterior form remains premature.

The consequence for the wider project is positive. The original ambition—a civil force built with defense-scale seriousness—becomes more credible when its spectacular platforms are delayed by harder questions. A Department capable of identifying every required position, reserving the right carrier, creating the receiving node, closing the full formation, protecting the next-event reserve and restoring readiness would possess something the present system does not: **auditable civil force projection rather than hopeful movement capacity**.

## Evidence boundary

All quantitative inputs in this pass are inherited from committed repository hypotheses or declared within the workbook. No external site research is introduced. The result has not been calibrated to observed national disaster cargo, commercial carrier schedules, port or airfield queues, route damage, bills of material, measured position dimensions, hazardous regulations, receiver sites, workforce cycles or lifecycle costs. The routing weights do not identify actual itineraries. Proportional allocation does not identify loaded items. The complete-formation rule is a conservative planning constraint, not a validated service degradation curve.

Accordingly, the workbook is an executable argument about what a credible deployment system must represent. It is not evidence that the United States currently possesses or could immediately procure the modeled capacity. The paper's strongest warranted conclusion is architectural: **tonnage-only planning materially overstates deployable resilience power, and the next serious acquisition object is the complete carrier–node–receiver system.**
