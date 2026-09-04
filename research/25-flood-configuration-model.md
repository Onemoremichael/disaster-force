# Flood hydraulic-control configuration model

## Decision purpose

This pass converts the flood-force architecture into an editable formation model. Its question is not how many pumps, boats or temporary barriers the Department of Resilience should buy. It is:

> What complete combination of forecast, decision authority, pumping, intake, conveyance, receiving water, barriers, interior drainage, breach control, amphibious access, earthworks, contamination control, strategic movement, workforce and industrial capacity can produce a safe hydraulic effect before a flood crosses a consequential threshold?

The answer is a two-force architecture with a non-negotiable systems boundary. The geographically distributed **Flood Intercept Network** (`FIN`) buys early action. Deployable inland and coastal **Hydraulic Control Groups** (`HCG-100`) buy sustained regional work. Neither is independently sufficient. A fast cell can act before the threshold while lacking enough hydraulic capacity to reverse the event. A heavy group can eventually control storage while arriving after a flash-flood or structural-failure threshold. The national capability must overlap them: FIN cells sense, isolate, rescue, protect critical nodes and prepare interfaces while HCG formations generate, move and assume the campaign.

The accompanying [`flood-hydraulic-control-engineering.xlsx`](../models/flood-hydraulic-control-engineering.xlsx) workbook contains 29 linked sheets. It is a design-study instrument, not an incident forecast, civil-works design, environmental authorization, navigation plan, acquisition estimate or performance claim. Yellow cells are editable assumptions; blue cells are calculated results. Three formations and five flood cases recalculate through the same visible logic.

The integrated `FIN` and `HCG-100` concepts advance from `R2` to `R2+`. The model now closes first-order time, hydraulic, access, mass, workforce, readiness and portfolio balances well enough to expose contradictions and direct experiments. It does not advance any pump, barrier, craft, robot or works carrier to `R3`. All twenty evidence gates remain open. Rendering remains prohibited.

## What the model changes

The model changes the meaning of “capacity.”

1. **Installed flow is not delivered hydraulic effect.** A group named for 100 m³/s does not move 100 m³/s merely because its unit nameplates sum to that number. Head, availability, intake condition, debris, pipe or channel capacity, receiving-water stage, environmental controls and power all constrain the same flow.
2. **Early action and regional control are different production systems.** FIN is positioned to beat forecast or detection thresholds. HCG is organized for high-mass, multi-day civil works. The scenario matrix shows that a formation can score nearly 100% action-before-threshold probability while its basin storage is still growing.
3. **Water has to go somewhere lawful and stable.** Pumps are only the middle of a mission thread. The Department must own or create intake structures, pipes, channels, crossings, discharge structures, receiving capacity, quality monitoring and authority to operate them.
4. **Exclusion creates a second hydraulic system.** A barrier that keeps river or surge water out can trap rainfall, sewer backflow and leakage behind it. Every modeled case has a negative interior-drainage margin under the provisional 15% pump allocation. A barrier battalion without protected-side drainage can manufacture the failure it was sent to prevent.
5. **Breach arrest precedes dewatering.** The reference levee breach initially passes about 165.7 m³/s. Under the degraded head, intake, debris and formation-utilization assumptions, the inland HCG delivers only 18.0 m³/s and the coastal HCG 17.0 m³/s. Pumping downstream of an open breach is a losing sequence; the force must reduce and stabilize the breach first.
6. **Hydraulic power projection is materially heavy.** The inland reference configuration is approximately 79,391 tonnes dry, of which about 66,844 tonnes requires external lift under the provisional self-deployment assumptions. Large-bore route material—not the pump wet ends—is the largest single manifest line.
7. **Novel technology must change a visible operational coefficient.** The Department is not restricted to current pump, pipe, barrier, craft or autonomy performance. Its research programs are legitimate only when they target action time, full-curve availability, route mass and setup, breach-flow reduction, safe operating envelope, machine productivity, contamination assurance or another measurable mission variable.

## Workbook architecture

The 29 sheets form eight analytical layers.

| Layer | Sheets | Function |
|---|---|---|
| Mission controls | Summary & Sources; Controls; Flood Cases | Select formation and flood case; expose readiness, reserve, energy, environmental and portfolio assumptions |
| Time and consequence | Forecast Action Clock; Basin Zones; Storage Mass Balance | Build the detection-to-effective-action distribution, allocate consequences and track stored water over 45 days |
| Hydraulic train | Pump Families; Pump Curves Availability; Power Fuel; Intake Debris; Drainage Spine; Receiving Discharge | Convert nominal equipment into the minimum shared flow supported by wet ends, intake, routes, power and receiving water |
| Exclusion and failure control | Barrier Geometry Loads; Interior Drainage; Breach Growth Arrest | Represent barrier geometry, material, loading, hold, protected-side drainage and breach sequencing |
| Human access | Rescue Demand Search; Amphibious Cycles; Access Logistics | Convert stranded population and wet-gap demand into search, patient, people and cargo cycles |
| Heavy work and environmental effect | Earthworks Material; Contamination Treatment; Infrastructure Protection | Represent machine production, competing material flow, hazardous-water isolation and critical-node throughput |
| Formation and national force | Deployment Manifest; Workforce Rotation; Readiness Concurrency; Works Carriers | Calculate deployment mass, shift-complete staff, institutional billets, ready packages, pump order of battle and carrier interfaces |
| Innovation and assurance | Technology Roadmap; Cost RDT&E; Failure Modes; R3 Evidence Gate | Link operational deficits to research campaigns, capital, degraded cases and independent evidence |

The workbook does not produce a single success score. It reports time, net basin removal, interior drainage, breach ratio, rescue clearance, cargo margin, material tempo, contamination utilization, deployment mass and evidence state separately. That is deliberate. Flood response contains competing objectives and stop conditions that cannot be responsibly hidden inside a weighted index.

## Reference formations

The model compares three operational echelons.

| Formation | P50 / P90 complete action | Pump portfolio | Principal package | Dry mass | Deployed / service establishment |
|---|---:|---:|---|---:|---:|
| FIN Regional Cell | 4 / 10 h | 7 m³/s nominal | 10 pumps, 6 pipe paths, 5 km barrier, 42 access vehicles/craft, 16 machines, 4 survey teams | 12,682 t in trapped-basin case | 3,447 / 12,926 billets |
| Inland HCG-100 | 24 / 48 h | 100 m³/s nominal | 36 pumps, 32 pipe paths plus 30 m³/s channel, 40 km barrier, 100 access vehicles/craft, 140 machines, 16 survey teams | 79,391 t | 7,039 / 26,394 billets |
| Coastal HCG-100 | 36 / 72 h | 104 m³/s nominal | 30 pumps, 24 pipe paths plus 60 m³/s channel, 30 km barrier, 94 access vehicles/craft, 108 machines, 20 survey teams | 73,912 t in compound case | 7,166 / 26,874 billets |

Mass changes slightly by flood case because barrier length and environmental packages change. The formation packages are not optimized tables of organization. They are sufficiently explicit hypotheses to reveal which assumptions must be replaced by evidence.

The large FIN mass is itself a warning. A regional cell should probably be divided into an always-ready alert element, locally cached hydraulic modules and a mobilized support echelon. The workbook currently carries them as one package so the project cannot obtain fast response by making the movement burden disappear.

## Complete action clock

The modeled action clock ends only when an intervention produces effect:

\[
T_{action}=T_{forecast/detect}+T_{verify}+T_{decide}+T_{mobilize}+T_{travel}+T_{site}+T_{effective}
\]

Each formation has P50 and P90 stage allocations. The screening probability uses a logistic cumulative distribution whose location is the P50 and whose scale is selected so the P90 is exactly the 90th percentile:

\[
s=\frac{T_{90}-T_{50}}{\ln 9}
\]

\[
P(T\leq T_{threshold})=\frac{1}{1+\exp[-(T_{threshold}-T_{50})/s]}
\]

This is not an empirically fitted response distribution. It makes the value of the tail visible. A force that cuts the median while leaving mobilization, route or site-setup failures in the tail has not achieved the desired readiness. Field exercises must eventually measure the correlated stage times by hazard, geography, warning quality, infrastructure state, crew posture and false-alarm load.

The action result must be read beside the hydraulic result. Against the trapped urban basin, FIN has a 99.9% modeled probability of acting before the 24-hour threshold, but its 3.6 m³/s effective pumping leaves day-zero net removal at −16.9 m³/s. It is early and overmatched. The inland HCG acts by that threshold only 50% of the time, but once operating it produces +16.1 m³/s day-zero net removal. This is the quantitative reason the Department needs both systems.

## Hydraulic train

The model calculates available pump-family flow as:

\[
Q_{available,i}=N_iQ_iA_iH_iI_iD_i
\]

where `N` is quantity, `Q` design flow, `A` availability, `H` head derating, `I` intake factor and `D` debris factor. It then constrains group flow by the complete hydraulic train:

\[
Q_{effective}=\min(Q_{pump/intake},Q_{spine},Q_{receiving},Q_{power})
\]

For the inland HCG against the trapped-basin case, the four capacities are:

| Shared constraint | Capacity |
|---|---:|
| Pump family after unit availability, head, intake/debris and formation utilization | 36.551 m³/s |
| Rapid Drainage Spine | 113.394 m³/s |
| Receiving-water allowance | 76.950 m³/s |
| Power-equivalent flow | 167.176 m³/s |

The pump/intake and formation-duty train binds. The result is not an argument for naming the formation `HCG-37`. `HCG-100` identifies its installed gross water-movement portfolio. The design task is to make the difference between installed and effective capacity explicit, to decide how much reserve is justified, and to determine whether different heads require different module mixes or separately generated sub-formations.

The four provisional pump classes range from 0.25 m³/s tactical high-head units to 20 m³/s barge or closure stations. Their common electric and control interfaces do not imply common wet ends. High head, axial basin drainage, sediment, trash, cavitation, fish protection, saltwater, corrosion and endurance impose different physical designs. A modular family should standardize power electronics, controls, instrumentation, couplings, maintenance data and transport interfaces while preserving hydraulic specialization.

At effective flow `Q`, total dynamic head `H` and combined efficiency `η`, input power is:

\[
P=\frac{\rho gQH}{\eta}
\]

The urban baseline uses 6.56 MW at 36.551 m³/s and 15 m head. With 10% auxiliaries and 25% reserve it requires 9.02 MW installed. The selected inland package carries 30 MW, leaving power well above the current pump/intake bottleneck. A 60% liquid-electric share produces a screening demand of 7,219 gallons/day at the assumed heat rate. This source mix is editable: safe grid, PRG modules, storage, gas, marine power or other sources can serve the common bus. The model does not award a nuclear carrier any hydraulic credit.

## Time-indexed basin balance

For each day `t`, the storage model evaluates:

\[
S_{t+1}=\max\{0,S_t-86400(Q_{gravity,t}+Q_{pump,t}-Q_{base,t}-Q_{rain,t}-Q_{breach,t})\}
\]

Base and rain inflows decay by a case-specific retention factor. That simple decay is a transparent stress assumption, not hydrology. It explains why a case can have negative day-zero removal but still drain after the peak inflow recedes. Future versions require sub-daily hydrographs, elevation–storage curves, connected zones, pump cutoffs, tide windows, rainfall ensembles, infiltration, sewer behavior and uncertainty.

The 15 formation–case combinations expose distinct regimes:

| Formation | Case | Act before threshold | Effective pump | Day-zero net | First zero-storage day | Interior margin | Breach/pump |
|---|---|---:|---:|---:|---:|---:|---:|
| FIN | Trapped urban | 99.9% | 3.6 m³/s | −16.9 m³/s | none in 45 d | −18.5 m³/s | 0 |
| FIN | Forecast river | 100.0% | 3.2 | −50.8 | none | −51.3 | 0 |
| FIN | Flash pluvial | 50.0% | 2.7 | −65.3 | 9 d | −13.9 | 0 |
| FIN | Coastal compound | 100.0% | 2.7 | −142.3 | none | −65.3 | 0 |
| FIN | Levee breach | 32.5% | 1.8 | −194.5 | none | −13.2 | 93.9× |
| Inland HCG | Trapped urban | 50.0% | 36.6 | +16.1 | 28 d | −14.0 | 0 |
| Inland HCG | Forecast river | 90.0% | 42.2 | −11.8 | none | −46.7 | 0 |
| Inland HCG | Flash pluvial | 13.8% | 31.2 | −36.8 | 4 d | −9.7 | 0 |
| Inland HCG | Coastal compound | 75.0% | 36.4 | −108.6 | none | −61.3 | 0 |
| Inland HCG | Levee breach | 11.8% | 18.0 | −178.3 | none | −11.3 | 9.2× |
| Coastal HCG | Trapped urban | 32.5% | 34.6 | +14.1 | 30 d | −14.3 | 0 |
| Coastal HCG | Forecast river | 67.5% | 41.0 | −13.0 | none | −46.5 | 0 |
| Coastal HCG | Flash pluvial | 12.4% | 30.0 | −38.0 | 4 d | −9.9 | 0 |
| Coastal HCG | Coastal compound | 50.0% | 36.6 | −108.4 | none | −61.0 | 0 |
| Coastal HCG | Levee breach | 11.2% | 17.0 | −179.2 | none | −11.5 | 9.7× |

“None” means the basin does not reach zero storage within the 45-day screen. The flash cases drain despite negative day-zero removal only because their inflows decay rapidly under the stated assumption. No operational conclusion should be drawn without calibrated hydrographs and receiving-stage behavior.

Several strong design judgments survive that caveat. FIN is an intercept, rescue and interface-preparation force, not a substitute HCG. The HCG can control some trapped or forecast river cases while still being too slow for flash thresholds. Open breaches dominate pumping. And protected-side drainage is an independent formation obligation, not a small allowance inside the primary dewatering total.

## Barrier, breach and interior-drainage architecture

The baseline barrier mix combines local earth fill, water-ballast sections, structural panels and tension membranes. A 20 km deployed screen produces a provisional 91.85% length-weighted hold probability and 2,980 tonnes of non-local barrier-system mass, while the large earth volume is treated as local material demand. These numbers do not establish reliability. The model omits foundation variability, seepage paths, transitions, terminations, overtopping duration, wave and debris impulses, settlement, scour and human installation error.

The most important barrier output is negative: with 30 km² protected, 50 mm/day rainfall, 80% runoff, 5 m³/s sewer inflow and a simple leakage allowance, total interior inflow is about 19.49 m³/s. A 15% allocation of the HCG's effective flow supplies only 5.48 m³/s, leaving a −14.01 m³/s margin. The architecture therefore needs dedicated protected-side drainage trains, controllable sewer isolation, local sumps and channels, source separation and a barrier-control system that reports interior state—not merely crest integrity.

The breach screen uses:

\[
Q_b=C_db\sqrt{2g}h^{3/2}
\]

For `b = 12 m`, `h = 3 m` and `C_d = 0.6`, initial flow is 165.7 m³/s. The provisional arrest concept reduces flow to 25% after six to eight hours, but that factor receives no force credit beyond the transparent scenario calculation. It must be demonstrated across soil, foundation, geometry, current, debris, access and widening states. The proper `ARPA-R` objective is not a dramatic plug silhouette. It is a measured reduction in breach growth and discharge, followed by filter-compatible closure and durable transfer.

## Amphibious access, search and heavy work

The access model retains five platform classes: shallow urban craft, swiftwater rescue craft, high-water land carriers, heavy amphibious logistics vehicles and coastal or surf craft. Quantity, mission payload, cycle time, operating hours, availability and case suitability produce people and cargo throughput. The inland baseline moves 15,315 people/day in the cycle screen and clears 40,000 stranded people in 2.61 days before search, patient acuity, shore congestion and destination capacity are imposed.

That result is intentionally incomplete. Rescue demand is divided into known occupied locations, door-to-door search, self-reported distress, institutional facilities and animal/family support. Each has different search time, medical share, accessibility requirement and priority. Future models must couple search-team hours and uncertainty to vehicle cycles so a large fleet cannot claim to move people it has not located, assessed or safely transferred.

Earthworks are represented as crewed and robotic production, with barrier material, breach closure and debris competing for the same machine-hours. The urban baseline requires 8.55 days to complete the provisional handled-material set. This is a key technology opportunity: optionally crewed machines can reduce exposure and extend work into contamination, unstable banks and current. But autonomy must demonstrate soil and debris perception, ground-pressure performance, tool change, productive local control, safe stop, lost-link operation, recovery and field repair. Removing an operator from the cab does not remove the human institution; it moves labor into mission planning, supervision, maintenance, recovery and assurance.

## Deployment, workforce and readiness

The inland HCG baseline manifest is approximately 79,391 tonnes dry after a 15% configuration contingency. Major lines include:

| Manifest element | Dry mass |
|---|---:|
| Drainage Spine material | 27,600 t |
| Spine handling and crossings | 6,900 t |
| Earthworks fleet | 6,600 t |
| Water-quality plant | 5,000 t |
| Command and sustainment | 5,000 t |
| Pump modules | 4,150 t |
| Rescue base and decontamination | 4,000 t |
| Barrier system excluding local earth | 2,980 t |
| Workshops and spares | 2,950 t |
| Amphibious fleet | 2,016 t |
| Pump power plant | 1,200 t |
| Sensors and survey | 640 t |

The pipe-route system and its handling allowance together account for 34,500 tonnes before joints, anchors, valves, some crossings and recovery reserve are fully specified. This is the clearest warning against the claim that drone fleets can simply “lay pipelines.” Autonomy can survey routes, pull pilot lines, position light elements, inspect joints and coordinate machine teams. Large-bore hydraulic mass still requires freight, ground bearing, crossings, cranes, joints, anchorage, pressure control and recovery.

The baseline establishment is 5,631 direct deployed positions plus 1,408 common-support positions, or 7,039 deployed people. The 3.75 institutional multiplier produces 26,394 service billets. This is not a personnel authorization. It demonstrates that a 24-hour hydraulic formation is an operating institution of pump crews, craft crews, machine teams, surveyors, environmental staff, barrier and breach teams, maintainers, logistics, health, command, schools and depot depth.

The illustrative national screen carries 40 FIN cells, ten inland HCGs and six coastal HCGs. At 80% FIN and 75% HCG readiness, it yields 32, seven and four ready packages against simultaneous requirements of twenty, four and two. The simple count does not yet model correlated regional demand, maintenance cohorts, base loss, damaged transport, equipment cannibalization, training draws or reconstitution.

The resulting pump order of battle is 1,176 owned units after a 25% procurement reserve: 770 tactical, 285 regional, 93 axial and 28 barge-class units. At provisional unit prices, pump hardware alone screens at $35.375B. This is not a pump-program cost. It excludes research, full drive and intake systems, drainage routes, power, spares, training, bases, depots, software, environmental systems and lifecycle support.

## Technology strategy beyond the current state of practice

The user-directed premise is that the Department may drive new technology with the ambition historically associated with defense programs. The model therefore treats present equipment as a lower-bound comparator, not a ceiling. Ten `ARPA-R` flood campaigns target mission variables:

- **Flood state in minutes:** dense expendable sensing, resilient local gages, autonomous bathymetry, surface-water radar, levee telemetry, data assimilation and uncertainty-aware edge models that keep operating without a cloud connection.
- **Megaflow modular pumping:** 1–15 m³/s modules with swappable wet ends, common high-voltage electric drives, wide solids passage, condition-based maintenance, automated priming, fast manifold connection and verified 30-day endurance.
- **Rapid Drainage Spine:** light high-strength large-bore sections, semi-flexible joints, active surge suppression, self-surveying anchors, reusable crossings and robotic assembly that reduce tonnes and setup hours per delivered m³/s-km.
- **Adaptive barriers:** instrumented, repairable systems that sense seepage, foundation movement, load history and interior water; change geometry or ballast; and share standardized sockets with pumps, drains and closures.
- **Active breach arrest:** staged structures, membranes, flow-guided elements, granular filters and autonomous placement that reduce widening and discharge under live flow before permanent closure.
- **Flood autonomy:** cooperative aerial, surface and underwater systems for mapping, inspection, marker placement, intake clearing, line pulling, search and infrastructure assessment under debris, current and communications loss.
- **Optionally crewed earthworks:** common heavy-work carriers with machine-readable tasks, local supervisory control, wading and soft-ground kits, standardized tools, safe stop and assisted recovery.
- **Purpose-built amphibious access:** separate hydrodynamic families for urban shallows, swiftwater, high-water land movement, heavy wet-gap logistics and coastal surf, unified by patient, accessibility, sensing, decontamination and maintenance interfaces.
- **Contamination-aware dewatering:** real-time field characterization, high-hazard stream isolation, modular treatment and containment, monitored discharge and traceable residuals rather than the fiction that all moved water is beneficial.
- **Hydraulic works carriers:** shallow-draft riverine and seagoing coastal mobile work bases with cranes, workshops, pump and pipe handling, electric distribution, small-craft support and shore-interface systems. A nuclear coastal water–energy variant remains held behind comparative energy, licensing, security, heat-rejection and lifecycle evidence.

Every campaign has a failure trigger and a model variable. This is how the Department avoids technological theater. If a lighter pipe cannot survive pressure transients, if an autonomous machine cannot recover from bogging, if a barrier cannot report dangerous seepage, or if a high-flow pump cannot tolerate real debris for thirty days, the formation does not receive the claimed performance.

The research enterprise should be built around destructive proving complexes, not demonstrations optimized for success. Instrumented basins, flowing breach ranges, movable-bed channels, contaminated-water loops, surf and current facilities, full-scale route corridors, lost-link autonomy trials and multi-week endurance campaigns should be operated by an independent Resilience Test and Evaluation Authority. Suppliers should be paid for data, reproducibility, open interfaces and demonstrated mission effect as well as delivered hardware.

## Industrial and capital implications

The $1 trillion real-2026-dollar capital and RDT&E thought experiment remains:

| Portfolio | Allocation |
|---|---:|
| Research, prototypes and independent test | $130B |
| Pumps, power interfaces and drainage spines | $220B |
| Amphibious rescue and logistics | $150B |
| Barriers, breach and autonomous earthworks | $160B |
| Hydraulic intelligence and communications | $80B |
| Riverine and coastal hydraulic works fleet | $90B |
| Regional bases, prepositioning and stocks | $70B |
| Industrial expansion and multi-source supply | $45B |
| Workforce, academies and exercises | $30B |
| Program reserve and uncertainty | $25B |

Routine personnel and operations are excluded. The allocations are a strategic research and industrial design, not a cost estimate or budget request.

The national pump-hardware screen and one inland carrier together use $36.575B against $310B of the two relevant portfolio lines, leaving $273.425B. That remainder is not savings. It indicates the share that must fund development, intake and route systems, power, mission equipment, spares, bases, test, depots, ports, training, support and failed pathways. A mature industrial base resembles a civil arsenal: multiple qualified pump and drive producers; composite and metal route factories; barrier and geotechnical suppliers; amphibious and work-machine yards; sensor and power-electronics firms; contamination-process manufacturers; software and controls providers; depots; ranges; and surge contracts. The economic opportunity is the interoperable system and its standards, not simply export sales of a dramatic platform.

## Failure modes and doctrine

The workbook retains fifteen explicit failure modes: forecast error, interior flooding, pump underperformance, closed receiving windows, intake clogging or cavitation, breach dominance, craft mismatch, autonomy loss, contamination export, route failure, crew exhaustion, temporary-works persistence, second-event concurrency, power-source failure and drainage-joint or anchor failure.

These translate into doctrine:

1. The hydraulic commander owns the complete source-to-receiver balance, not only pump dispatch.
2. Technical authority can refuse unsafe barrier, breach, electrical, navigation or environmental operation.
3. Forecast uncertainty triggers staged posture and reserve; it does not become a single authoritative map.
4. Barriers are commissioned with interior drainage and inspection plans.
5. Breach flow is reduced before basin pumping receives success credit.
6. Rescue craft are assigned by depth, velocity, debris, surf, access, patient and recovery envelope.
7. Environmental characterization and residual handling are continuous operational functions.
8. Temporary works have transfer, inspection, maintenance, removal and recovery criteria before deployment.
9. National readiness is judged after the first campaign has consumed crews, spares and transport.

## Verification and maturity decision

The workbook was exported, re-imported and recalculated across all fifteen formation–case combinations. All 29 sheets were rendered and visually inspected. Pre-export, post-import and independent formula-error scans returned zero spreadsheet-error matches. Independent verification performed 237 checks covering sheet structure, scenario switching, action clocks, hydraulic minimums, pump-family derating, power, zone totals, pipe geometry, barrier weighting, interior drainage, breach logic, all 45 storage recursions, rescue, cargo, earthworks, contamination, manifest, workforce, readiness, capital, evidence gates, package integrity and file identity; no check failed. The repository and generated workbook hashes were identical.

This supports `R2+` for the integrated `FIN` and `HCG-100` configurations. It does not establish physics closure. The most consequential open evidence is:

- empirical correlated action-time distributions;
- calibrated sub-daily basin, zone and receiving-water models;
- complete pump curves under head, solids, submergence, wear and endurance;
- intake, debris, cavitation and maintenance trials;
- drainage-spine transients, joints, anchors, crossings, setup, leaks and recovery;
- barrier foundations, seepage, overtopping, termination and interior drainage;
- live-flow breach growth, reduction and closure;
- amphibious stability, maneuver, wake, patient and decontamination performance;
- autonomy, earthwork productivity, recovery and maintainability;
- environmental sampling, treatment, discharge and residuals;
- itemized deployment, route and sustainment manifests;
- qualification pipelines, readiness correlation, lifecycle cost and complete mission-thread test.

All twenty R3 gates therefore remain open. Renderings of pumps, craft, barriers, robotic machines and works carriers remain prohibited. The next useful pass is not a beauty view. It is an empirical research plan that assigns experiments, ranges, prototypes, measurements, failure criteria, schedules and budgets to the few variables that most change mission outcome: the action tail, full-curve pump availability, route mass and setup, interior-drainage capacity, breach-flow reduction and safe amphibious access. Pass 15 implements that plan in [Inventing the flood force: research, prototyping and independent test](26-flood-research-test-and-evaluation.md) and the editable [Flood Research, Test & Evaluation Campaign workbook](../models/flood-research-test-evaluation.xlsx).
