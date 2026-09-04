# PRG-100 configuration model

## Decision purpose

This pass converts the Power Restoration Group 100 (`PRG-100`) from a force-engineering concept into an editable configuration model. Its question is not how many portable generators should be bought. It is:

> What complete deployable electric utility must the Department of Resilience own to deliver 100 MW of safe, continuous critical service when the receiving network may be reusable, bypassable, or functionally absent?

The distinction is decisive. A source produces electrical power. A utility formation turns that power into controlled civilian service across a damaged territory. The formation must discover and prioritize loads; survey an unfamiliar electrical system; isolate unsafe plant; establish voltage and frequency; transform, protect, distribute and meter power; manage storage and fuel; operate around the clock; repair itself; and transfer service without a second outage. These functions are inseparable at campaign level even when they are acquired as different product lines.

The accompanying [`power-restoration-engineering.xlsx`](../models/power-restoration-engineering.xlsx) workbook is the configuration-control object for this stage of the research. It has 17 sheets covering controls, critical loads, network states, source mixes, generation, storage, feeders, transformation, construction, fuel, thermal protection, deployment mass, workforce, failure cases, evidence gates and sources. All consequential design-study inputs are visible. Formulas recalculate when the network or source case changes.

This is an `R2+` model. It closes first-order balances and makes the formation falsifiable. It does not provide a construction-ready one-line, protection study, equipment specification, independent cost estimate or verified performance claim. Renderings remain prohibited.

## Reference configuration

The baseline is a 100 MW net critical-load mission using the `Bypass` network state and the `Liquid fuel dominant` source case. It assumes five electrical islands, ten 34.5 kV feeders, 0.90 power factor, a 30-day campaign, 3% auxiliary load, 10% environmental derating and 20% owned-capacity reserve.

The source mix is deliberately not 100% liquid fuel. Eighty percent of average gross generation is assigned to liquid fuel and 20% to surviving grid or local sources. This lets the baseline represent a severe but not completely electrically sterile environment. The workbook also contains a gas-hybrid case and a surviving-grid/local case. The formation is source-neutral at its common electrical interfaces; mission conditions determine which source modules are attached.

The baseline produces the following configuration:

| Measure | Baseline result | Interpretation |
|---|---:|---|
| Net critical load | 100 MW | Service delivered to registered loads |
| Average network loss | 0.78 MW | Screening loss across 60 circuit-km |
| Average gross dispatched generation | 103.89 MW | Net load plus line loss and auxiliaries |
| Required unrounded owned nameplate | 138.53 MW | Includes derating and capacity reserve |
| Rounded owned source capacity | 140 MW | Fourteen 10 MW modules |
| Current per feeder | 185.94 A | Ten equal 10 MW feeders at 34.5 kV and 0.90 PF |
| Approximate end-of-feeder voltage drop | 0.87% | Screening calculation, not a power-flow study |
| Battery fleet | 140 MW / 140 MWh | Seven 20 MW / 20 MWh reference blocks |
| Mobile substations | 8 × 25 MVA | Capacity floor plus one N-1 reserve |
| Temporary route | 60 circuit-km | 24 km surface cable and 36 km overhead |
| Network setup target | 13.57 days | Twelve parallel work fronts plus commissioning |
| Daily liquid fuel | 152,461 gal/day | 80% liquid share at average gross dispatch |
| Onsite liquid reserve | 1.067 million gal | Seven-day route-interruption stock |
| Onsite liquid mass | 3,372 t | Excluded from dry deployment mass |
| Preliminary dry deployment mass | 18,332 t | Includes 15% configuration contingency |
| Deployed personnel | 2,796 | Shift-complete formation hypothesis |
| Service establishment | 10,485 billets | Three operational echelons plus 25% school/depot overhead |
| Thermal allocation | 20 MWe | Produces 60 MWth at a design COP of 3.0 |
| Concurrent thermal protection | 120,000 people | At 0.5 kWth per person; explicit assumption |

The numbers are useful because they are difficult. A 100 MW response is not a small convoy. Even the bypass case is a heavy engineering formation with a strategic movement problem, a major recurring fuel flow, a large electrical-safety burden and an occupational structure closer to a field utility than a temporary-power team.

## Model architecture

### Controls

The controls sheet distinguishes four input types:

1. **Scenario controls** select the network state, source case and mission.
2. **Design targets** state the intended effect, duration and service allocation.
3. **Engineering assumptions** enable screening calculations but require later validation.
4. **Mass and productivity assumptions** make the preliminary manifest and setup time explicit rather than hiding them inside platform labels.

The model does not use a balancing plug. If an assumption produces an infeasible configuration, the workbook exposes the conflict. The first build did this with mobile transformation: six 25 MVA units—the intuitive rule of one per island plus one reserve—provided only 150 MVA, less than the rounded 140 MW source fleet requires at 0.90 power factor. The rule was corrected to the greater of the island floor and the capacity floor, plus one N-1 reserve. The result is eight units and 200 MVA. This is the intended behavior of a configuration model: attractive verbal shorthand yields to system balance.

### Critical-load registry

The 100 MW objective is allocated across ten provisional civilian load classes:

| Load class | Net MW | Priority role |
|---|---:|---|
| Hospitals and acute care | 22 | P0, with a no-break subset |
| Water treatment and pumping | 10 | P1 |
| Wastewater | 8 | P1 |
| Communications and dispatch | 5 | P0 |
| Shelters and thermal protection | 20 | P1 |
| Food and pharmacy cold chain | 10 | P2 |
| Transit and fuel distribution | 8 | P2 |
| Civil services | 5 | P2 |
| Critical manufacturing and laboratories | 7 | Interruptible |
| Unallocated connection reserve | 5 | Interruptible |

These are design allocations, not claims about a representative city. Their purpose is to force the model to represent different outage tolerances, connection types, power factors, ride-through needs and public consequences. An operational PRG-100 would replace this illustrative registry with a surveyed, time-indexed load model containing motor starts, reactive demand, harmonic sources, daily and seasonal profiles, restoration dependencies and safe shedding sequences.

The registry is also a civil-authority object. Incident leadership determines which civilian outcomes have priority. The PRG commander determines how those priorities can be delivered safely with the available topology, sources and crews. The electrical model must preserve that distinction: a technically convenient load is not automatically the socially correct load.

### Network states

The model compares three configurations.

| State | Total route | Cable / overhead | Nodes | Setup target | Network materials and construction equipment |
|---|---:|---:|---:|---:|---:|
| Reuse | 10 circuit-km | 80% / 20% | 20 | 6.33 days | 449 t |
| Bypass | 60 circuit-km | 40% / 60% | 60 | 13.57 days | 4,115 t |
| Rebuild | 180 circuit-km | 20% / 80% | 120 | 39.29 days | 14,479 t |

`Reuse` means the force has surveyed and accepted existing conductors, clearances, grounding, protection and structures. It still requires temporary ties, transformation, connection packages and repairs. Its speed advantage is purchased with epistemic risk: hidden damage can defeat an otherwise light configuration.

`Bypass` treats the surviving network as locally useful but not trustworthy end to end. The force creates several controlled islands, routes around failed nodes and connects priority facilities through a mixture of protected surface cable and rapid overhead line. It is the baseline because it expresses the defining PRG mission: create a safe substitute network without waiting for normal reconstruction.

`Rebuild` assumes that the original distribution system is absent, inaccessible, contaminated, incompatible or strategically unsuitable. It creates an independent regional bridge network. This is not merely a larger bypass. It changes the formation into a line-construction campaign whose labor, structures, materials, inspection, land access and transfer requirements dominate the source modules.

The model shows why the Department of Resilience should own distinct network packages. The same source fleet should not carry every pole, reel, transformer and construction machine needed for the worst case. A PRG should be composable from a core utility command and source/storage/protection system plus a selected `reuse`, `bypass` or `rebuild` network train.

## Electrical balances

### Feeder current

For balanced three-phase power, feeder current is:

\[
I = \frac{P \times 1000}{\sqrt{3} V_{LL} PF}
\]

where `P` is feeder real power in MW, `V_LL` is line-to-line voltage in kV and `PF` is power factor. Ten equal feeders carry 10 MW each. At 34.5 kV and 0.90 power factor:

\[
I = \frac{10 \times 1000}{\sqrt{3} \times 34.5 \times 0.90} = 185.94\text{ A}
\]

This result is not a conductor selection. It is the starting point for ampacity, insulation, installation, temperature, voltage drop, short-circuit, protection and mechanical design. The configuration deliberately uses medium voltage because 100 MW cannot be responsibly distributed as a collection of low-voltage extension systems.

### Resistive loss

The screening loss is:

\[
P_{loss} = \frac{3 I^2 R L}{10^6}
\]

where resistance is 0.125 ohm/km/phase and `L` is total three-phase circuit-kilometres. For the bypass case:

\[
P_{loss} = \frac{3(185.94)^2(0.125)(60)}{10^6} = 0.778\text{ MW}
\]

This is 0.78% of net load. The corresponding simplified end-of-feeder voltage-drop screen is 0.87% using a 6 km average feeder length and 0.10 ohm/km reactance. These low screening values do not prove the topology. Unequal routes, motor starts, transformer impedance, cold-load pickup, faults, harmonics, unbalance and dynamic source behavior can govern the real design.

### Gross dispatch and owned capacity

Average gross dispatched generation is:

\[
P_{gross} = \frac{P_{net} + P_{loss}}{1-a}
\]

where auxiliary share `a` is 3%. The baseline requires 103.89 MW average gross output.

Owned nameplate must then account for environmental derating `d` and reserve `r`:

\[
P_{owned,unrounded} = \frac{P_{gross}}{1-d}(1+r)
\]

At 10% derating and 20% reserve, this is 138.53 MW. Fourteen 10 MW modules provide 140 MW. Loss of the largest 10 MW module leaves 130 MW, still above average gross dispatch. This passes a static N-1 capacity check; it does not demonstrate transient ride-through, stable island separation or successful restart.

## Storage architecture

Storage is sized against two duties.

The full-load transfer bridge is:

\[
E_{bridge} = 100\text{ MW} \times 0.25\text{ h} = 25\text{ MWh usable}
\]

The P0 endurance requirement is:

\[
E_{P0} = (100\text{ MW} \times 20\%) \times 4\text{ h} = 80\text{ MWh usable}
\]

The larger duty controls. With 80% usable depth, 92% AC conversion efficiency and 20% reserve:

\[
E_{nominal} = \frac{80}{0.80 \times 0.92}(1.20) = 130.43\text{ MWh}
\]

Power capacity must also cover 120 MW after reserve. Seven illustrative 20 MW / 20 MWh blocks produce 140 MW / 140 MWh, satisfying both screens.

This should not be misread as a battery procurement specification. The formation needs at least five storage behaviors: no-break ride-through, grid formation, source synchronization, black-start sequencing and protected reserve. Cell chemistry, thermal propagation, environmental control, state-of-charge policy, inverter fault contribution, motor-start performance and module separation remain open.

## Source and fuel cases

### Liquid-fuel-dominant baseline

Liquid generation is 80% of 103.89 MW, or 83.12 MW average. With a 10,500 Btu/net-kWh heat rate and 137,381 Btu/gallon heat content:

\[
F_{liquid} = \frac{83.12 \times 24{,}000 \times 10{,}500}{137{,}381} = 152{,}461\text{ gal/day}
\]

That is approximately 577 m³/day or 16.9 nominal 9,000-gallon tanker loads every day. A seven-day reserve is 1.067 million gallons and approximately 3,372 tonnes of liquid. The storage inventory exceeds the mass of the entire 140 MW dry source-module fleet. Fuel is therefore not support to the power force; it is one of the force's defining operational systems.

The workbook includes a 100 MW all-liquid benchmark of approximately 183,900 gallons/day. The distinction between the benchmark and the baseline is important: the former isolates source physics, while the latter evaluates an explicit mixed portfolio.

### Gas hybrid

The gas-hybrid case assigns 25% of average gross dispatch to liquid fuel, 55% to gas and 20% to surviving grid or local sources. It reduces liquid demand to approximately 47,644 gallons/day while requiring approximately 12,343 MMBtu/day of gas energy.

The logistical benefit is real, but not free. Gas pressure, composition, compressor power, freezing, pipeline damage and upstream electric dependencies become mission variables. A gas-hybrid PRG needs liquid-fueled black-start capacity and a controlled degradation plan if gas fails. The Department should not encode gas availability into the core formation; it should own interface and conditioning packages that can exploit gas when the receiving environment supports it.

### Surviving grid and local resources

The grid/local case assigns 80% of average gross dispatch to controlled ties and local generation, with 10% liquid and 10% gas. This is the lightest recurring-fuel posture, but it may be the most demanding protection problem. The PRG must determine when remaining connected to an unstable, damaged or weak grid creates more risk than separating. Resynchronization and return of operating authority are command decisions executed through technical procedures, not automatic consequences of available voltage.

## Transformation and protection

The baseline transformation layer contains:

- eight 25 MVA mobile substations, including one capacity reserve;
- 60 distribution nodes with local isolation and load-shed control;
- seven grid-forming control cells;
- five synchronization and controlled-tie packages; and
- 12 grounding and feeder-protection kits.

The preliminary dry mass is 1,376 tonnes. More important than the mass is the configuration problem. Transformer voltage ratios, vector groups, grounding, neutral behavior, impedance, fault duty, tap range, protective-device ratings, insulation, connectors and transport geometry cannot be left to improvisation after arrival.

The Department should create a bounded, configurable transformation portfolio rather than attempt to reproduce every utility's installed diversity. A national portfolio would combine common cores with field-changeable bushings, cable terminations, arresters, grounding packages, relay libraries and adaptation kits. Its industrial program should include depot stocks, rotating reserve, domestic multi-source production, test capacity, transport fixtures and trained commissioning teams.

## Rapid distribution and construction

The bypass network contains 24 circuit-km of surface cable and 36 circuit-km of overhead line. The screening manifest is:

| Element | Baseline quantity | Dry mass |
|---|---:|---:|
| Surface cable sets | 24 circuit-km | 192 t |
| Overhead conductor and hardware | 36 circuit-km | 119 t |
| Poles | 720 | included below |
| Poles, foundations and structures | 720 sets | 2,304 t |
| Construction equipment | route-scaled | 1,500 t |

Structures dominate line-material mass. This is a warning against treating rapid distribution as a cable-reel problem. Pole erection, anchoring, foundations, rights of way, debris removal, crossings, traffic control, grounding, inspection and repair determine what can be energized.

The setup target uses twelve parallel work fronts, a provisional 0.50 km/front-day surface-cable rate, a provisional 0.35 km/front-day overhead rate and five days for survey, protection and commissioning. The slower overhead path controls:

\[
T = \max\left(\frac{24}{12 \times 0.50}, \frac{36}{12 \times 0.35}\right) + 5 = 13.57\text{ days}
\]

These rates are deliberately exposed as open evidence. Real performance will depend on terrain, debris, soil, access, crossings, weather, permitting, daylight, material handling, site preparation and inspection. The next evidence step is a multi-front field trial, not a more precise spreadsheet coefficient.

## Thermal protection

The model allocates 20 MWe to thermal safety. At a coefficient of performance of 3.0, this provides 60 MWth. At an explicit concurrent intensity of 0.5 kWth/person, it supports 120,000 people at one time. Operating for 16 hours produces 1.92 million protected person-hours/day, equivalent to 80,000 people protected continuously.

This calculation is an effect screen. A thermal-protection system also requires heat pumps or chillers, temporary hydronic or air distribution, electrical interfaces, water treatment, filters, refrigerant, shelter-envelope work, ventilation, occupancy controls, accessibility and public-health supervision. Climate, smoke, humidity, building stock and population behavior can invalidate a simple coefficient. The Department should create a `Thermal and Clean-Air Works` program measured in safe occupied people-hours, not tons of cooling equipment delivered.

## Deployment manifest

The baseline preliminary dry mass is 18,331.92 tonnes:

| Category | Dry mass |
|---|---:|
| Fourteen 10 MW generation modules | 2,800 t |
| Seven 20 MW / 20 MWh BESS modules | 1,750 t |
| Transformation and protection | 1,376 t |
| Line materials | 2,615 t |
| Construction equipment | 1,500 t |
| Controls, communications and survey | 400 t |
| Fuel plant and tanks, dry | 500 t |
| Maintenance and workshops | 1,000 t |
| Responder base and logistics | 4,000 t |
| Subtotal | 15,941 t |
| Configuration contingency | 2,391 t |
| Total | 18,332 t |

Stored fuel is reported separately because it is a recurring inventory rather than owned dry equipment. The seven-day baseline stock adds 3,372 tonnes at the incident. Replacement parts, consumables, food, water and daily fuel movement would further increase theater throughput.

The strategic implication is that a PRG-100 requires planned rail, sealift, road, staging, heavy handling and reception. It cannot be made rapidly employable by buying more airlift. The most time-sensitive command, survey, protection, control and connection elements may move by air; the main source, storage, substation, line and construction trains require surface movement. The formation design should separate an early electrical reconnaissance and control echelon from the heavy utility body.

## Workforce and force generation

The deployed personnel model contains ten functional pools: command/grid operations, generation/storage, substations/protection, line construction, connection teams, fuel logistics, maintenance/fabrication, safety/medical/environmental, logistics/camp/movement, and planning/survey/liaison.

Continuous posts use a 4.2-person shift-and-relief factor. Day crews and scaling staff are added explicitly. The baseline produces 2,796 deployed personnel. Three operational echelons require 8,388 billets; a further 25% for schools, depots, doctrine, test, replacement and institutional overhead brings the service establishment to 10,485 billets.

This is not a validated table of organization. It is a warning against platform-centric manpower accounting. Every 24/7 control position creates more than one billet. Every specialized relay, transformer, inverter, fuel-quality and high-voltage task creates a training and certification pipeline. A mature Department of Resilience would require licensed electrical professionals, protection engineers, grid operators, lineworkers, heavy-equipment operators, power-generation technicians, battery specialists, fuel specialists, safety officers, logisticians and maintainers in active and reserve structures.

The force-generation consequence is material. If one PRG-100 is to remain continuously deployable, the Department likely needs at least a deployed, ready and reset/training set of people and equipment, plus attrition and depot reserve. The workbook applies three echelons to personnel only; a future national order-of-battle model must apply formation-specific availability, overhaul, training and transportation constraints to equipment as well.

## Failure logic

The workbook tests twelve reference failures:

1. largest source-module loss;
2. one feeder fault;
3. one mobile-substation loss;
4. fuel-route interruption;
5. control-network failure;
6. loss of one battery block;
7. high-ambient derating;
8. missing or incorrect utility drawings;
9. skilled-crew loss;
10. a 90-day campaign;
11. common fuel contamination; and
12. protection miscoordination.

The static model closes the largest-source, modeled-derating and seven-day liquid-reserve arithmetic. Other cases are bounded or open. Three failure families deserve special institutional treatment.

**Common-mode failures** can defeat nominal modularity. Contaminated fuel, shared firmware, incorrect relay settings or a common connector defect can remove multiple independent modules. The Department needs independent test, quarantine and configuration-control authority.

**Knowledge failures** are physical failures in disguise. Missing drawings, unknown grounding and unclear ownership can prevent safe energization even when equipment is present. Survey, mapping, test and liaison are therefore operational capacity, not headquarters overhead.

**Duration failures** reveal the difference between response and force generation. A system that works for 72 hours may fail over 30 or 90 days because of filters, lubrication, battery degradation, crew fatigue, component lead times or accumulating configuration drift. Endurance tests must include maintenance, replacement and rotation.

## Network-state sensitivity

Changing only the network-state control produces:

| State | Setup target | Preliminary dry deployment mass | Change from bypass |
|---|---:|---:|---:|
| Reuse | 6.33 days | 13,932 t | −4,400 t |
| Bypass | 13.57 days | 18,332 t | baseline |
| Rebuild | 39.29 days | 30,757 t | +12,425 t |

Source and storage capacity remain broadly constant because the delivered-load objective is unchanged; feeder losses change modestly with route length. The major swing is the distribution system. This validates the Pass 9 decision to make network state a primary force variable.

The result also suggests a doctrine of **selective substitution**. A catastrophe command should not choose one state for an entire metropolitan area. It may reuse a safe utility island around hospitals, bypass a damaged substation corridor and rebuild a separate network serving shelters and water works. Future versions should therefore allow mixed route segments and staged transition among states.

## Industrial program implied by the model

A mature PRG industrial base would contain several product and production systems, not one prime contractor's vehicle program:

1. **Modular source family.** Grid-forming, black-start-capable source blocks with common AC, fuel, control, cooling and maintenance interfaces.
2. **Storage and power-electronics family.** Separated battery blocks, inverters, DC systems and black-start controllers designed for transport, environmental exposure and field replacement.
3. **Mobile transformation family.** Configurable substations, transformers, switchgear, grounding systems, controlled ties and adaptation kits.
4. **Rapid distribution family.** Surface cable, overhead structures, reels, connectors, protection, crossings, repair kits and instrumented service points.
5. **Electrical construction fleet.** Purpose-built pole/foundation machines, cable handlers, trench and surface-protection systems, access equipment and autonomous survey tools.
6. **Fuel-assurance family.** Receiving, storage, filtration, sampling, fire protection, metering and multi-fuel conditioning.
7. **Digital utility stack.** Offline-capable mapping, load registry, protection libraries, grid control, maintenance records and manual-safe local control.
8. **Depot and proving-ground system.** Transformer and inverter test bays, high-power hardware-in-loop facilities, environmental chambers, line-construction courses and campaign endurance ranges.

This architecture supports the user's central industrial proposition. Lockheed Martin-scale resilience companies would not merely manufacture emergency equipment. They would integrate complete civilian-effect systems, carry configuration and safety responsibility, maintain warm production capacity, support depots and field service, and compete on verified time-to-service, availability and lifecycle performance.

The Department should preserve multiple integrators and component sources. A single national prime could create dangerous common modes and brittle production. The government should own interface standards, reference architectures, test data and the right to re-compete modules. The recurring demand signal should come from fleet recapitalization, reserve stocks, exercises, domestic utility hardening and allied exports—not only post-disaster supplemental appropriations.

## Acquisition object

The acquisition unit is one ready utility formation increment, not a list of equipment. A PRG-100 program increment includes:

- certified delivered-load capacity under defined network states;
- people, qualifications and relief;
- source, storage, transformation, protection and distribution hardware;
- line-construction and connection tools;
- fuel plant and quality assurance;
- command, survey, mapping and communications;
- maintenance, spares and depot capacity;
- strategic transport fixtures and reception equipment;
- training devices, ranges and exercises;
- replacement and reconstitution stock;
- environmental, safety and transfer packages; and
- a measured regeneration time after deployment.

Contract incentives should use civilian-effect metrics: time to first safe P0 service, time to 25/50/75/90% registered load, service availability, unscheduled P0 energy not served, safe connection rate, fuel consumed per delivered critical MWh, network construction rate under specified conditions, repair time and transfer without a service cliff.

## R3 evidence gate

Fifteen gates control advancement:

| Gate | Current state | Proof required |
|---|---|---|
| Load registry | Model closed | Sourced regional demand datasets and time series |
| Network topology | Model closed | Survey and tabletop selection tests |
| Power flow | Bounded | Detailed multi-case load-flow studies |
| Protection and grounding | Open | Fault, grounding and hardware-in-loop tests |
| Generation N-1 | Model closed | Integrated source-trip test |
| Storage dynamics | Bounded | Dynamic model and full-scale test |
| Fuel sustainment | Bounded | 30- and 90-day logistics demonstration |
| Construction productivity | Open | Multi-front field trial |
| Strategic mobility | Open | Itemized lift and reception model |
| Connection interfaces | Open | Facility-interface prototypes |
| Thermal protection | Bounded | Integrated shelter-system field test |
| Workforce endurance | Open | 30- and 90-day duty-cycle trial |
| Maintainability | Open | Reliability and maintainability program |
| Cyber and manual mode | Open | Red-team and disconnected manual-operations test |
| Cost and industrial base | Open | Vendor studies and configuration-level cost model |

No gate is `Verified`. The model therefore advances PRG-100 from `R2` to `R2+`, not to `R3`.

## Verification

The workbook was exported, re-imported and checked after creation. Verification confirmed:

- all 17 sheets are present;
- no formula error token is present;
- controls are restored to `Bypass` and `Liquid fuel dominant` in the delivered file;
- reuse is lighter and faster than bypass;
- rebuild is heavier and slower than bypass;
- gas hybrid materially reduces liquid demand and creates nonzero gas demand;
- maturity remains `R2+` and rendering remains prohibited;
- the largest-source static capacity check passes;
- the mobile-substation capacity check passes after the configuration correction; and
- independent calculations reproduce feeder current, line loss, gross generation, source-module count, BESS count, line mass, setup time, fuel demand and total dry mass to numerical precision.

The independent baseline recomputation used no workbook formulas. Its values matched the exported workbook:

| Check | Independent | Workbook |
|---|---:|---:|
| Feeder current | 185.942 A | 185.942 A |
| Resistive loss | 0.77793 MW | 0.77793 MW |
| Gross dispatch | 103.89477 MW | 103.89477 MW |
| Source modules | 14 | 14 |
| BESS modules | 7 | 7 |
| Line-material mass | 2,614.8 t | 2,614.8 t |
| Setup target | 13.57143 d | 13.57143 d |
| Liquid fuel | 152,460.57 gal/d | 152,460.57 gal/d |
| Dry deployment mass | 18,331.92 t | 18,331.92 t |

## Limits

The workbook should not be used as:

- an electrical construction design;
- a claim that 100 MW is sufficient for a defined population;
- a sourced facility-load estimate;
- a conductor, transformer, inverter, generator or battery specification;
- a verified installation-rate forecast;
- a transport plan;
- a safety case;
- a staffing authorization;
- a lifecycle cost estimate; or
- evidence that one source portfolio is nationally optimal.

Equipment masses are screening assumptions. The line model is balanced and static. It excludes detailed power flow, fault contribution, sequence networks, grounding, relay coordination, harmonics, arc flash, transient stability, cold-load pickup, motor starts, power quality and electromagnetic compatibility. The fuel model excludes delivery loss, idle and part-load penalties, maintenance outages, seasonal fuel properties and safety separation. The thermal model is a first-order effect conversion. The workforce model does not yet map occupations, grades, licenses, attrition, training throughput or reserve availability.

## Decisions

This pass makes six force-design decisions.

1. **Retain Department of Resilience as the institutional name.** The PRG is an operating formation within a cabinet-level department, not an expanded FEMA mission or a military support detachment.
2. **Advance PRG-100 to R2+.** First-order service, electrical, storage, fuel, network, mass and personnel balances cohere.
3. **Create separate reuse, bypass and rebuild network trains.** Network state changes the formation more than source nameplate does.
4. **Size transformation by capacity and N-1, not island count alone.** The model's first failed check demonstrated why configuration balance must govern doctrine.
5. **Treat fuel assurance and electrical construction as coequal system families.** Neither is ancillary support to generation.
6. **Keep rendering prohibited.** The visible asset should emerge only after the one-line, protection, mobility, construction, maintainability and workforce gates close.

## Next research

The next power pass should not add more conceptual equipment. It should close one of the decisive open evidence blocks:

1. build sourced hourly load archetypes for at least three regional disaster cases;
2. create a mixed-state one-line and run power flow, fault, grounding, protection and transient cases;
3. replace mass assumptions with a configuration-controlled equipment and connector manifest;
4. build the item-level strategic movement and reception model;
5. design and cost a multi-front line-construction demonstration;
6. build occupation, certification, shift, attrition and school-pipeline schedules;
7. add 30- and 90-day maintenance, spares and fuel-quality models; and
8. develop the configuration-level cost and industrial capacity model.

Only after these steps should the Department choose a physical layout and commission a rendering. At that point, the image will express a tested operating system rather than substitute visual confidence for engineering knowledge.
