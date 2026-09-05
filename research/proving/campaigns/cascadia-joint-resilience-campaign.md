# The Cascadia Joint Resilience Campaign

## Designing a national force to restore public service across a broken region

### Research state

`R2 campaign architecture` · `R2+ deterministic arithmetic` · all throughput, restoration, cost, workforce and technology coefficients remain evidence gates · no platform rendering authorized

## Executive judgment

A magnitude-9 Cascadia rupture should not be treated as one large incident with a larger incident-management organization. It should be treated as a **joint public-service campaign across nine temporarily disconnected theaters**. The earthquake, tsunami, liquefaction, landslides, bridge failures, port obstruction, utility loss, aftershocks and workforce disruption would fracture the Pacific Northwest into service islands whose surviving assets could not be assumed to reach one another.

This distinction changes the force. A force designed around intact interstate highways, usable deepwater ports, commercial lodging, grid power and a functioning regional fuel market will become another claimant on a damaged society. A force designed around the Cascadia campaign must instead carry or prepare the missing system: independent origins, entry nodes, no-pier and shallow-draft access, route-opening formations, self-contained responder bases, local water production, grid-forming power, public communications, clinical systems, recurring supply, hazardous reverse flow, personnel relief and return to readiness.

Pass 24 found that the national deployment enterprise could close all ten reference campaigns under its declared base assumptions, but that a correlated primary-path loss reduced the Cascadia and allied coastal-megacity chains to `0.765×`. More long-range lift did not repair the failure. Reception, responder support and sustainment failed together.

This study replaces that aggregate screen with an item-level Cascadia campaign. The linked [Cascadia campaign model](../../../models/cascadia-campaign-model.xlsx) resolves:

- nine service islands;
- eight safe-zone or afloat origin complexes;
- eleven entry-node classes;
- twelve deployment and distribution paths in eleven correlation groups;
- sixty-four mission-package load records with mass, volume, handling, hazard, mode, origin, destination, public effect and deadline;
- four formation waves totaling exactly 1,762,600 tonnes;
- eleven public-service families at days 3, 14, 45 and 90;
- a 90-day sustainment campaign peaking at 22,520.4 tonnes per day;
- protected patient movement, responder relief and hazardous reverse flow;
- responder-base independence and a 180-day reconstitution screen;
- twelve technology requirements and twenty evidence gates; and
- an attributable regional capital program of $373.44 billion, including reserve, plus $34.2 billion in mature annual operations.

Under the selected correlated-aftershock-and-winter design case, all sixty-four loads meet their deadlines, all forty-four service tests close, every service island has at least five independently failing path groups available by day 14, all responder-base milestones close, and sustainment, reverse flow, patient movement, staff rotation and the modeled reconstitution promise reconcile. That result is a **requirements demonstration**, not a prediction. It shows one internally consistent force architecture that could satisfy the declared public promise if its coefficients were real. Twenty open evidence gates state why the nation is not yet entitled to believe they are.

The campaign reveals four governing principles.

First, **geographic separation must precede mobilization**. Damaged metropolitan airports and ports are destinations, not origins. The force begins from interior and afloat complexes outside the principal correlated failure.

Second, **the first 72 hours are primarily a prepositioning and theater-opening problem**. The model's 88,130-tonne minimum viable service wave cannot be improvised after rupture. Its distributed cache path must make 112,651 handling-equivalent tonnes accessible by day 2, while the south-air bridge must provide at least 18,730 gross handling-equivalent tonnes per day under the declared node and deployment factors to place a 650 MW power starter by day 3.

Third, **bulk lift is not public service**. A load receives credit only when it reaches its service island on time and completes an effect family that also has sustainment and responder support. Every path, module and authority therefore sits in the same closure logic.

Fourth, **a mature force is an industrial system rather than an inventory**. The Cascadia posture implies prepared complexes, purpose-built aircraft and craft, bridge and runway systems, depots, caches, schools, ranges, data infrastructure, public authorities and a permanent regional workforce. The dramatic vehicle is only one element of that system.

## 1. The scenario is a topology, not a point estimate

The campaign does not claim to forecast the next rupture. The U.S. Geological Survey's Cascadia magnitude-9 scenario catalog provides thirty realizations and recommends the median ensemble for general planning; the distribution matters because rupture direction, shaking, deformation and local ground response alter which links survive.[^usgs-scenario] The USGS's 2025 regional fact sheet places the 50-year probability of a magnitude-9 Cascadia event at roughly 10–15 percent and describes the January 1700 event as approximately magnitude 8.7–9.2.[^usgs-2025] Those are hazard statements, not load plans.

The operational baseline comes from official state planning and exercise evidence. Cascadia Rising 2022 used a 700-mile rupture and four to six minutes of shaking, treated aftershocks as a continuing problem, and identified limited east-west corridors, bridge vulnerability, unresolved maritime and rail planning, uncertain fuel demand and incomplete mass-care standards.[^cr22] The Washington transportation resilience assessment describes a system in which surface transport may be unusable, air is insufficient for bulk movement, ports are exposed to liquefaction and tsunami, shallow-draft access may precede full dredging, and crane or channel obstruction can persist far longer than the life-safety window.[^wa-rrap]

The Oregon Resilience Plan is equally sobering. Its baseline anticipates months to years of service restoration in affected areas, extensive coastal highway failure, hundreds of landslide and instability locations, the likely loss of multiple coastal airports, Redmond as a principal response airport, and severe fuel-terminal and distribution exposure.[^orp] The plan is older than this study and is not an asset-level forecast. Its value is structural: coast, valley and interior do not fail or recover as one network.

The workbook uses legacy population and movement anchors from a 2011 federal analytical draft—2.4 million people requiring food and water support, 933,000 requiring emergency shelter, 27,000 initial injuries and about 119,000 people in a patient-movement planning pool.[^hitrac] These values are intentionally labeled as old and provisional. They should be replaced by current, privacy-protecting population, facility, mobility, dependency and daytime/nighttime distributions before operational use.

The model therefore treats the scenario as a **failure topology**:

```text
rupture and tsunami
    ↓
shared failure of roads, bridges, ports, grids, fuel, communications and labor access
    ↓
nine service islands with different hazards and surviving interfaces
    ↓
independent safe-zone origins and entry paths
    ↓
time-bounded restoration of public services
```

The topology is more important than false precision about a single damage total. It determines whether nominal alternatives are actually independent.

## 2. The object is a joint public-service campaign

### 2.1 The campaign promise

Military deployment doctrine provides a useful discipline: force closure occurs when the required force reaches its destination with enough resources and readiness to perform the mission, not when cargo leaves an origin.[^jp401] The Department of Resilience changes the purpose from combat power to public service but retains the systems logic.

For service island `z`, service family `s` and milestone `t`, campaign closure is:

```text
closure(z,s,t)
  = min(
      lawful civil task,
      complete service module,
      safe origin availability,
      independent path availability,
      entry and handling capacity,
      last-mile access,
      responder-base capacity,
      recurring sustainment,
      technical release,
      public-service effect
    )
```

No term can be averaged away. Excess communications capacity cannot substitute for unsafe drinking water. A hospital package without oxygen, sterile supply, wastewater, power, staff lodging, referral and patient movement does not close health service. A desalination plant without distribution closes no household service. A bridge system without surveyed abutments, traffic control and a release authority does not reopen a route.

The force is assessed against four public promises:

| Wave | Deadline | Required formation mass | Public promise |
| --- | ---: | ---: | --- |
| `R1` | Day 3 | 88,130 t | Minimum viable service: command, communications, urgent access, clinical stabilization, first water, food, shelter, sanitation and power effects |
| `R2` | Day 14 | 317,268 t | Initial operating capability: multimodal entry, major public-service islands, responder bases and recurring supply |
| `R3` | Day 45 | 828,422 t | Complete operating formation: heavy access, utilities, care, housing, distribution, maintenance and command depth |
| `R4` | Day 90 | 528,780 t | Replacement, redundancy, reserve stocks, second routes and endurance |

The sixty-four modeled lots are not a procurement manifest. They are the minimum accounting objects needed to prevent the model from treating mass as homogeneous. Each record carries a service module, cargo lot, target zone, origin, assigned and alternate path, admissible modes, package count, mass, volume, TEU equivalent, handling penalty, cold-chain, hazardous-material and outsized flags, public effect, readiness date and latest useful arrival.

### 2.2 Nine service islands

The command map divides the campaign into nine planning zones:

| Zone | Service island | Dominant isolation | Day-14 path promise |
| --- | --- | --- | ---: |
| `Z1` | Puget North | bridge, ferry and port interfaces | at least 3 independent groups |
| `Z2` | Puget Central | urban bridges, liquefaction and fuel hub | at least 5 |
| `Z3` | Puget South | interstate, port and crossing loss | at least 4 |
| `Z4` | Southwest Washington | Columbia crossings and coast corridors | at least 3 |
| `Z5` | Oregon North Coast | US 101 bridges, tsunami and slopes | at least 3 |
| `Z6` | Oregon Central Coast | US 101, mountain routes and airfield survival | at least 3 |
| `Z7` | Oregon South Coast | single corridors, tsunami and long distance | at least 3 |
| `Z8` | Willamette Valley | liquefaction, bridges, fuel and utility loss | at least 4 |
| `Z9` | Eastern safe zone | surge population and mountain transfer | at least 3 |

These are command and service-accounting zones, not claims that every community within them has the same condition. The campaign command should be able to subdivide them as evidence arrives. What matters is that no metropolitan headquarters can silently assume control of resources that cannot physically cross a broken corridor.

Each service island receives a joint resilience task force with one public-service ledger, one movement-control cell and one civil authority interface. The regional campaign commander allocates scarce national effects among them but cannot erase state, tribal, local, territorial or invited-host authority. Independent medical, infrastructure, environmental, aviation, maritime, nuclear, data and worker-safety authorities retain release powers.

### 2.3 The command structure

The Department should maintain a standing **Cascadia Joint Resilience Campaign Command** rather than assemble a temporary interagency committee after rupture. Its peacetime role is to own the regional campaign design, maintain agreements, conduct exercises, audit preparedness and translate new hazard or infrastructure evidence into force requirements.

Its wartime-equivalent structure has five echelons:

1. **National Resilience Operations Center** allocates scarce forces among concurrent national and global campaigns.
2. **Cascadia Joint Resilience Campaign Command** owns regional priorities, independent-path design, force flow and public-service outcomes.
3. **North, Central, South and Afloat Support Commands** operate safe-zone origins, strategic entry and the regional distribution lattice.
4. **Nine Service-Island Commands** integrate land, air, maritime, utility, health and community formations around local public effects.
5. **District Service Groups** deliver and transfer water, power, care, shelter, sanitation, communications, access and community services.

This is deliberately larger than incident coordination. It is a permanent operational institution with trained commanders, logisticians, engineers, clinicians, utility operators, public administrators, labor and community specialists, contracting officers, environmental scientists, safety authorities and data stewards.

## 3. Origins must survive the theater they support

The campaign uses eight origin complexes: Spokane–Fairchild, Yakima–Tri-Cities, Redmond–Bend, Klamath Falls–Medford, a Boise–Twin Falls relay, a northern California sea-and-air complex, and north- and south-Pacific offshore groups. These are analytical candidates, not siting decisions.

Each origin must satisfy six independence tests:

- outside the principal severe-shaking, tsunami, liquefaction or landslide mechanism it supports;
- independent water, power, sanitation, communications and fuel endurance;
- workforce access that does not depend on the damaged metropolitan network;
- at least one paired origin with a different hazard and transport correlation group;
- capacity to receive national flow, assemble service modules, shelter personnel and repair equipment; and
- lawful, exercised access to onward air, road, rail, inland-water or maritime routes.

The safe zone is not merely a warehouse. It is a force-generation base. It must provide crew rest, family support, maintenance, decontamination, medical care, metrology, configuration control, waste handling, replacement stock, public information and the ability to absorb displaced people without losing its own operation.

This is why the model distinguishes origin hubs from entry nodes. Paine Field, Joint Base Lewis–McChord, Portland-area airfields, damaged ports and valley terminals may become valuable receiving nodes. They are not treated as sources of unaffected fuel, labor, lodging or utility service.

## 4. Build eleven independent path groups, not one efficient pipeline

The campaign uses twelve named paths in eleven correlation groups:

| Path | Mode | Stress opening | Stress capacity structure | Strategic role |
| --- | --- | ---: | --- | --- |
| `P0` distributed upland caches | cached | Day 0 | 40,000 handling-t/day; 125,000 finite stock | day-3 formation core |
| `P1` Spokane heavy-air bridge | air | Day 1 | 15,000 then 20,000/day | Washington urgent and medium-weight modules |
| `P2` Redmond–Klamath heavy-air bridge | air | Day 1 | 19,000 then 22,000/day | Oregon and valley urgent modules |
| `P3` distributed vertical-lift network | vertical | Day 0 | 14,000 then 18,000/day | isolated landing lattice and patient transfer |
| `P4` Puget no-pier bridge | littoral | Day 3 | 16,000 then 24,000/day | ferry, beach and damaged-terminal access |
| `P5` Oregon no-pier bridge | littoral | Day 3 | 22,000 then 30,000/day | three dispersed coastal sectors |
| `P6` recovered Puget deepwater | ocean | Day 8 | 20,000 then 40,000/day | heavy formation closure after survey and release |
| `P7` Columbia–Willamette shallow draft | inland water | Day 6 | 18,000 then 28,000/day | valley and southwest bulk flow before full port recovery |
| `P8` Washington east–west surface | road | Day 7 | 16,000 then 32,000/day | route-opening and inland distribution |
| `P9` Oregon east–west surface | road | Day 6 | 15,000 then 28,000/day | multiple mountain-corridor packages |
| `P10` interior-to-valley rail | rail | Day 14 | 16,000 then 38,000/day | late bulk and reconstitution flow |
| `P11` offshore support shuttle | ocean support | Day 2 | 14,000 then 22,000/day | repair, utility, clinical and base modules |

Capacities are handling-equivalent tonnes rather than payload mass. A tonne requiring cold chain, hazardous separation, unusual lift, slow rigging, scarce cranes or controlled transfer consumes more of the node than a tonne of compatible palletized cargo. The model computes each load's effective burden as the maximum of mass, volume, TEU-handling and outsized terms multiplied by its handling factor.

Every daily path capacity is then reduced by opening state, node condition, correlated aftershock days and winter windows before being partitioned among deployment, sustainment and hazardous reverse flow. Capacity reserved for recurring food, fuel, medical supply or waste cannot be quietly reassigned to clear a formation backlog.

This representation produces a key threshold. The south-air path carries a 13,787.9 handling-tonne grid-forming power starter. To dispatch it on day 1 and deliver it by day 3, the path needs at least:

```text
required gross handling capacity
  = 13,787.9 / (0.92 destination-node factor × 0.80 deployment share)
  = 18,733.6 handling-equivalent tonnes/day
```

The modeled requirement is rounded to 19,000. An 18,000-tonne/day assumption delivers the power starter on day 4 and fails the entire day-3 public promise. This is the appropriate use of a deterministic design model: not to claim that 19,000 is known, but to reveal the full-mission performance that research, fleet sizing, node design and exercises must prove.

### 4.1 No-pier is a primary mode

The coast cannot wait for conventional port restoration. Washington planning evidence notes that shallow-draft operations may precede dredging and that fixed port obstructions may persist; Oregon planning assumes extensive coastal route and airport loss.[^wa-rrap][^orp] The mature force therefore treats no-pier littoral and shallow-draft inland-water operations as primary modes, not salvage auxiliaries.

Current military systems establish lower bounds, not solutions. The Army Engineer Research and Development Center has demonstrated a lightweight modular causeway that can assemble a 120-foot span in roughly three hours with seven people and support a 40-ton fire vehicle, while military bridging provides other wet-gap precedents.[^lmcs][^irb] Navy logistics-over-the-shore programs demonstrate that ship-to-shore transfer is a real system family.[^lots] None of those facts validates sustained civil traffic, winter sea states, tsunami debris, accessibility, hazardous cargo, public queuing or the modeled 8,000–16,000-plus tonne mission threads.

The Department needs complete no-pier groups: hydrography, debris and obstruction removal, autonomous and crewed shallow craft, modular causeways, beach and ferry-interface structures, cranes, roll-on/roll-off surfaces, traffic control, environmental monitoring, security, public access, maintenance, crew support and alternate landing sectors.

### 4.2 Surface restoration is a network operation

The land force cannot promise to “reopen I-5” as a single project. It must create a lattice of certified corridors, temporary spans, bypasses, slopes, culverts, pavement, traffic control, rail interfaces and last-mile routes. Federal Highway Administration experience with self-propelled modular transporters shows that prefabricated bridge elements can compress construction time where sites and interfaces are prepared.[^spmt] The campaign requirement extends that principle to pre-surveyed abutments, modular foundations, mixed public traffic and repeated aftershock inspection.

Route status must be evidence, not rumor. An autonomous reconnaissance swarm may collect geometry, imagery and instrument data, but a human public authority retains release. The relevant output is not kilometers surveyed; it is safe, load-classified, continuously monitored access connected to an operating destination.

## 5. Close services, not commodities

The model has eleven service families: civil command, end-to-end access, responder basing, potable and essential water, food and nutrition, emergency shelter, sanitation, critical-load power, priority communications, staffed health capacity and hazard-control works.

Each milestone has a public effect target. Day 3, for example, requires command coverage across nine service islands, 25,000 tonnes/day of enabled access, bases for 25,000 responders, 18,000 m³/day of water, food service for 2.4 million people, refuge support for 450,000 people, sanitation for 450,000 users, 500 MW of critical power, communications for 2.4 million users, 500 staffed care beds and 100 route-equivalent kilometers/day of hazard-control work.

The quantities are planning requirements, not established need. Their analytical importance lies in their non-fungibility and completeness. A service row activates only when its associated load arrives. Its final closure ratio is the minimum of material effect, campaign sustainment and responder-base capacity. The same method carries through days 14, 45 and 90.

This creates several practical disciplines:

- bottled water does not substitute for a functioning high-volume water system beyond the survival interval;
- power generation receives no service credit without isolation, grid formation, transformation, protection and distribution;
- nominal beds receive no credit without staff, oxygen, sterile supply, water, wastewater, diagnostics, referral and patient movement;
- shelter must include accessibility, thermal safety, hygiene, safeguarding and transition rather than tent count;
- communications must reach residents and public-service workers, not only headquarters; and
- route opening includes inspection, debris, crossing, traffic, geotechnical and public-release functions.

## 6. The force must not consume the society it is saving

The campaign deploys up to 108,110 people. In a damaged region, that population can overwhelm surviving hotels, water systems, sanitation, clinics, food distribution and fuel. Responder support is therefore an operational effect and a moral obligation.

The model uses nine base systems across interior fixed sites, afloat groups, upland deployable campuses and mobile bridge bases. Effective stress capacity reaches 97,920 people by day 3 and 150,720 by day 45. The capacity exceeds the deployed force at each milestone, but every coefficient remains unproved.

A **zero-host-utility responder base** must provide, for ninety days:

- weatherized and accessible lodging;
- drinking water, hygiene and wastewater treatment;
- food, cold chain and kitchens;
- grid-forming power, backup, thermal safety and fuel or alternative energy;
- occupational and primary health, behavioral health and infection control;
- communications, records and family contact;
- rest cycles, quiet space, safeguarding and labor protections;
- maintenance, decontamination, waste segregation and hazardous reverse flow; and
- a measured handoff or removal plan.

The model's requirement is 5,000 people per deployable module at full winter occupancy without host utilities. This is not a camp-design detail. It is the difference between a force that restores public capacity and one that displaces survivors from it.

## 7. Sustainment is the campaign's center of gravity

The ninety-day daily supply bill rises from roughly 15,996 tonnes during initial operations to a peak of 22,520.4 tonnes per day as the full formation deploys. It includes force support, food, limited imported water, fuel and process consumables, medical and cold-chain material, repair stock, shelter and sanitation supply, utility chemicals and general stores.

The imported-water line is intentionally small. Moving enough bottled water for 2.4 million people would dominate the movement system and still fail wastewater and distribution. The force must instead produce, treat, test, store and distribute water locally from qualified seawater, surface-water, groundwater and surviving utility sources. Strategic lift carries membranes, pumps, pipe, storage, laboratories, chemicals and repair stock—not a permanent ocean of bottles.

Daily capacity is protected by mode. Local survival-supply reserves can release up to 20,000 tonnes per day from an 80,000-tonne stock during the opening interval. Air, maritime, inland-water, surface and rail paths then take over recurring demand. The selected stress case produces a small transient backlog during the modeled aftershock sequence but returns to full cumulative fill and zero day-90 backlog.

The campaign should be judged on its worst service island, not regional aggregate supply. The next model must disaggregate recurring demand and inventory by zone, temperature, hazard class, shelf life, maintenance class and substitution rule. It must also model forecast error, lost loads, damaged stock, queue discipline, private-market recovery and the point at which public procurement begins to crowd out local access.

## 8. Reverse flow, people flow and force regeneration are first-class missions

Inbound logistics creates outbound obligations. The campaign reserves capacity for medical waste, contaminated material, treatment residuals, damaged batteries and controlled debris. The modeled demand reaches 1,840 tonnes per day while protected reverse capacity remains above it. The movement ledger requires a licensed receiving destination; moving material away from the service island without lawful acceptance is not closure.

People move on protected passenger capacity rather than on fictional unused cargo tonnes. The model screens the 119,000-person patient movement pool through day 30 and a thirty-day responder relief rhythm through day 90. Both clear under the declared seats. Clinical prioritization, family unity, accessibility, consent, receiving-facility capacity and continuity of records remain open.

Finally, the Department must remain able to answer the next catastrophe. The 180-day reconstitution screen returns, decontaminates, inspects and inducts the `R1` and `R2` equipment mass by day 120 after a thirty-day release lag. The screen is deliberately incomplete: real regeneration must include exhausted people, family recovery, clinical stock, software state, calibration, contaminated equipment, repair parts, depot queues and concurrent campaign demand.

## 9. Technology programs revealed by the campaign

The campaign does not assume that today's equipment defines tomorrow's force. It uses current systems as lower bounds and states the inventions needed to close the public promise.

| Program | Full-mission threshold before force credit |
| --- | --- |
| Distributed strategic-to-austere cargo aircraft | 40–80 t payload into 600–1,200 m repaired runway; three-hour ground cycle; 100-sortie representative campaign with at least 85% completion |
| Aftershock-tolerant runway regeneration | Restore a 1,200 m × 30 m strip in 12 hours; re-certify within 30 minutes after a trigger event |
| No-pier littoral throughput | 8,000–16,000 handling-equivalent t/day per group for 30 days in representative protected-water winter conditions |
| Robotic port hydrography and clearance | Survey and release one shallow path in 24 hours; remove 10,000 t of obstruction within seven days |
| Long-span civil emergency bridge train | 80 m gap, 80 t gross vehicle, 1,500 vehicles/day and 72-hour opening from first load |
| Autonomous route-certification support | 500 route-km/day per group in a seeded-damage blind trial, with human public release |
| Zero-host-utility responder base | 5,000 people per module for 90 winter days at full occupancy |
| Damage-tolerant movement ledger | Offline custody, priority, hazard and substitution state for 500,000 loads during a 72-hour disconnected exercise |
| Hazardous reverse-flow system | 1,800 t/day segregated, tracked and accepted by licensed destinations by day 14 |
| Shallow-draft inland distribution flotilla | 20,000 handling-equivalent t/day across temporary terminals under debris, sediment and failed-terminal conditions |
| Rapid public utility corridor | 100 km/day of mixed temporary feeder and pipe corridor after route release, tested under live load and pressure |
| Reconstitution depot and digital twin | Return, decontaminate, inspect and release `R1/R2` formations by day 120 after a full campaign |

Current aircraft illustrate why system throughput cannot be read from brochure payload. The Air Force lists the C-17 at a maximum payload of about 170,900 pounds and the C-130 family near 42,000 pounds depending on configuration.[^c17][^c130] Campaign output also depends on runway length and strength, fuel, weather, maintenance, crews, cargo handling, destination capacity, cycle time and completion probability. The novel requirement may be satisfied by new aircraft, distributed conventional fleets, autonomous cargo systems, prepared runways or a different modal allocation. The Department should fund rival pathways until evidence discriminates among them.

Technology credit requires a representative mission thread, not a component demonstration. The no-pier trial must include actual mixed cargo, public traffic, debris, environmental limits, maintenance and responder support. The runway trial must include drainage, lighting, foreign-object control, load classification and repeated aftershock release. The utility-corridor trial must carry live electrical load and hydraulic pressure across real crossings. The autonomy trial must measure missed hazards and false releases, not just average inspection speed.

This is how a resilience establishment drives innovation: it creates demanding public missions, stable long-term procurement, competing technical approaches, national ranges, independent measurement, production transition and a visible path from failed trial to improved design.

## 10. The regional industrial program

The modeled Cascadia program is an attributable slice of the Pass 24 deployment enterprise and the Pass 23 Department envelope. It must not be added again to those totals.

| Capital line | Illustrative quantity | Unit hypothesis | Extended |
| --- | ---: | ---: | ---: |
| Prepared Resilience Entry Complexes | 8 | $6.0B | $48.0B |
| Distributed upland cache and auxiliary sites | 24 | $1.2B | $28.8B |
| Interior strategic-air complexes | 4 | $5.5B | $22.0B |
| No-pier littoral groups | 8 | $2.4B | $19.2B |
| Shallow-draft flotillas | 6 | $2.0B | $12.0B |
| Port-clearance and dredge groups | 8 | $2.5B | $20.0B |
| Land route-opening groups | 12 | $2.1B | $25.2B |
| Modular heavy-bridge systems | 24 | $0.6B | $14.4B |
| Offshore responder bases | 6 | $5.8B | $34.8B |
| Distributed cargo aircraft | 24 | $0.9B | $21.6B |
| Vertical-lift logistics craft | 48 | $0.3B | $14.4B |
| Autonomous runway-repair trains | 10 | $0.6B | $6.0B |
| Zero-host-utility base packages | 8 | $1.5B | $12.0B |
| Deployment data and communications | 1 program | $6.0B | $6.0B |
| Research, proving and independent test | 1 program | $24.0B | $24.0B |
| Depots, initial spares and stock depth | 1 program | $15.0B | $15.0B |
| **Subtotal** |  |  | **$311.2B** |
| **Explicit 20% program reserve** |  |  | **$62.24B** |
| **Attributable envelope** |  |  | **$373.44B** |

The twenty-five-year profile begins with design, prototypes, sites and independent test; rises through network construction and production; sustains a national fielding plateau; then shifts toward depth, recapitalization and transition. It is a program-development shape, not a schedule estimate.

The mature annual operating hypothesis is $34.2 billion: $9.9B for roughly 45,000 loaded regional billet-equivalents, $8.0B for fleet operations and maintenance, $4.0B for prepared-site operations and access, $3.0B for stock rotation and consumables, $2.5B for full-mission exercises, $1.5B for continuous research and test, $0.8B for access agreements, $2.0B for operational deployment allowance and $2.5B for depots, spares and reconstitution. Reconstruction payments and broad disaster assistance are excluded.

This program would create a new industrial geography. Pacific Northwest shipyards, ports, aircraft and drone firms, heavy-civil contractors, utilities, tribal enterprises, laboratories, health systems, manufacturers, unions and technical colleges would form one production-and-readiness network. Ordinary-time output would include bridge modules, mobile substations, treatment trains, causeways, cranes, sensors, communications, medical systems, public works and skilled workers that can also serve domestic infrastructure and export markets.

The industrial policy must avoid a single prime contractor becoming the architecture. Government owns the public-service requirements, interfaces, safety cases, reference data and test results. Competing firms own products and production know-how. Open physical and data interfaces permit one supplier's failure to be replaced without invalidating the entire force.

## 11. Authority is throughput

Every major movement or service action requires a lawful and technical release. The workbook therefore tracks nine authority chains: public priorities and allocation, airfield release, port and waterway release, potable-water release, electrical energization, clinical opening, hazardous reverse flow, autonomous action and reconstitution release.

Each chain separates four roles:

- the **operational owner**, who needs the effect;
- the **independent authority**, who may release or refuse it;
- the **host civil authority**, who sets public priorities and acceptable conditions; and
- the **public ledger**, which records evidence, limits, uncertainty and the next review.

Urgency cannot allow the campaign commander to self-certify a bridge, energize an unsafe network, discharge treatment residuals, open a clinical service without infection control or deploy autonomous heavy equipment without a bounded action class. Conversely, authority cannot remain a serial paperwork queue disconnected from operations. Inspectors, laboratories, legal powers, data systems and public communication deploy with the formation.

## 12. What the model proves—and what it does not

The workbook proves six limited things:

1. the 1,762,600-tonne formation mass reconciles across four waves and sixty-four records;
2. the declared path capacities can clear those handling-equivalent loads by their deadlines;
3. the declared service-effect packages can close the forty-four milestone targets;
4. the eleven correlation groups can give every zone at least the required day-14 path diversity;
5. the declared bases, supply, reverse flow, passenger movement and depot capacity can close the campaign logic; and
6. the capital and annual profiles reconcile to their stated envelopes.

It does not prove that the hazard quantities are current, the loads are complete, the paths will open, the capacities are physically achievable, the public-effect coefficients are causal, the workforce exists, the authorities will act, the costs are reliable, or the force will perform under surprise and fatigue.

The twenty evidence gates include scenario and demand validation; independent path covariance; air, no-pier, port, inland-water, road and rail throughput; responder-base independence; water, power, health and shelter effects; sustainment and reverse flow; hazardous-material control; patient and staff movement; reconstitution; capital and operating cost; and the rendering gate.

The campaign architecture should be falsified in this order:

1. update the population, infrastructure and hazard baseline;
2. build asset- and route-level covariance maps with utility and labor dependencies;
3. create item manifests for `R1` and `R2`, including packaged dimensions and maintenance stock;
4. run discrete-event movement, weather, aftershock, failure and repair simulations;
5. design representative responder-base, no-pier, airfield and utility-corridor prototypes;
6. execute multi-week trials in which one primary path and one host utility fail together;
7. measure public service rather than equipment activity;
8. obtain independent cost, schedule, workforce and industrial-base estimates; and
9. repeat the method against an unfamiliar global campaign to identify assumptions hidden by U.S. infrastructure and authority.

### Pass 26 assurance finding

The linked [Cascadia network covariance and assurance study](cascadia-network-covariance-and-assurance.md) completes the first item on that continuation path. It replaces nominal correlation-group counting with a fixed-seed stochastic screen across path copies, system and mode-family shocks, and five shared enablers: fuel and energy, communications, qualified workforce, civil and technical authority, and repair/inspection.

Under its declared assumptions, this paper's reference architecture closes only 5.8 percent of trials. Hardening without topological change reaches 21.4 percent; two separately supported copies reach 48.0 percent; and a three-cell campaign mesh reaches 84.2 percent. None meets the 95-percent design-assurance target. These are not forecast probabilities. They supersede only the inference that deterministic closure and named correlation groups were enough to demonstrate path independence.

The revised design rule is that an independent path must carry an independent origin, enabler package, workforce, repair chain, technical release and civil interface. The remainder of this paper remains the authoritative Pass 25 load, service and campaign baseline.

## 13. Implications for the Department of Resilience

Cascadia makes the Department more ambitious, not more centralized. It requires a cabinet institution capable of national force generation while distributing operational authority to service islands and preserving independent release.

The mature structure needs:

- a Strategic Mobility Command that owns end-to-end force closure rather than transportation alone;
- a standing Cascadia campaign command with permanent regional plans and exercises;
- air, maritime, land, infrastructure, health and community services that generate complete formations;
- a Responder Base Command with equal standing to movement commands;
- a national cache, depot, repair and reconstitution enterprise;
- a civil authority that owns priorities, rights, accessibility, public explanation and transfer;
- technical authorities with deployable laboratories and inspectors;
- a National Resilience Proving Network able to test whole mission threads destructively; and
- an industrial mobilization organization that maintains multiple suppliers, workforce pipelines and surge capacity.

This is not FEMA with a larger equipment account. It is a sovereign operational institution whose purpose is to project life-support systems through broken geography. It can support existing state, tribal, local and international authorities precisely because it arrives with coherent force, measured capacity and an explicit command relationship rather than a collection of grants, contracts and borrowed platforms.

## Conclusion

The first-principles Cascadia force is not a hospital ship, a fleet of cargo aircraft or an earthquake corps. It is a permanent national system that can create public service across a region whose own connective tissue has failed.

Its defining assets are prepared safe-zone origins; distributed caches; independent air, vertical, littoral, ocean, inland-water, road and rail paths; complete service modules; zero-host-utility bases; recurring supply and reverse flow; public and technical authority; and a reconstitution system. Purpose-built vehicles follow from those requirements. They do not lead them.

The model's clean closure is therefore not the conclusion. The conclusion is the research program it exposes. A coequal Department of Resilience would spend decades turning the yellow assumption cells into national evidence: building prototypes, breaking them, operating them through winter and aftershocks, measuring whether people actually regain water, power, care, access and agency, and sustaining enough industrial depth to do it again.

Only after that configuration evidence exists should the project render the machines.

[^usgs-scenario]: U.S. Geological Survey, [Cascadia M9 scenario catalog](https://earthquake.usgs.gov/scenarios/catalog/cszm9/).
[^usgs-2025]: U.S. Geological Survey, [Earthquake Probabilities and Hazards in the U.S. Pacific Northwest](https://pubs.usgs.gov/publication/fs20253050/full), 2025.
[^cr22]: Washington Emergency Management Division, [Cascadia Rising 2022 After-Action Report and Improvement Plan](https://mil.wa.gov/asset/64dce2b7dec3b/FINAL%20-%20Revised%20CR22%20AAR-IP%20%20071823%20Signed.pdf), 2023.
[^wa-rrap]: Washington Emergency Management Division and U.S. Department of Homeland Security, [Washington State Transportation Systems Regional Resiliency Assessment Program](https://mil.wa.gov/asset/5d8ba2a03a1b7), 2019.
[^orp]: Oregon Seismic Safety Policy Advisory Commission, [The Oregon Resilience Plan](https://www.oregon.gov/lcd/NH/Documents/Apx_9.2.3_OR_Res_Plan_Final_OPT.pdf), 2013.
[^hitrac]: U.S. Department of Homeland Security HITRAC/NISAC, [Analytical Baseline Study for the Cascadia Earthquake and Tsunami, draft](https://www.co.wahkiakum.wa.us/DocumentCenter/View/185/Draft-Analytical-Baseline-Study-for-the-Cascadia-Earthquake-and-Tsunami---September-12-2011-PDF), 2011. Used only as a legacy planning anchor.
[^jp401]: Joint Chiefs of Staff, [Joint Publication 4-01, The Defense Transportation System](https://www.jcs.mil/Portals/36/Documents/Doctrine/pubs/jp4_01_20170718.pdf), 2017.
[^lmcs]: U.S. Army Engineer Research and Development Center, [Lightweight Modular Causeway System](https://www.erdc.usace.army.mil/Media/Fact-Sheets/Fact-Sheet-Article-View/Article/476717/lightweight-modular-causeway-system/).
[^irb]: U.S. Army, [Improved Ribbon Bridge](https://asc.army.mil/docs/wsh2/2005-wsh.pdf).
[^lots]: Naval Facilities Engineering Systems Command, [Logistics Over the Shore program](https://www.navfac.navy.mil/PEO-Infrastructure-and-Expeditionary/PMO-314-LOTS/).
[^spmt]: Federal Highway Administration, [Self-Propelled Modular Transporters for Accelerated Bridge Construction](https://www.fhwa.dot.gov/publications/focus/07dec/02.cfm).
[^c17]: U.S. Air Force, [C-17 Globemaster III payload benchmark](https://www.af.mil/News/Features/Article/142847/c-17-globemaster-iii-amcs-workhorse-meeting-airlift-needs-across-the-globe/).
[^c130]: U.S. Air Force, [C-130 Hercules fact sheet](https://www.af.mil/About-Us/Fact-Sheets/Display/Article/1555054/c-130-hercules/).
