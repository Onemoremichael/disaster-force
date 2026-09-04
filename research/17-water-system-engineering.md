# Water restoration force engineering

## Purpose and finding

This pass asks what the Department of Resilience must own if it promises to restore safe water as an assured public service rather than deliver bottles, loan a purifier, or count production at a plant fence. It closes a reference architecture for the **Regional Water Works** (`W-2`) and **Rapid Water Grid** (`W-4`) far enough to define the machinery, formations, interfaces, and remaining tests.

The central finding is that the operational unit is a **deployable utility**, not a treatment plant. The Department needs a family of Water Restoration Groups able to survey sources and damaged networks, produce water, establish pressure-zoned conveyance, buffer output, certify quality, connect critical facilities and neighborhoods, control wastewater and residuals, repair what they install, and transfer service to a lawful local operator.

No single national machine should be specified as “the water asset.” Source chemistry, topography, access, surviving networks, discharge constraints, climate, and duration create distinct configurations. The Department should standardize the interfaces and force modules while retaining multiple treatment and conveyance sets.

## Correction to Pass 4

Pass 4 overstated ideal pumping power by approximately a factor of ten. A 0.5-meter internal-diameter line flowing at 1.5 meters per second carries about 0.295 m³/s. Raising that flow through **100 meters of total dynamic head** at 75-percent efficiency requires:

\[
P = \frac{\rho g Q H}{\eta}
  = \frac{(1{,}000)(9.81)(0.295)(100)}{0.75}
  \approx 0.385\ \text{MW},
\]

not 4 MW. That idealized number excludes line friction. For 100 kilometers of 0.5-meter pipe at the same velocity and an assumed Darcy friction factor of 0.015, friction head is about 344 meters. With 100 meters of static lift, total head is approximately 444 meters and shaft power is approximately **1.71 MW**. The strategic conclusion survives but becomes more precise: water production energy can dominate in seawater reverse osmosis, while route length, diameter, elevation, pressure segmentation, and network condition determine whether delivery is feasible.

This is a design-study correction, not a construction specification. Friction factor, minor losses, surge, temperature, pipe class, elevation profile, pump curve, and operating reserve must be resolved for each route.

## The delivered-service requirement

Water demand must be stated at point of use and by service phase. For one million supported people:

| Service condition | Liters/person/day | Delivered volume/day | Operational meaning |
|---|---:|---:|---|
| Immediate household floor | 3.8 | 3,800 m³ | drinking, limited cooking and hygiene; CDC household planning floor of one gallon |
| Emergency public-health target | 15 | 15,000 m³ | survival service with constrained hygiene |
| Stabilized basic service | 20 | 20,000 m³ | drinking, cooking, food hygiene, hand and face washing; other hygiene remains constrained |
| Expanded community service | 50 | 50,000 m³ | on-plot or near-plot service with materially improved hygiene, but below normal U.S. utility consumption |

The World Health Organization notes that volume collected is strongly related to distance and collection time: an arithmetically sufficient supply can still fail as a public-health service if users cannot reach it or queues consume the day.[^who-quantity] EPA emergency guidance likewise requires planners to consider the existing network partly usable or completely unusable and to assess distribution, storage, transport, operators, power, and security—not only source quantity.[^epa-edws]

The Department should therefore report four quantities separately:

1. **certified production** leaving treatment;
2. **bulk delivery** reaching a pressure zone or storage node;
3. **accessible delivery** available at a functioning building connection, institutional connection, local loop, or staffed public point; and
4. **safely used volume**, estimated through metering, quality surveillance, queue/access sampling, and loss accounting.

Only the third and fourth are response outcomes.

## Complete system boundary

A deployable water utility has nine inseparable functions:

`assess demand → qualify source → treat → certify → convey → buffer → distribute → manage return flows → transfer`

| Function | Required elements | Failure if omitted |
|---|---|---|
| Demand and network assessment | population-service-time map, critical facilities, pressure-zone map, contamination isolation, outage forecast | production is sent to the wrong place or into an unsafe network |
| Source qualification | hydrology, intake survey, contaminant screen, source protection, seasonal yield, water rights/authority | treatment train cannot handle the actual feed or depletes/contaminates a source |
| Treatment | intake, pretreatment, core process, disinfection, finishing, chemical systems, clean-in-place | unreliable output, membrane/media failure, or unsafe product |
| Independent quality authority | field and regional laboratories, sampling plan, chain of custody, release authority, public advisory | “purified” water is distributed without potability assurance |
| Bulk conveyance | pipe/hose, pumps, valves, surge control, crossings, anchors, telemetry, repair bypass | plant output accumulates while users remain dry |
| Buffering | raw and product storage, break tanks, pressure control, reserve inventory | treatment and demand fluctuations propagate into outages or unsafe pressure |
| Point-of-use distribution | repaired utility sectors, critical-load manifolds, neighborhood loops, tanker and container fill, accessible public points | bulk water exists but households and institutions cannot use it |
| Return-flow control | sewer bypass, temporary sanitation, wastewater treatment, concentrate/backwash/CIP residual management | the response creates a sanitation or environmental emergency |
| Transfer and demobilization | as-builts, asset condition, operator training, spares, water-quality history, removal or conversion plan | an unmaintainable temporary network becomes a second failure |

Army and Marine Corps water doctrine independently reaches the same systems conclusion: water support includes treatment, storage, distribution, and issue, and production commonly exceeds organic storage and transport capacity.[^atp-water] The Department’s civil system must go further by closing household access, wastewater, regulatory transfer, and months-long operation.

## Reference formation: WRG-50

The **Water Restoration Group 50** (`WRG-50`) is a sizing reference, not a frozen platform. It is designed to deliver up to 50,000 m³/day of expanded community service or the same volume divided among larger populations at lower emergency service levels.

### Reference mission

- support up to 1 million people at 50 L/person/day, 2.5 million at 20 L/person/day, or a mixed portfolio of residents, hospitals, shelters, food systems, and essential industry;
- qualify and begin using a viable local source within 72 hours when reception and civil authority permit;
- establish 50 kilometers of trunk conveyance over a reference 50-meter net rise while local and point-water systems bridge the gap;
- operate for at least 180 days with scheduled rotations and replenishment;
- function with the host distribution system absent, partly usable, or isolated into safe sectors; and
- transfer an enduring configuration or remove a temporary one without interrupting service.

### Modular organization

| Module | Reference composition | Primary effect |
|---|---|---|
| Utility command and civil integration | technical authority, operations center, utility liaison, legal/environmental, public information | one accountable water service plan |
| Source and network reconnaissance squadron | hydrogeology, intake survey, damage isolation, geospatial/hydraulic modeling, unmanned survey | validated source/route/network options |
| Treatment regiment | six nominal 10,000 m³/day trains, five online plus one maintenance/contingency train | 50,000 m³/day certified output after demonstrated source derating |
| Quality and public-health regiment | mobile laboratories, field sampling teams, epidemiology and advisory cell | independent release and continuing surveillance |
| Conveyance regiment | two nominal 0.5-meter-ID trunks or equivalent; booster, valve, crossing and repair companies | 50,000 m³/day over the reference route |
| Storage and distribution regiment | raw/product/break storage, district nodes, critical-facility connectors, tanker/package interfaces | accessible point-of-use service |
| Sanitation and residuals regiment | sewer bypass, modular wastewater, concentrate/residual containment and discharge monitoring | safe return-flow path |
| Utility support regiment | power, maintenance, spares, heavy handling, chemicals, fuel, camp and internal communications | sustained availability and repair |

Six treatment trains do not imply six identical membrane boxes. The common product interface is certified water at defined flow, pressure, chemistry, and telemetry. Upstream trains are selected from fresh surface water, brackish groundwater, seawater, high-turbidity floodwater, and specialized-contaminant configurations. A source outside a validated train’s contaminant envelope is a no-go condition, not an invitation to improvise.

## Source and treatment architecture

### Source hierarchy

The Group should select the least complex safe source that closes the mission:

1. isolate, disinfect, power, and repair a surviving local utility;
2. interconnect to an adjacent operating utility;
3. develop protected groundwater or bank filtration;
4. treat fresh surface water;
5. treat brackish water;
6. desalinate seawater; or
7. import packaged or bulk water as a temporary bridge.

This hierarchy is not a rule that seawater systems deploy last. It prevents the institution from spending high energy and residual-management capacity while a safer, closer, lower-complexity source is available.

### Treatment balance

At a design value of 4 kWh/m³ for seawater reverse osmosis, 50,000 m³/day of product requires about 200 MWh/day, or 8.3 MW average, for the RO process reference before route pumping and site auxiliaries.[^doe-bandwidth] A 50-percent-recovery reference train also requires about 100,000 m³/day of feed and creates about 50,000 m³/day of concentrate before other residuals. Intake, pretreatment, post-treatment, clean-in-place systems, product stabilization, and discharge remain part of the plant.

Fresh and brackish sources can require much less process energy but may impose difficult turbidity, biological, salinity, industrial-chemical, fuel, or wildfire-ash loads. The procurement specification should use a source test matrix and guaranteed net output under named feed envelopes. Nameplate output on ideal feed is not accepted capacity.

### Quality release

Treatment operators do not unilaterally certify their own product. A separate quality authority owns:

- source baseline and process-control sampling;
- microbial, disinfectant-residual, turbidity, conductivity and selected chemical testing;
- unknown-contaminant escalation and laboratory referral;
- sanitary inspection of tanks, hoses, fittings, tankers and public points;
- release, restriction, boil-water/do-not-use and return-to-service decisions;
- geolocated sample records and chain of custody; and
- building and sector flushing before reconnection.

EPA’s contamination-response guidance treats distribution pipes and storage as sampling locations, while current military doctrine requires continuing residual monitoring through storage and distribution.[^epa-sampling][^atp-water] Potability is a continuing system state, not a certificate issued once at the plant.

## Conveyance physics

### Diameter, velocity, and mass

The preliminary model uses Darcy–Weisbach, water density of 1,000 kg/m³, 75-percent pump efficiency, and a friction-factor design band rather than a single false-precision value. The table below uses `f = 0.015`, 100 km, 100 m static lift, 1.0 or 1.5 m/s, and an illustrative PE pipe with internal diameter as shown, dimension ratio 17, and material density of 950 kg/m³. Pipe mass excludes fittings, valves, couplings, anchors, crossings, pumps, packing, damage allowance, and handling equipment.

| Internal diameter | Velocity | Flow/day | Friction head, 100 km | Total head | Pump power | Approx. pipe mass, 100 km |
|---:|---:|---:|---:|---:|---:|---:|
| 0.30 m | 1.0 m/s | 6,107 m³ | 255 m | 355 m | 0.33 MW | 1,910 t |
| 0.30 m | 1.5 m/s | 9,161 m³ | 573 m | 673 m | 0.93 MW | 1,910 t |
| 0.50 m | 1.0 m/s | 16,965 m³ | 153 m | 253 m | 0.65 MW | 5,306 t |
| 0.50 m | 1.5 m/s | 25,447 m³ | 344 m | 444 m | 1.71 MW | 5,306 t |
| 0.75 m | 1.0 m/s | 38,170 m³ | 102 m | 202 m | 1.17 MW | 11,938 t |
| 0.75 m | 1.5 m/s | 57,256 m³ | 229 m | 329 m | 2.85 MW | 11,938 t |
| 1.00 m | 1.0 m/s | 67,858 m³ | 76 m | 176 m | 1.81 MW | 21,223 t |
| 1.00 m | 1.5 m/s | 101,788 m³ | 172 m | 272 m | 4.19 MW | 21,223 t |

Larger pipe trades lift and material mass for lower friction and higher capacity. The correct design cannot be selected from flow alone; it minimizes time to accessible service subject to route, pressure, transport, joining, repair, reuse, energy, and lifecycle constraints.

The Plastics Pipe Institute handbook treats sustained pressure, surge, temperature, hydraulic design, burial, and thermal movement as interacting design problems.[^ppi-design] Its field guidance requires trained operators, maintained fusion equipment, controlled joining force, and cooling time; jointing is therefore a production line and quality process, not a trivial field connection.[^ppi-field]

### WRG-50 reference route

The reference route uses two parallel 0.5-meter internal-diameter trunks, each carrying approximately 25,000 m³/day over 50 km with a 50-meter net rise. At about 1.47 m/s and a Darcy friction-factor band of 0.012–0.020:

- friction head is approximately 132–220 meters per line;
- total dynamic head is approximately 182–270 meters before minor-loss and surge allowances;
- combined average hydraulic power is approximately 1.4–2.1 MW; and
- the two lines contain approximately 5,300 tonnes of illustrative DR-17 PE pipe before fittings and reserve.

The route is divided into hydraulic reaches with break tanks or controlled booster stations. A single pump cannot simply impose the whole head on a long temporary line: normal pressure, low-point static pressure, surge, temperature derating, fitting class, anchor load, air/vacuum behavior, and failure consequence all constrain reach length. The route survey must produce an elevation and pressure envelope before pipe class and station placement are released.

Two lines provide isolation and repair flexibility but are not full redundancy at peak output. Losing one line cuts trunk capacity roughly in half. Full `N+1` conveyance would require a third line, a larger alternate route, or intentional service curtailment. The reference formation accepts degraded service during a line outage and carries sectional isolation and bypass material.

### Why drones do not lay the trunk

Five thousand tonnes of pipe for the reference route, plus pumping, crossings, anchoring, storage, and fittings, establishes the boundary. Aerial systems can map the alignment, detect washouts, pull pilot cords, deliver sensors and small fittings, inspect joints, and localize leaks. Ground, rail, barge, or heavy-lift systems must move the trunk mass. Optionally crewed route-clearance, trenching, pipe-handling, fusion, anchoring, and recovery machines are the high-value autonomy investment.

## Deployment and construction system

The Department should acquire a **pipeline factory that moves**, divided into parallel work fronts:

1. route survey and civil-access authorization;
2. clearance, grading, matting, trench or protected surface preparation;
3. pipe and fitting shuttle from railhead, port, or staging yard;
4. controlled fusion or mechanical joining with serialized joint records;
5. crossing, anchor, valve, air-release and drain construction;
6. booster/break-tank installation and power connection;
7. cleaning, pressure test, disinfection, quality release, and commissioning; and
8. patrol, leak repair, security, weather protection, and eventual recovery.

No national installation-rate promise is justified yet. Route productivity must be tested across flat road shoulder, dense urban corridor, rubble, river crossing, steep grade, frozen ground, wildfire exposure, and inundated terrain. The force should carry at least three construction modes:

- **surface rapid:** fastest, accessible for inspection and recovery, vulnerable to traffic, heat, vandalism, fire, flotation and impact;
- **shallow protected:** slower, using trench, berm, mat, barrier, culvert and protected crossing; and
- **enduring:** code-compliant buried or structurally protected installation suitable for transfer.

The same line should not be promised as both an hours-scale temporary asset and an unattended multi-decade utility without an explicit conversion plan.

## Storage and last-mile service

At 50,000 m³/day, twelve hours of product buffer is 25,000 m³ and 25,000 tonnes. Even an ideal 2.5-meter-deep reservoir requires 10,000 m² of water surface before berms, separation, access, treatment protection, and secondary containment. Storage is therefore a site and civil-works problem.

The Group should use divided storage rather than one reservoir:

- treatment clearwell and contact storage;
- pressure-zone break tanks;
- district reserves near hospitals, shelters and population clusters;
- tanker and packaged-water fill nodes; and
- isolated contingency reserves that survive one contamination or rupture event.

EPA lists stationary emergency bladders in the 10,000–100,000 gallon range, transportable bladders up to 6,000 gallons, and tanker trucks in the 3,000–20,000 gallon range.[^epa-edws] Those are useful interfaces, but they reveal the scale mismatch: 50,000 m³/day is more than 13 million U.S. gallons per day. Tankers and household containers cannot be the primary metropolitan trunk.

### Distribution hierarchy

1. isolate, flush, sample, and pressurize safe surviving utility sectors;
2. connect hospitals, dialysis, cooling centers, shelters, food facilities, and public-health sites directly;
3. install district loops and neighborhood service islands where the buried network is unusable;
4. use tanker delivery for isolated institutions and dispersed users; and
5. use packaged water for the first hours, mobile populations, and sites where containers or sanitation make bulk issue unsafe.

Every public point requires accessible approach, drainage, lighting, communications, security, containers or container policy, queue control, flow metering, residual checks, and a plan for people unable to travel. A distribution node is a staffed public-service site, not a row of taps.

## Wastewater, sanitation, and residuals

Water supply and wastewater are a single operational promise. The planning model should assume that 60–90 percent of delivered community water can return as wastewater unless use restrictions, decentralized sanitation, irrigation, evaporation, or collection failure demonstrate otherwise. At the WRG-50 ceiling, that is a design band of **30,000–45,000 m³/day** of return flow.

The sanitation plan chooses among:

- repair and power of surviving lift stations and treatment works;
- sectional sewer isolation and temporary bypass pumping;
- decentralized toilets and contained collection;
- modular treatment near district service nodes;
- controlled discharge under public-health and environmental authority; and
- sludge, screenings, hazardous residual, membrane-cleaning waste, and concentrate transport or treatment.

Seawater desalination adds a distinct high-volume concentrate stream. A 50-percent-recovery reference makes approximately one cubic meter of concentrate for each cubic meter of product. It cannot be blended into a damaged sewer by assumption. Intake and discharge geometry, salinity, temperature, chemicals, receiving-water conditions, monitoring, and permit/emergency authority belong in the receiving-site design.

## Personnel and force generation

The WRG-50 personnel model remains a bounded hypothesis pending time-and-motion exercises. A deployed Group likely requires approximately **2,300–3,200 people** when operating continuously across multiple work fronts:

| Workforce block | Deployed planning band | Major occupations |
|---|---:|---|
| Command, planning and civil integration | 120–180 | utility incident management, engineering authority, legal/environmental, liaison, public information |
| Source, network and route assessment | 150–250 | hydrogeologists, hydraulic modelers, surveyors, GIS, inspectors, unmanned-system crews |
| Treatment and quality | 350–500 | operators, process engineers, chemists, microbiologists, samplers, public-health staff |
| Conveyance construction and operations | 650–850 | heavy equipment, pipe handling/fusion, pump/valve, crossing, electrical, civil and patrol crews |
| Storage and distribution | 400–550 | tank/reservoir, critical-facility connection, district-node, tanker/package and accessibility teams |
| Sanitation and residuals | 300–450 | wastewater operators, bypass crews, industrial hygiene, residual transport and monitoring |
| Maintenance, logistics, power and internal support | 330–420 | mechanics, electricians, controls, warehouse, transport, fuel/chemical, communications, medical and camp support |

Twenty-four-hour operation means positions, not people, must be converted into shifts, relief, leave, illness reserve, training, and rotation. A sovereign force capable of sustaining one deployed WRG-50 while retaining a ready replacement and resetting a returned group could require roughly three personnel/equipment echelons, shared schools and depots, and an industrial/operator reserve. The final multiplier must come from an exercised force-generation cycle, not an analogy.

Professional authority matters. Water-quality release, pressure-system commissioning, electrical energization, confined-space work, hazardous residual handling, and transfer to a public utility require named accountable qualifications. Autonomy may reduce exposure and repetitive labor, but it does not erase technical authority.

## Deployment sequence and lift

The force arrives as layered effects rather than waiting for the full trunk:

| Time from employment decision | Intended water effect | Primary modules |
|---|---|---|
| 0–24 hours | demand/source reconnaissance; protect or isolate local assets; immediate packaged/point supply | command advance party, survey, W-1 cells, quality teams, utility repair liaison |
| 24–72 hours | critical-facility and shelter water; first local treatment; district storage | source/intake, early treatment trains, tanker and bladder nodes, power, sewer bypass |
| Days 3–10 | parallel treatment and first trunk reaches; safe surviving sectors re-pressurized | main treatment, pipeline work fronts, booster/break tanks, district connections |
| Days 7–21 | reference regional output and accessible distribution, route permitting | complete conveyance, storage/distribution, sanitation/residual systems, replacement shifts |
| Weeks 3–26 | reliability, network repair, enduring conversion and civil transfer | depot support, capital repair, operator training, as-builts, spares and demobilization |

The reference trunk alone is approximately 5,300 tonnes of pipe. With treatment trains, pumps, storage, construction machinery, fittings, spares, power, laboratories, sanitation systems, vehicles and support, the full group is plausibly a **five-figure-tonnage deployment**. That inference is deliberately broad until packaging and equipment schedules are modeled. The main body is a rail, sealift, barge and heavy-road force. Airlift is reserved for reconnaissance, command, quality, critical spares, point systems, and the earliest treatment capability.

## Failure and degraded modes

The acquisition program must demonstrate safe behavior for at least these cases:

- source quality shifts outside the active train envelope;
- one treatment train unavailable;
- one trunk isolated or ruptured;
- power loss at treatment or a booster station;
- pressure excursion, air lock, vacuum, surge, or anchor failure;
- suspected contamination after release;
- telemetry and positioning unavailable;
- road, bridge, railhead, port, or crossing loss;
- freezing, extreme heat, flood, wildfire, salt spray, debris impact, and deliberate damage;
- wastewater acceptance lost while potable production continues; and
- local operator unable or unwilling to accept transfer.

The safe state may be lower output, isolated district service, manual operation, tanker bridge, or public restriction. It is not uncontrolled continuation.

## Acquisition programs that follow

The first-principles requirement produces a portfolio, not a hero vehicle:

1. **Source and Network Survey System** — sampling, hydraulic/network mapping, geophysics, intake survey, aerial/ground/surface robotics, and field decision support.
2. **Treatment Train Family** — common product, power, chemical, data and maintenance interfaces across source-specific process variants.
3. **Mobile Water Laboratory Family** — field release laboratories, regional confirmatory laboratories, sample logistics, and independent quality command.
4. **Rapid Trunk System** — flexible and semi-rigid pipe classes, valves, manifolds, bypasses, anchors, road/rail/river crossings, and recovery kits.
5. **Autonomous Utility Works Family** — route clearance, trenching, pipe handling, fusion assistance, joint inspection, leak localization, and hazardous repair.
6. **Booster and Pressure-Zone System** — pump modules, break tanks, surge control, power, protection, telemetry and manual controls.
7. **Deployable Storage Family** — raw, contact, product, district and contingency reservoirs with sanitary protection and rapid civil works.
8. **Community Water Interface** — critical-facility connectors, district loops, accessible public points, tanker/package nodes, metering and communications.
9. **Wastewater and Residuals Works** — sewer bypass, modular treatment, sanitation, sludge/residual handling and concentrate monitoring.
10. **Water Utility Support System** — chemicals, membranes/media, clean-in-place, repair stock, calibration, workshops, power and operator sustainment.

Lockheed-Martin-scale industrial ambition belongs here: high-rate pipe and fitting capacity, standardized treatment cores, autonomous construction machinery, mobile laboratories, pumps and drives, controls that survive disconnection, national depots, exercised reserve production lines, and a professional integration authority. The industrial product is assured utility restoration, not just equipment sales.

## Technical-gate decision

| Record | Decision after Pass 6 | Reason |
|---|---|---|
| `WRG-50` reference architecture | **R2+, not R3** | mass, flow, approximate energy, treatment redundancy, storage, return flow and formation bands now close at concept level; pressure class, minor losses/surge, detailed route, source train, installation rate, equipment schedule and transport packaging do not |
| `W-2` Regional Water Works family | **Remain R2** | common functional architecture is credible, but source-specific treatment trains need guaranteed feed/output/consumable envelopes |
| `W-4` Rapid Water Grid family | **Remain R2** | hydraulic reference closes, but pressure-zoned hardware, crossings, joining productivity, recovery, and tested setup rates remain open |
| `W-5` Wastewater and Residuals Works | **Advance R1 to R2** | return-flow and desalination-residual scale are bounded; process variants and discharge cases remain open |
| `N-WEP` Nuclear Water–Energy Platform | **Remain held at R2** | abundant production power does not close source, shore manifold, trunk mass, pressure zones, wastewater, receiving site, licensing, security, crew, or alternative comparison |

No water platform is authorized for concept rendering yet. The next gate is a configuration-level engineering model of the WRG-50: route profiles, pump and pressure-zone schedule, treatment/feed cases, storage site plan, equipment and lift manifest, construction productivity, crew positions, maintenance/spares, and three degraded-mode demonstrations. The eventual first rendering must show the **whole utility formation**—source works, treatment, laboratory, pipeline factory, booster nodes, storage, district interfaces, sanitation, support, and people—not a futuristic desalination box.

## Research implications

1. The Department’s water service should be organized as a standing utility profession with construction, operations, quality, public-health, logistics, and civil-transfer authorities inside one deployable command.
2. Metropolitan-scale emergency water is primarily a network-restoration and temporary-infrastructure campaign. Packaged water and tankers are bridges and edge tools.
3. Large pipe reduces energy but increases industrial mass, route footprint, joining burden, and transport dependence. Multiple diameters and construction modes are required.
4. Seawater desalination is technically powerful near coastlines but produces an equally serious intake, concentrate, and shore-distribution problem.
5. Nuclear power may add endurance and simultaneous grid support, but does not make the water system mobile by itself. The shore works remain the controlling design.
6. The highest-value autonomy is in surveying, construction, inspection, and hazardous repair. The high-throughput main remains a heavy civil-engineering system.
7. The mature industrial base must be able to manufacture, stock, inspect, mobilize, repair, recover, and replenish complete utility formations at concurrency scale.

[^who-quantity]: World Health Organization, [*Guidelines for Drinking-water Quality: Fourth Edition Incorporating the First and Second Addenda*](https://iris.who.int/bitstream/handle/10665/352532/9789240045064-eng.pdf), 2022, pp. 86–88; see also [*How Much Water Is Needed in Emergencies*](https://www.who.int/docs/default-source/wash-documents/wash-in-emergencies/technical-notes-on-wash-in-emergencies/who-tn-09-how-much-water-is-needed.pdf).
[^epa-edws]: U.S. Environmental Protection Agency, [*Planning for an Emergency Drinking Water Supply*](https://www.epa.gov/sites/default/files/2015-03/documents/planning_for_an_emergency_drinking_water_supply.pdf), EPA 600-R-11-054, June 2011, pp. 18–22.
[^atp-water]: U.S. Army and U.S. Marine Corps, [*ATP 4-44/MCRP 3-40D.14, Water Support Operations*](https://rdl.train.army.mil/catalog-ws/view/100.ATSC/26F5F885-EE29-4461-A569-E226165D10CA-1443796247417/ATP_4_44wc2.pdf), Change 2, September 16, 2025, paras. 1-1–1-23.
[^doe-bandwidth]: U.S. Department of Energy, [*Bandwidth Study on Energy Use and Potential Energy Savings Opportunities in U.S. Seawater Desalination Systems*](https://www.energy.gov/sites/default/files/2017/12/f46/Seawater_desalination_bandwidth_study_2017.pdf), 2017.
[^epa-sampling]: U.S. Environmental Protection Agency, [*Module 3: Site Characterization and Sampling Guide for Drinking Water Utilities*](https://www.epa.gov/waterutilityresponse/module-3-site-characterization-and-sampling-guide-drinking-water-utilities), updated May 18, 2026.
[^ppi-design]: Plastics Pipe Institute, [*Handbook of PE Pipe*, Chapter 6: Design of PE Piping Systems](https://www.plasticpipe.org/common/Uploaded%20files/Technical/PPI%20PEHandbook2022.pdf), 2022 edition.
[^ppi-field]: Plastics Pipe Institute, [*Polyethylene Piping Systems Field Manual for Municipal Water Applications*](https://www.plasticpipe.org/common/Uploaded%20files/1-PPI/Manuals-Design%20Guides/Polyethylene%20Piping%20Systems%20Field%20Manual%20for%20Municipal%20Water%20Applications/mid-pe-field-manual-municipal-water-applications.pdf), pp. 35–39.
