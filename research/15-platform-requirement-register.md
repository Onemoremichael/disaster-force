# Platform and system requirement register

## Purpose

This register is the control point between mission research and vehicle design. It records which concepts are admitted for further analysis, which are held behind an unresolved comparison, and which are rejected. Admission is not approval to procure or render a platform.

The Department of Resilience should maintain this as a configuration-controlled technical record. Each program inherits the service-level target, design reference missions, mission thread, lifecycle and formation requirements in the earlier research.

## Status grammar

| Status | Meaning |
|---|---|
| Admitted | A persistent requirement exists; concept alternatives should be modeled |
| Conditional | Requirement may justify a unique system, but an alternatives or network test remains open |
| Held | Technically plausible but its strategic value or enabling regime is not yet established |
| Rejected | Violates the system architecture or does not solve the stated need |

Readiness for visualization uses a separate scale:

| Visualization state | Meaning |
|---|---|
| R0 — verbal | Mission and role only |
| R1 — functional | Major functions and interfaces identified |
| R2 — bounded | Capacity, access, endurance, staffing and environment have credible ranges |
| R3 — physics-closed | Mass, energy, flow, heat, structure, stability and lifecycle balances close |
| R4 — formation-closed | Crew, maintenance, connectors, bases, sustainment and rotation demonstrated |

Concept renderings begin at R3 and must show the complete operating system, not only a heroic exterior view. No concept in this pass is yet R3.

## Water, sanitation, power, and thermal safety

| ID | Concept | Status | Primary requirement | Current bound or discriminant | Critical unknown before R3 | State |
|---|---|---|---|---|---|---|
| W-1 | Point Water Cell | Admitted | Hours-scale safe water at isolated sites | pallet/trailer; source-flexible treatment; local quality verification | contaminant envelope, waste handling, operator burden | R1 |
| W-2 | Regional Water Works | Admitted | Community-scale production and storage | six-train WRG-50 reference; five online plus one contingency; up to 50,000 m³/day | guaranteed feed/output envelopes, setup rate, detailed equipment and consumables | R2 |
| W-3 | Strategic Water Works | Admitted | Sustained city/region supply | tens to hundreds of thousands m³/day by parallel trains | intake, concentrate, source seasonality, distribution loss | R2 |
| W-4 | Rapid Water Grid | Admitted | Move bulk water from source to point of use | 0.5 m pipe at 1.5 m/s is roughly 25,000 m³/day before losses | route, pressure zones, anchoring, joints, crossings, repair | R2 |
| W-5 | Wastewater and Residuals Works | Admitted | Prevent response-created sanitation and environmental failure | WRG-50 return-flow band 30,000–45,000 m³/day; seawater concentrate can equal product flow | influent/process variants, discharge authority, sludge and hazardous residuals | R2 |
| WRG-50 | Water Restoration Group 50 reference formation | Admitted reference | Deliver a complete temporary utility, not source production | default model: 50,000 m³/day; four pressure zones; 5,836 t pipe with reserve; 23,516 t preliminary deployment; 2,720 deployed personnel | surveyed transient model, vendor feed/hardware guarantees, installation trials, reliability/maintenance and degraded-mode demonstrations | R2+ |
| N-WEP | Nuclear Water–Energy Platform | Held | Long-duration coastal/island water and grid support | concept band 100–300 MWe net; 50,000–250,000 m³/day water | reactor choice, hull/stability, heat rejection, licensing, security, siting, crew, overhaul | R2 |
| P-1 | Critical Facility Power Cell | Admitted | Energize a bounded life-safety load within hours | 0.25–5 MW source/storage blocks plus survey, protection, connection, fuel, maintenance and transfer | standardized safe connection, sourced load profiles, equipment configuration and field reliability | R2 |
| P-2 | Community Grid Island | Admitted | Multi-building critical-load continuity | 5–25 MW islands with grid formation, load blocks, storage, medium-voltage distribution, control and synchronization | solved topology, short-circuit/transient studies, source portfolio, manual-safe operation and tests | R2 |
| P-3 | Regional Grid Bridge | Admitted | Substitute failed substations and key transmission/distribution nodes | 50–300+ MW mobile transformation, switching, reactive support, protection and intertie/source options | voltage-class portfolio, transport geometry, fault duty, protection, spares and field commissioning | R2 |
| P-4 | Rapid Distribution System | Admitted | Restore the last electrical mile | surface cable and overhead feeders with routes, poles/foundations, transformers, protection, grounding, crossings and service points | feeder quantities, conductor mass, installation productivity, electrical code path and hazard envelope | R2 |
| P-5 | Thermal and Clean-Air Works | Admitted | Safe occupied temperature and air during heat, cold and smoke | people-hour outcome and facility, neighborhood, district and movement strategies defined | climate/building loads, equipment, water/air distribution, storage, access and population behavior | R1+ |
| PRG-100 | Power Restoration Group 100 reference formation | Admitted reference | Deliver up to 100 MW net critical load as several safe utility islands or grid bridges | 17-sheet baseline: 103.89 MW gross dispatch; 140 MW owned source; 140 MW/140 MWh storage; 60 circuit-km bypass network; 18,332 t dry mass; 2,796 deployed people; 152,461 gal/day at 80% liquid share | sourced load archetypes, solved one-line, itemized equipment/connector manifest, protection/transients, verified construction rates, mobility, maintainability, workforce endurance, thermal demonstration and cost | R2+ |

## Fire, flood, access, and public works

| ID | Concept | Status | Primary requirement | Current bound or discriminant | Critical unknown before R3 | State |
|---|---|---|---|---|---|---|
| IIN | Ignition Intercept Network | Admitted reference | Place a verified effective intervention before a threatening ignition escapes | 23-sheet WUI cell screen: P50/P90 action 28.2/62.8 min; 81.2% modeled action before 50-min escape; 30.23 km/day effective line; 2,606 t dry mass; 1,393 deployed; generally negative closure margin in rapid cases | empirical correlated intercept distributions, regional ignition/consequence cases, false-alarm load, coverage, line productivity, availability and handoff under simultaneous demand | R2+ |
| IFCG | Integrated Fire Control Group | Admitted reference | Control an escaped fire or complex while protecting communities, responders and lifelines | WUI campaign screen: P50/P90 action 69.6/135.4 min; 798.28 effective sorties/day; 411.80 km/day effective line; +4.77 km/h closure margin; 42,339 t dry mass; 12,330 deployed / 46,237.5 billets; retardant binds and airspace is 94.8% utilized | calibrate growth, aircraft yield, airspace/base queues, robot production, hold/breach, public protection, item manifest, workforce, movement, concurrency, lifecycle cost and complete-thread test | R2+ |
| FA-1 | Persistent Fire Sentinel | Admitted | Find, map and coordinate fires through smoke and night | layered space/high-altitude/tactical/edge family measured by coverage-hours, probability, latency and uncertainty | sensor calibration, false alarms, obscuration, data fusion, weather, airspace and disconnected operation | R2 |
| FA-2 | Rapid Attack Aircraft | Admitted | High sortie rate in the first operational period | roughly 800–2,000 gallon exploration band; precision, alert time, austere basing and high-cycle availability over raw load | complete target cycle, low-altitude fatigue spectrum, agent/refill system, drop yield and ground hold | R2 |
| FA-3 | Regional Amphibious Suppressor | Admitted | Repeated attack near suitable water | roughly 2,000–4,000 gallon exploration band; source-to-target cycle rather than scoop rate | water geometry, weather/sea state, fatigue, corrosion, contamination transfer, agent mixing and alternate basing | R2 |
| FA-4 | Heavy Line Builder | Admitted | Build long controlled agent line for sustained campaign objectives | roughly 8,000–15,000 gallon exploration band; must compete with multiple smaller aircraft on delivered objective yield | runway/base throughput, drop geometry, fire interaction, fatigue, dispatch availability, maintenance and ground completion | R2 |
| FA-5 | Precision Lift and Suppression Rotorcraft | Admitted | Hover, lift, rescue and precision delivery | distinct suppression, lift and rescue configurations; optionally piloted variants are a research path | downwash, hot/high useful load, degraded-visual navigation, crew, maintenance, water cycle and rescue compatibility | R2 |
| FA-6 | Fire Aviation Base System | Admitted | Sustain predictable high sortie productivity | queue-bounded water/agent/fuel/traffic/maintenance/crew system with fixed and expeditionary configurations | service-time distributions, surge/fault behavior, water and fuel supply, pavement, environmental containment and workforce | R2 |
| FG-1 | Wildland Mobility Engine | Admitted | Protect crews and deliver water/agent in extreme terrain and heat | terrain and interface variants publish pump, mobility, survivability, refill and recovery envelopes | rollover, burnover, filtered crew environment, pump-and-roll, water logistics, repair and lifecycle availability | R2 |
| FG-2 | Autonomous Fireline Tractor | Admitted | Create and hold line in lethal conditions while displacing exposure | optionally crewed carrier/tool family with local safe stop, intermittent-comms behavior and machine-readable line quality | perception in smoke/dust, rollover, productivity distribution, safe separation, remote recovery, field repair and assurance | R2 |
| FG-3 | Long-Reach Water and Hose System | Admitted | Deliver surface water beyond conventional hose reach | source/intake/pump/relay/hose-or-pipe/storage/monitor formation with elevation and loss balance | route cases, pump curves, water/ecological compatibility, robotic placement, leaks, access, recovery and crew throughput | R2 |
| FG-4 | Structure and Ember Protection System | Admitted | Reduce cluster loss under ember, heat, flame and structure-to-structure exposure | rapid hardening, sensing, wetting/agent and incipient suppression measured by survival probability | exposure classes, water/energy demand, installation time/error, weathering, building diversity and neighborhood-scale validation | R2 |
| FIN | Flood Intercept Network | Admitted reference | Act before a location-specific water, access or structural threshold | 29-sheet configuration: 4/10 h P50/P90 action, 7 m³/s nominal portfolio, 1.76–3.59 m³/s effective across five cases after formation utilization; frequently acts before threshold but lacks positive day-zero hydraulic reversal; roughly 12,500–12,750 t dry | correlated action distributions, regional posture, alert/mobilized echelon split, local interfaces, rescue/search coupling, simultaneous watches, readiness and complete-thread field test | R2+ |
| HCG-100 | Hydraulic Control Group 100 reference formation | Admitted reference | Deliver complete regional water control, access and recovery | inland urban screen: 100 m³/s nominal becomes 36.551 m³/s effective, +16.051 m³/s day-zero removal, 28 d drawdown, −14.01 m³/s interior margin, 79,391 t dry and 7,039 deployed / 26,394 billets; Pass 15 assigns all twenty open gates to a $130B, 46-package experimental campaign and eight mission-thread trials | execute and independently accept calibrated hydrographs/action distributions; full pump/intake curves; route transients; receiving stage; barrier, interior drainage and breach trials; amphibious, environmental, item-manifest, workforce, readiness, lifecycle and complete-thread evidence | R2+ |
| FL-1 | Flood Intelligence Mesh | Admitted | Map evolving depth, velocity, contamination and failure risk | national forecast/gage/SAR base plus incident sensors, levee and drainage telemetry, autonomous bathymetry and uncertainty field | calibration, velocity/depth performance, latency, communications loss, debris damage, cyber, public warning and decision validation | R2 |
| FL-2 | Megaflow Pump Train | Admitted | Remove trapped water and control levels | four provisional classes from 0.1–0.5 m³/s high-head to 20–50 m³/s barge/closure stations; common electric drive and controls | full curves, head portfolio, cavitation, solids, intake, power, cooling, failure isolation, endurance, downstream effects and maintenance | R2 |
| FL-3 | Adaptive Barrier and Closure System | Admitted | Protect critical zones and close bounded openings | foundation/closure/interior-drainage system; 2 m ideal wall load 19.6 kN/m; 10 km conventional 2 m earth section screens at 180,000 m³ / roughly 360,000 t | load history, waves/current/debris, seepage, foundation, overtopping, terminations, installation, monitoring, removal and recovery | R2 |
| FL-4 | Breach and Control-Structure Works | Admitted | Stabilize levee, dam, canal and drainage failures | staged edge arrest, flow reduction, filter-compatible closure, armor and monitoring; 12 m × 3 m illustrative breach screens near 166 m³/s | breach growth and geotechnics, access, flow-control performance, material supply, filter/foundation, authority and failure consequence | R2 |
| FL-5 | Amphibious Rescue and Logistics Family | Admitted | Move people and priority cargo across distinct flood geometries | five separate shallow-urban, swiftwater, high-water land, heavy amphibious and coastal/surf classes with common sensing/patient/decon interfaces | stability, maneuver, wake, obstacles, entanglement, self-righting, patient/accessibility flow, road/rail transport, crew cycle and recovery | R2 |
| FL-6 | Rapid Drainage Spine | Admitted | Connect pump capacity to a lawful receiving water | large-bore surface trunk, channel, siphon, lift and crossing system; 100 m³/s requires about 64 one-metre or 16 two-metre lines at 2 m/s before reserve | route hydraulics, transient loads, mass, joints, anchors, crossings, robotic installation, leaks, contamination, setup and recovery | R2 |
| FL-7 | Hydraulic Works Carrier | Conditional | Deliver pumps, pipe, craft, heavy works, repair and command from waterways/coast | separate shallow-draft riverine modular carrier and seagoing coastal works ship; nuclear coastal variant held behind mission-energy comparison | payload/draft/lock/port/sea-state geometry, pump and pipe interfaces, cranes, power, stability, crew, maintenance, alternatives and cost | R1+ |
| EW-2 | Common Autonomous Work Machine | Admitted | High-tempo debris and earthwork with lower exposure | optionally crewed excavator/dozer/loader/hauler/dredge cores with wading, soft-ground, contamination, local-stop and recovery packages | standardized productivity, perception, tool change, ground pressure, protection, link loss, recovery, repair and lifecycle availability | R2 |
| EW-3 | Debris Processing Line | Admitted | Convert debris clearance into controlled material flow | survey, characterize, sort, reduce, recover, contain, load, sample, track and document; drainage and wet-debris interfaces explicit | waste distributions, hazardous fraction, water/sediment behavior, process equipment, site area, throughput, residuals and disposition | R1+ |
| EW-4 | Rapid Utility Corridor System | Admitted | Place pipe, cable, hose and access along damaged routes | drones survey/pull pilot; ground/heavy systems carry mass | jointing rate, crossings, trench/no-trench mix, testing and code approval | R1 |
| BR-1 | Immediate Crossing | Admitted | Hours-scale personnel/light vehicle access | light modular/temporary spans | bank prep, anchoring, current, inspection and load control | R1 |
| BR-2 | Heavy Modular Bridge | Admitted | Days-scale heavy logistics access | common load classes; reusable spans and foundations | approach works, launch system, geometry portfolio and fatigue | R1 |
| BR-3 | Accelerated Permanent Bridge | Admitted | Move from emergency to durable transport | prefabricated elements and standardized interfaces | code/site adaptation, foundation uncertainty, ownership and reuse | R1 |

## Maritime, air mobility, and health

| ID | Concept | Status | Primary requirement | Current bound or discriminant | Critical unknown before R3 | State |
|---|---|---|---|---|---|---|
| MR-1 | Littoral Access Craft | Admitted | Connect deep-draft ships to damaged shore and inland water | shallow draft; cargo/person/patient variants | payload-draft-speed trade, debris, sea state, propulsion and transport | R1 |
| MR-2 | Port-Opening Group | Admitted | Restore safe berth/channel/cargo flow | survey, salvage, tow, dive, temporary works, power and traffic system | equipment mix by port class, environmental limits, mobilization time | R1 |
| MR-3 | Resilience Support Carrier | Admitted | Sustain and repair distributed response forces without shore base | exploratory 20,000–60,000 tonnes payload/support; 15–30 days | hull count/size, module inventory, aviation/well access, crew, stability and cost | R2 |
| MR-4 | Modular Sealift and Sustainment Ship | Admitted | Carry recurring campaign mass and retrograde | self-discharge, Ro/Ro, cold/hazard/battery zones | sovereign fleet floor, commercial mix, port envelope and cycle time | R1 |
| MR-5 | Riverine/Inland-Waterway Group | Admitted | Work and distribute within flooded continental terrain | road/rail-deployable craft, barges, tows and shore systems | launch geometry, current/debris, locks, mooring, inter-basin transport | R1 |
| MH-1 | Littoral Stabilization Ship | Admitted | Hours-to-days coastal emergency and limited surgical care | small, high-readiness, multiple patient paths | staff model, bed/holding mix, aviation/craft interface and endurance | R1 |
| MH-2 | Regional Clinical Support Ship | Admitted | Weeks of specialty and chronic/acute support | modular acuity and specialty mix | clinical module geometry, infection zones, crew rotation, discharge path | R1 |
| MH-3 | Strategic Health-Support Platform | Admitted | Regional workforce, specialty, laboratory and health logistics hub | hospital capacity expands only with staffing and pathway | common-hull value, health manufacturing, accreditation and lifecycle | R1 |
| AM-1 | Strategic Mission-Module Airlift | Admitted requirement | Assured first-entry movement | own fleet/configuration floor; airframe source open | load/network model, fleet availability, basing and outsized need | R1 |
| AM-2 | Short-Field Disaster Airlifter | Conditional | Frequent theater cycles to degraded 900–1,500 m fields | medium payload, self-loading, high-cycle and field-maintainable | advantage over runway repair/existing aircraft, payload-range and cost | R2 |
| AM-3 | Vertical Access Family | Admitted | Patient, team, sensor, repair and priority-cargo access | separate medical, external-load and urban variants with common cores | payload/range, weather, noise/downwash, energy and fleet support | R1 |
| AM-4 | Airborne Command/Sensing/Relay | Admitted | Restore coverage and observation over wide damaged areas | evaluate coverage-hours rather than aircraft count | altitude mix, spectrum, backhaul, weather and persistence | R1 |
| AM-5 | Airfield-Opening Group | Admitted | Make aircraft throughput possible | survey, repair, lighting, traffic, fuel, handling and onward movement | package sizes by field class, certification, fuel and traffic capacity | R1 |
| HM-1 | Community Health Continuity Team | Admitted | Maintain primary/chronic/public-health functions | neighborhood/mobile multidisciplinary teams | population caseload, medication/oxygen chain and local integration | R1 |
| HM-2 | Mobile Acute-Care Unit | Admitted | Stabilize, diagnose, observe and prepare movement | staffed treatment positions with full clinical utilities | treatment rate, acuity mix, staffing, oxygen and evacuation queue | R1 |
| HM-3 | Modular Theater Hospital | Admitted | Flexible staffed inpatient and specialty capacity | independent blocks around common utility/logistics spine | bed/acuity demand curves, workforce rotations, infection and discharge | R1 |
| HM-4 | Patient Movement System | Admitted | Complete appropriate origin-to-destination journeys | ground, water and air modes plus command/records | receiving-bed visibility, accessible mix, escort staff and route loss | R1 |
| HM-5 | Health Logistics/Workforce Group | Admitted | Sustain clinicians, supplies, quality and replacement rotations | credentialing, oxygen, blood, pharmacy, maintenance and staff support | staffing pipeline, cold chain, stock rotation, quality governance | R1 |

## Information, observation, robotics, and sustainment

| ID | Concept | Status | Primary requirement | Current bound or discriminant | Critical unknown before R3 | State |
|---|---|---|---|---|---|---|
| C-1 | Responder Mesh Kit | Admitted | Local life-safety voice/data/location in isolation | human/vehicle scale; offline operation | spectrum/interoperability portfolio, battery and usability | R1 |
| C-2 | Incident Network Node | Admitted | Rapid local broadband, compute and gateways | road/air/boat-mobile; federated nodes | coverage/capacity bands, spectrum rights, power and backhaul | R1 |
| C-3 | Airborne Coverage/Relay | Admitted | Area communications when towers/backhaul fail | aerostat/rotor/fixed/high-altitude product line | weather and airspace availability, link budget and support system | R1 |
| C-4 | Strategic Backhaul/Emergency Cloud | Admitted | Diverse national connectivity and sovereign computation | multi-provider, regional edge and disconnected environment | capacity reservation, cyber boundary, identity and data governance | R1 |
| C-5 | Public Continuity Package | Admitted | Accessible warnings, charging, connectivity and public services | neighborhood and institutional nodes | population use, language/accessibility, privacy and device scarcity | R1 |
| O-1 | Rapid Damage/Service Survey | Admitted | Versioned population-service-time picture | multi-source observation with confidence and age | validation, sampling bias, owner data and field workflow | R1 |
| O-2 | Infrastructure Dependency Graph | Admitted | Predict cascades and target restoration | planning fidelity, not universal real-time replica | data access, model validation, security and regional maintenance | R1 |
| O-3 | Resilience Space Layer | Conditional | Fill unique revisit, sensing or communications gaps | mixed federal/commercial/allied/hosted/small-satellite architecture | gap analysis, orbital/ground resilience, lifecycle and duplication | R1 |
| O-4 | Mission Decision Environment | Admitted | Show demand, uncertainty, alternatives and downstream effects | advisory optimization with accountable human decision | explainability, data age, rights, allocation rules and validation | R1 |
| R-1 | Aerial Survey/Light Delivery | Admitted | Distributed sensing and urgent small payloads | standardized mission bays and safe loss-of-link | weather, airspace, batteries, fleet maintenance and recovery | R1 |
| R-2 | Heavy Cargo Shuttle | Conditional | Repeat priority movement over broken routes | corridor- and payload-tier specific | whole-cycle productivity, energy, landing nodes, weather and safety | R1 |
| R-3 | Hazardous Earthwork/Fireline Robot | Admitted | Reduce exposure in destructive work | optionally crewed, local stop and manual operation | perception, communications loss, productivity and recovery | R1 |
| R-4 | Utility Inspection/Repair Robot | Admitted | Find and address faults in confined/damaged systems | aerial/ground/surface/underwater variants | manipulation limits, certification, access and fleet proliferation | R1 |
| R-5 | Depot/Distribution Automation | Admitted | Improve readiness, inventory and loading | controlled-environment first | common item identity, offline/manual mode and cyber safety | R1 |
| R-6 | Clinical/Community Robotics | Conditional | Materials, telepresence, mobility and bounded clinical support | no autonomous care or rights decisions | evidence of clinical/workforce value, privacy and infection control | R1 |

## Rejected architectures

| Architecture | Reason for rejection |
|---|---|
| One universal disaster ship | Concentrates availability and combines conflicting draft, aviation, clinical, nuclear, cargo and port-opening requirements |
| Converted legacy platform as default acquisition model | Imports another mission's structure, fatigue, flow, maintenance and support compromises |
| Tank capacity as fire-aircraft performance | Ignores cycle time, accuracy, availability, ground hold and objective completion |
| Nominal beds as medical capacity | Ignores staffing, acuity, utilities, infection control, referral, evacuation and discharge |
| Drone logistics as a massless substitute | Conceals payload, energy, handling, weather, maintenance and recovery burdens |
| Production at source as delivered service | Omits connection, route, distribution, quality and point-of-use availability |
| Proprietary cloud as a critical control dependency | Fails the disconnected and sovereign-sustainment requirement |
| Armor and combat systems by default | Consume civil payload without solving the dominant environmental and infrastructure threats |

## Gate-to-rendering work queue

The first rendering candidates are selected only after quantitative modeling and configuration-level physics closure. Pass 7 makes the water configuration auditable at R2+; Pass 10 does the same for the power formation; Pass 12 makes the fire-force configuration auditable at R2+; Pass 14 makes the integrated flood-force configuration auditable at R2+. None is verified hardware or field performance, and no concept is yet authorized for rendering. Priority is determined by research value, not spectacle.

1. **Rapid Water Grid and Regional Water Works:** replace provisional equipment and rates with source/vendor evidence, surveyed transients, installation trials, reliability, maintenance and degraded-mode demonstrations.
2. **PRG-100 deployable electric utility:** close reuse, bypass and rebuild cases across load, one-line, sources, storage, transformation, protection, distribution, fuel, thermal effect, workforce and deployment.
3. **Ignition Intercept Network and Integrated Fire Control Group:** replace the configuration workbook's highest-leverage assumptions with empirical distributions and subsystem evidence, beginning with tail intercept, mixed-airspace capacity, retardant/agent throughput, robotic line productivity and hold/breach; no FA-2/3/4 or ground-system drawing precedes R3 closure.
4. **Resilience Support Carrier group:** close module inventory, connectors, aviation, workshops, replenishment, crew, availability and alternative hull counts.
5. **Littoral and regional medical groups:** close patient demand, clinical flow, transfer, staff rotation, utility and discharge balances.
6. **FIN and HCG-100:** execute the Pass 15 `ARPA-R` / independent `RTEA` campaign: 46 preregistered packages across ten purpose-built range families, rival prototype cohorts and eight escalating mission threads. Correlated action tails, full-curve pump/intake availability, drainage-spine mass/setup/transients, dedicated interior drainage, live-flow breach reduction and amphibious operating envelopes remain first priorities; no pump, craft, barrier, robot or works-carrier drawing precedes R3 closure.
7. **Nuclear Water–Energy Platform:** proceed only after non-nuclear alternatives, siting/licensing system, heat and mass balance, lifecycle workforce and shore distribution are modeled.

The visualization brief for each concept must include cutaways or operating diagrams showing connectors, payload flow, crew, power, waste, maintenance and surrounding formation. Exterior beauty views alone would repeat the platform-first error this research is designed to avoid.
