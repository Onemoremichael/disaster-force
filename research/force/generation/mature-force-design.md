# Mature force design: the operational grammar of the Department of Resilience

## Design judgment

The Department of Resilience should not be organized as an enlarged emergency-management agency with unusually large equipment accounts. It should contain a **permanent national operating establishment** that can generate, deploy, sustain, replace, and regenerate complete civilian-service formations across several simultaneous campaigns.

The mature structure has three distinct objects:

1. the **Department of Resilience**, which makes policy, sets the national readiness promise, controls resources, governs civil authority, and maintains public accountability;
2. the **National Resilience Establishment**, which includes the seven operating services, commands, schools, laboratories, acquisition system, depots, reserves, state and tribal components, and certified industrial base that generate capacity; and
3. the **Resilience Force**, meaning the certified headquarters, units, stocks, transport, and support actually assigned or available for operations.

These are not synonyms. A department can exist without a ready force. An inventory can exist without crews. A contractor can exist without being available during correlated national demand. A technical module can arrive without the reception, distribution, waste, replacement, and transfer systems that turn output into sustained civilian service. The proposed institution is credible only if its public promise can be traced through all three objects.

The Department should therefore be designed around a **force-generation contract**:

> For each declared service objective, the establishment will maintain enough certified, deployable, and regenerable formations to deliver the required effect in the stated places, conditions, and time bands while preserving the national concurrency reserve.

That is a much larger proposition than coordinating federal assistance. It is the civilian equivalent of maintaining national power at readiness.

## What this pass adds

Earlier passes established the [Department and its operating services](../../mandate/department-of-resilience.md), [effect portfolios and force components](force-composition.md), [readiness and geographic posture](readiness-and-force-generation.md), mission modules, and an [initial quantitative envelope](../../programmatics/force-and-resource-model.md). Pass 33 subsequently separated person-specific mobility from common-user logistics and made it a seventh professional service. The formation grammar below remains valid with that addition.

This pass defines that missing layer:

- a common formation grammar;
- permanent unit families for each operating service;
- joint theater-opening, sustainment, mobility, information, and replacement formations;
- the relationship between administrative force generation and operational employment;
- a campaign organization centered on civilian effects rather than service ownership;
- force packages for local, major, catastrophic, and global operations;
- readiness and rotation rules that count complete units rather than nominal assets;
- command and technical-authority boundaries;
- a provisional mature-force scale without pretending that unresolved capability coefficients are validated; and
- the tests required before the structure becomes a program of record.

The purpose is not to copy military organization. Joint doctrine is useful evidence that forces from different professional systems need an integrator and that reception, onward movement, sustainment, reconstitution, and transfer must be designed as operations.[^jp333][^atp493] The mission, authority, performance measure, force mix, and professional culture proposed here are civilian and distinct.

## Deriving a formation from a service deficit

### The demand object

The force should never begin planning with a request for a named asset. It begins with a time-indexed service deficit:

```text
D(e, z, t) = P(z, t) x max[0, S_required(e, z, t) - S_credible_local(e, z, t)]
```

where:

- `e` is a civilian effect such as compliant water, usable electricity, accessible shelter, acute care, mobility throughput, or communications;
- `z` is the service geography or critical node;
- `t` is the time interval;
- `P` is the affected population or critical-function denominator;
- `S_required` is the phased service level; and
- `S_credible_local` is the service likely to survive or be restored without national substitution.

The demand record also carries access, contamination, weather, duration, host-support, dependency, distribution, and uncertainty fields. A population count without those fields is not a force requirement.

### The formation object

For candidate formation `j`, define:

```text
A(e, z, t, j) = safely delivered effect from one formation j
                after setup, derating, distribution loss, maintenance,
                staffing, local interface, and degraded-mode constraints
```

The operational design problem is to choose formations `x_j` such that:

```text
sum_j A(e, z, t, j) x_j >= D(e, z, t)   for every protected effect, place, and time
```

subject to:

- qualified people and shift coverage;
- transport weight, volume, route, berth, runway, rail, and handling constraints;
- power, fuel, feedstock, water, oxygen, data, and consumable limits;
- staging land and host-community burden;
- waste, emissions, residuals, contamination, and retrograde capacity;
- maintenance and replacement pools;
- safety, licensing, clinical, environmental, and technical-authority rules;
- correlated loss of bases, routes, suppliers, and crews; and
- the required residual force for other campaigns.

The objective is not simply to minimize cost or headcount. It is a multi-objective choice among time to stabilized life-support, service shortfall, mortality and morbidity risk, responder exposure, logistics burden, recoverability, lifecycle cost, ecological burden, and transfer quality. A fast package that cannot be sustained is dominated by a slightly slower package that closes the service chain.

The linear notation is an accountability ledger, not an assumption that formations combine linearly in the field. Shared routes, mutually dependent utilities, scarce specialists, congestion, common-mode failures, and beneficial combinations create nonlinear effects. Those relationships belong in explicit constraints and scenario states. Uncertainty should be represented through low/reference/high demand records and correlated disruptions before a later model adopts probabilistic distributions.

### Five quantities that cannot be collapsed

Every force decision must keep five quantities separate:

1. **productive capacity** — plant-gate or technical output;
2. **delivered effect** — service safely received by the intended user;
3. **ready capacity** — delivered-effect capacity certified for the response time band;
4. **deployed capacity** — ready capacity assigned to an operation; and
5. **regenerable capacity** — the replacement crews, repair parts, depots, training pipeline, and industrial flow that preserve output over time.

The [WRG-50 configuration study](../../systems/water/configuration-model.md) demonstrates the distinction. Six treatment trains are only one part of a formation that also requires source qualification, laboratories, 100 kilometers of parallel pipe in the reference case, pressure zones, storage, access interfaces, wastewater and concentrate management, 2,720 deployed people, and a three-echelon establishment. Counting treatment trains would overstate the national water promise by orders of organizational complexity.

## Two organizations must coexist

### The generating organization

The seven services organize, train, equip, certify, sustain, and professionally govern forces:

| Service | Permanent responsibility | What it does not own alone |
|---|---|---|
| Land Engineering Service | Access, earthworks, crossings, debris, flood works, structural stabilization, ground fire control | Strategic movement, utility operation, clinical care, civil priorities |
| Air Response Service | Cargo and force mobility, aerial fire control, sensing, relay, airborne delivery, deployable air operations | Ground reception, onward distribution, civil-passenger regulation, community transfer |
| Maritime Response Service | Ocean, coastal, lake, and river access; port opening; cargo sealift; salvage; offshore production and support | Inland distribution, civil-passenger regulation, utility connection, local patient pathways |
| Infrastructure Restoration Service | Water, wastewater, power, thermal safety, communications utility, fuel systems, controls, and grid repair | Major civil works, strategic transport, public-health authority |
| Health Protection Service | Clinical care, public health, medical logistics, patient regulation, workforce replacement, health protection | General power, water, shelter, and protected-movement systems on which care depends |
| Community Stabilization Service | Shelter, food, essential goods, accessible services, population support, housing transition, public information, local economic continuity | Bulk production, strategic logistics, technical utility release |
| Civil Mobility and Continuity Service | Door-to-node collection; accessible road, rail, air and water passenger movement; transfer nodes; household, clinical and custody continuity; reunification and return | Common-user cargo lift, route repair, receiving capacity, civil priority and sovereign authority |

Each service controls professional qualification, maintenance standards, configuration, safety, technical release, and formation readiness. It does not retain operational control of deployed units merely to protect institutional ownership.

### The employing organization

Geographic and functional commands employ joint forces. A campaign commander receives certified formations and organizes them around service outcomes:

```text
Civil objectives and local authority
└── Resilience campaign commander
    ├── Civil integration and effects command
    ├── Hazard control command
    ├── Access and distribution command
    ├── Life-support utilities command
    ├── Health protection command
    ├── Community continuity command
    └── Theater support command
        ├── Reception and onward movement
        ├── Mobility and movement control
        ├── Sustainment and maintenance
        ├── Information and communications
        ├── Responder health and replacement
        └── Retrograde, transfer, and reconstitution
```

This operational structure is intentionally not a mirror of the seven services. If it were, service seams would become incident seams. The Infrastructure Restoration Service may generate a water group, the Land Engineering Service its corridor-construction elements, the Maritime Response Service its intake and connector elements, and the Health Protection Service its quality and surveillance elements; once assigned, the combined water mission answers to the life-support utilities commander.

Joint Publication 3-33 uses a headquarters to integrate forces generated by different services, while preserving service responsibilities and specialist advice.[^jp333] That integration problem is real even though the Department of Resilience should use different language, civilian authority, and outcome measures.

## Common formation grammar

Names should describe organizational responsibility, not prestige. Headcount bands are planning ranges, not fixed tables of organization.

| Echelon | Typical planning scale | Independent function | Command and support character |
|---|---:|---|---|
| Technical team | 4–20 people | One licensed, analytical, repair, clinical, survey, or operating task | Normally attached; limited independent endurance |
| Detachment | 20–80 | One bounded capability at a site or route segment | Local lead, communications, safety, and entry sustainment |
| Mission module | 60–250 | One measured effect with its immediate distribution or interface tail | Small headquarters, two-shift option, basic maintenance, 72-hour entry load |
| Response group | 400–1,500 | Several modules delivering one complete consequence-chain outcome | Organic planning, logistics, maintenance, data, responder support, and seven-day independence |
| Response command | 2,000–8,000 | Several groups across a metropolitan area, corridor, watershed, or functional effect | Theater distribution, technical authority, replacement management, and 30-day campaign ability |
| Regional resilience force | 8,000–25,000 assigned and aligned personnel | Multiple simultaneous incidents or one major campaign | Standing joint headquarters, reception, mobility, sustainment, civil integration, and reserve relationships |
| Catastrophe stabilization force | 25,000–100,000 task-organized personnel | One national-scale campaign or several linked regional operations | National augmentation, strategic movement, multiple operating bases, rotational depth, and months of endurance |

Personnel scale is not the primary definition. A highly automated pumping group may carry more mass and fewer operators than a health group with the same command echelon. The controlling test is what level can accept an objective, produce a complete measured effect, sustain itself for the stated interval, and be held accountable for transfer.

FEMA's incident doctrine appropriately emphasizes modular expansion, common terminology, and manageable spans of control.[^nims] The Department should retain those interface principles. It should not infer that an incident management chart creates operational capacity. Each box in the new force must correspond to certified people, equipment, support, and output.

## Permanent unit families by service

### Land Engineering Service

The Land Engineering Service should generate five major families:

| Formation family | Complete operational thread | Principal output measure |
|---|---|---|
| Access and route-opening group | survey; hazard marking; clearance; temporary surface; crossing; traffic control; route maintenance | tonnes and priority users moved per route-day under stated access class |
| Flood and water-control group | hydraulic reconnaissance; barriers; high-volume pumping; breach closure; drainage restoration; controlled dewatering | protected or dewatered area and critical nodes within water-level limits |
| Debris and materials group | characterize; clear; segregate; reduce; recycle; transport; document; dispose | certified tonnes processed per day without creating secondary hazard |
| Temporary works group | structural assessment; shoring; bridging; utility corridors; public facilities; habitability works | certified facilities, crossings, or corridor capacity delivered and maintained |
| Ground fire and landscape group | detection interface; line construction; mobile water; structure protection; prescribed fire; repair | protected objectives and durable containment contribution, not acres disturbed |

Each family includes survey, engineering, operators, maintainers, environmental control, safety, logistics, and transfer records. Earthmovers are equipment inside the group; they are not the capability.

### Air Response Service

The Air Response Service should generate:

| Formation family | Complete operational thread | Principal output measure |
|---|---|---|
| Strategic mobility wing | load planning; aircraft; crews; maintenance; aerial port; movement control | complete formations delivered by required delivery time |
| Austere air-access group | assess; clear or repair; establish navigation, fuel, handling, weather, fire/rescue, and airspace control | safe daily aircraft movements and cargo/passenger throughput |
| Aerial hazard-control wing | sense; plan; load; attack; coordinate with ground; maintain; measure hold | delivered objective yield over operational cycles |
| Tactical distribution group | short-field or vertical lift; landing sites; manifests; local movement; evacuation | priority people and tonnes delivered from hub to point of need |
| Air sensing and relay group | crewed and uncrewed sensing; communications relay; processing; dissemination | decision-quality coverage at stated latency and persistence |
| Aeromedical movement group | patient regulation; staging; en-route care; aircraft; receiving interface; return | patients moved by acuity without avoidable care discontinuity |

Aircraft types should follow route geometry and mission throughput. The service should not pursue a unique airframe merely to establish institutional identity.

### Maritime Response Service

The Maritime Response Service should generate:

| Formation family | Complete operational thread | Principal output measure |
|---|---|---|
| Port-opening group | hydrographic and structural survey; channel and berth clearance; salvage; aids; cargo handling; movement control | safe berth, channel, and cargo throughput restored over time |
| Littoral access group | shallow-water connectors; beach and damaged-quay interfaces; ramps; local control; maintenance | passengers, vehicles, and tonnes across the water–land seam |
| Inland-waterway group | river and lake survey; navigation; ferry; barge distribution; rescue; mobile bases | corridor reach and sustained node-to-node throughput |
| Offshore support group | command; workshops; stores; aviation or boat support; utilities; crew recovery | supported formations and operational days without burdening shore systems |
| Maritime production group | water, power, oxygen, cold-chain, communications, or medical production with shore interface | compliant service delivered ashore, including residual management |
| Ocean sustainment group | strategic sealift; afloat stocks; transfer; repair; replenishment; retrograde | campaign mass delivered and returned through constrained ports |

These are product lines, not one universal ship. A port opener, littoral connector, regional medical vessel, offshore water–energy plant, and high-volume sealift vessel have incompatible operating geometries and safety cases.

### Infrastructure Restoration Service

The Infrastructure Restoration Service should generate:

| Formation family | Complete operational thread | Principal output measure |
|---|---|---|
| Water restoration group | source; treatment; quality release; conveyance; storage; distribution; wastewater; residuals; transfer | compliant liters delivered and return flow safely managed |
| Power restoration group | load assessment; generation/storage; protection; distribution; service connection; fuel/energy; synchronization; transfer | critical-load megawatts continuously served at required quality |
| Grid bridge group | damaged-substation bypass; mobile transformation; protection; conductor; controls; synchronization; repair support | stable transmission/distribution capacity restored across a failed node |
| Thermal safety group | building assessment; district or facility cooling/heating; power; ventilation; accessible public service | protected people-hours inside safe thermal envelopes |
| Communications utility group | backhaul; radio and cellular access; dispatch; edge services; power; cyber; provider transfer | priority users and area served at defined availability, latency, and throughput |
| Utility reconstruction group | multidisciplinary repair of water, wastewater, power, controls, fuel, and telecommunications plant | service-capacity restoration curve accelerated against the local baseline |

The WRG-50 is the first configuration study in this family. Equivalent configuration studies are required before the other group labels become credible.

### Health Protection Service

The Health Protection Service should generate:

| Formation family | Complete operational thread | Principal output measure |
|---|---|---|
| Community health continuity group | primary care; pharmacy; dialysis continuity; home-health support; behavioral health; public health | protected patient-days and continuity of time-critical therapy |
| Mobile acute-care group | emergency, surgery, critical care, diagnostics, sterilization, oxygen, laboratory, waste, discharge | staffed and utility-supported care episodes by acuity |
| Theater hospital command | several acute-care groups; specialty services; patient regulation; medical logistics; replacement staff | complete regional care pathway and decompression effect |
| Public-health control group | surveillance; laboratory; vaccination; infection prevention; environmental health; vector control | population risk detected and controlled within defined time bands |
| Patient movement group | regulation; staging; accessible ground movement; aeromedical or maritime care; reception; return | patients moved safely through a complete receiving network |
| Health workforce replacement group | credentialed clinical teams; scheduling; licensing; fatigue and exposure management | qualified shifts supplied to damaged fixed facilities without hollowing other regions |

Nominal beds are prohibited as a readiness metric. The unit is a staffed, supplied, utility-supported, clinically governed care pathway.

### Community Stabilization Service

The Community Stabilization Service should generate:

| Formation family | Complete operational thread | Principal output measure |
|---|---|---|
| Population support group | registration; accessible shelter/lodging; feeding; sanitation; laundry; family support; safeguarding | safely supported person-days with functional-needs compliance |
| Essential-goods group | demand sensing; procurement; cold chain; break-bulk; household distribution; reverse logistics | households receiving the required basket at stated frequency |
| Civil access group | public information; multilingual services; identity and benefits access; communications access; case routing | people able to receive warnings, assistance, health, and administrative service |
| Displacement transition group | shelter exit; housing navigation; site services; schools; transport; workforce connection | durable exits from emergency accommodation without renewed displacement |
| Community institutions group | continuity sites for local government, schools, clinics, courts, commerce, and civil society | critical civic functions reopened and locally governed |
| Economic restart group | market assessment; contractor integration; temporary commercial nodes; payment and logistics access | local enterprises and supply channels returned to operation |

This service is not a softer tail added after engineering. It converts technical output into legitimate, accessible, and durable human service.

## Joint formations that cannot be improvised

Some organizations must be permanently joint because no generating service can provide their effect alone.

| Joint formation | Why it exists before the incident | Minimum complete functions |
|---|---|---|
| Civil integration and effects group | turns local authority and service priorities into measurable objectives | liaison, public information, rights, disability integration, tribal affairs, geospatial analysis, effects assessment |
| Theater-opening command | a broken community cannot be assumed to receive a national force | port/airfield/rail/road assessment, reception, staging, onward movement, cargo handling, initial bases, movement control |
| Theater sustainment command | every productive module creates fuel, stock, repair, responder, and waste demand | supply, distribution, maintenance, calibration, fuel, responder life support, contracting, waste, retrograde |
| Resilience information group | the force requires a shared operational and infrastructure model under degraded communications | communications, edge compute, data fusion, infrastructure telemetry, cyber, spectrum, public-data interfaces |
| Replacement and reconstitution group | the first crew and first equipment set cannot be treated as the whole campaign | personnel replacement, exposure tracking, equipment recovery, decontamination, repair, retraining, return to readiness |
| Transfer and demobilization group | withdrawal can create a second service collapse | asset disposition, records, local training, utility acceptance, environmental closeout, contract closure, retrograde |

Theater opening deserves particular emphasis. Army doctrine treats reception, staging, onward movement, initial sustainment, movement control, and distribution as a combined operation because arrival at a port is not arrival as a usable force.[^atp493] The Department needs a civilian version built for damaged communities, accessible evacuation, contaminated flows, public utilities, and local sovereignty.

## The force-package library

The Department should maintain a small set of **command-and-support packages** and a large library of effect groups. The former create an operating environment; the latter are selected from the demand vector.

### Type L: local reinforcement package

**Use:** a bounded incident that overwhelms a locality but leaves regional systems substantially functional.

- one integration detachment;
- one to three effect modules;
- one sustainment detachment;
- commercial or local movement with a verified fallback;
- 72-hour independent entry load; and
- a transfer horizon generally measured in days.

Planning scale: roughly 100–600 deployed people. This package should normally be sourced by a forward station or state/tribal component.

### Type M: major regional response force

**Use:** several damaged jurisdictions or one metropolitan, watershed, fire, health, or infrastructure campaign.

- deployable joint headquarters;
- civil integration and effects group;
- theater-opening group;
- two to eight effect groups selected by service deficit;
- theater sustainment group;
- mobility, information, health protection, and replacement elements;
- at least two operating bases or a survivable alternative; and
- 30-day organic campaign design with planned follow-on rotations.

Planning scale: roughly 3,000–12,000 deployed people. The defining feature is not size; it is the ability to run several linked service lines without transferring the integration burden back to the damaged jurisdiction.

### Type C: catastrophe stabilization force

**Use:** multi-state, territorial, or national-level loss of several lifelines; mass displacement; severe receiving-capacity damage; or a long-duration campaign.

- campaign headquarters with subordinate area or effect commands;
- full theater-opening and movement-control command;
- multiple access, utility, health, community, and hazard-control commands;
- dedicated strategic air and maritime movement allocation;
- theater distribution, depots, maintenance, medical support, responder bases, and replacement flows;
- distributed operating bases resilient to the same hazard;
- industrial mobilization cell and long-lead stock control;
- independent operational assessment; and
- transfer and reconstitution commands established at the beginning.

Planning scale: approximately 25,000–100,000 deployed people, potentially higher for an island, contaminated, or mass-displacement campaign. This range is a planning envelope. The design-reference mission and capability models must generate the actual force.

### Type G: global stabilization force

**Use:** host-nation invitation for a catastrophe whose stabilization is a major humanitarian and strategic objective.

- internationally certified joint headquarters;
- sovereign liaison and multinational coordination;
- austere theater opening and independent sustainment;
- modular effect commands compatible with partner standards;
- customs, medical, aviation, maritime, environmental, labor, and asset-transfer authorities prepared before deployment;
- security supplied by the host, a partner, or a separately authorized U.S. instrument; and
- a defined host-nation capacity-building and transfer pathway.

Planning scale: approximately 8,000–30,000 people for the American contribution, with multinational augmentation. Domestic certification alone is insufficient because sovereignty, standards, language, supply, clinical authority, and transfer differ.

## A reference catastrophe force—not a universal template

The table below is an **allocation frame** for planning and exercises. Counts vary with service demand; a drought, megafire, earthquake, pandemic, and coastal storm should not produce the same force.

| Force element | Reference allocation | Scaling driver |
|---|---:|---|
| Campaign headquarters | 1 | geography, subordinate commands, coalition and civil complexity |
| Civil integration and effects groups | 2–6 | governments, languages, access needs, population, information environment |
| Theater-opening commands | 1–3 | independent entry corridors and damage correlation |
| Hazard-control commands | 0–4 | active fire, water, contamination, structural, biological, or geotechnical process |
| Access and distribution commands | 1–4 | route classes, isolation, displacement, daily mass flow |
| Life-support utility commands | 1–5 | water, wastewater, power, thermal, communications and fuel deficits |
| Health protection commands | 1–3 | affected population, acuity, facility damage, patient export capacity |
| Community continuity commands | 1–4 | displacement, shelter duration, accessibility, institutional disruption |
| Theater sustainment commands | 1–3 | number of bases, daily tonnage, distance, contamination, campaign duration |
| Replacement and reconstitution groups | 2–8 | exposure, fatigue, technical density, maintenance and decontamination load |
| Transfer and demobilization command | 1 | number of systems and owners, environmental closeout, asset disposition |

This frame makes two design choices explicit. First, sustainment and reconstitution are commands, not percentages silently added to each platform. Second, the Department does not pre-build a hurricane force, earthquake force, and wildfire force. It builds consequence-specialist formations that train in several hazard combinations, then assembles campaign forces from measured service deficits.

## Command, control, and professional authority

### Four authorities must remain distinct

| Authority | Holder | Decision |
|---|---|---|
| Civil objective authority | affected legitimate governments through the Civil Resilience Authority | priorities, protected populations, acceptable disruption, transfer conditions |
| Operational control | geographic or campaign commander | task organization, sequencing, allocation, supported/supporting relationships |
| Technical control | service chief engineer, medical director, aviation/maritime authority, safety and environmental authorities | professional standards, safe operating envelope, certification, release and stop-work |
| Administrative control | generating service | personnel, training, equipment configuration, maintenance, career and readiness systems |

The two-key rule remains: civil authorities determine legitimate ends; the operational force determines how assigned resources are employed within law and professional safety. Neither key is sufficient alone.

### The supported-command rule

For each phase and service objective, one command is designated **supported** and other formations are **supporting**. This prevents every service from optimizing its own output while the population receives no complete effect.

Example: for restoration of dialysis continuity, the Health Protection command may be supported; Infrastructure supplies power and water, Air or Land moves patients and staff, Community maintains accessible transport and case contact, and Theater Sustainment supplies oxygen, pharmaceuticals, fuel, and waste removal. Once fixed facilities are stable, the supported role may shift to Infrastructure or Community for transfer.

### Headquarters should be a standing capability

A campaign headquarters is not a meeting assembled from whichever senior officials are free. It requires collectively trained command groups, planners, logisticians, engineers, clinicians, data teams, public-information staff, legal advisers, civil-rights and disability integration, contracting, safety, environmental authority, and liaison capacity. Joint doctrine's case for a trained integrator is applicable by analogy; the civilian headquarters must additionally expose its assumptions, service outcomes, and distributional consequences to public oversight.[^jp333]

## Deployment is a sequence, not an arrival time

The Department should plan six overlapping waves:

| Wave | Indicative start | Purpose | Exit condition |
|---|---:|---|---|
| 0. Anticipatory posture | before impact where forecast permits | move outside correlated loss; establish liaison; protect routes and stocks | employment authorized or threat passes |
| 1. Find and connect | 0–12 hours | civil link, sensing, communications, route and node survey, immediate rescue support | decision-quality operating picture and initial priorities |
| 2. Open and protect | 6–48 hours | reception nodes, access, hazard control, responder bases, critical medical and utility continuity | at least one safe force and supply corridor functions |
| 3. Substitute life support | 1–7 days | water, power, health, communications, shelter, food, sanitation, local mobility | stabilization bundle reaches protected population |
| 4. Expand and repair | 3 days–8 weeks | increase service levels, restore networks, rotate crews, process debris, support institutions | fixed or durable interim systems can accept load |
| 5. Transfer and regenerate | begins on day 1; continues months | train and hand off; retrograde; repair; decontaminate; document; restore force readiness | no service cliff and units return to certified readiness |

These times are decision bands, not promises that every geography can meet them. The force must report both first effect and full sustainable effect. “Federal assets arrived” is not a service outcome.

## Readiness and force generation

### Readiness is a vector

For formation `j`, readiness should be reported as:

```text
R_j = min(P_j, E_j, C_j, M_j, L_j, S_j, I_j, A_j)
```

where:

- `P` = qualified people and replacement shifts;
- `E` = equipment mission capability;
- `C` = consumables and entry stocks;
- `M` = strategic and onward movement availability;
- `L` = receiving and staging plan;
- `S` = sustainment and maintenance closure;
- `I` = technical, data, and civil interfaces; and
- `A` = authority and certification.

The minimum formulation is deliberately unforgiving. The unavailable critical link governs. A second dashboard may show the reasons for non-readiness, but averages must not disguise a zero.

### Four force pools

Every complete formation belongs to one of four pools:

1. **committed** — deployed or executing a real domestic or global mission;
2. **ready** — certified within its assigned response band, with movement and entry load;
3. **preparing** — training, maintenance, personnel replacement, or forecast posture; and
4. **recovering** — retrograde, repair, decontamination, leave, health surveillance, and collective requalification.

National capacity is the ready pool plus only the portion of the preparing pool that can meet a stated response time without breaking certification. Recovering units are not counted because their equipment is physically present.

### Rotation factors are formation-specific

The WRG-50 currently uses three operational echelons plus school and depot overhead. That is not automatically correct for every force. A technical crew operating continuously under ordinary exposure may use a three-unit cycle; a contaminated-environment team, ICU workforce, flight crew, or arduous fire-line unit may require greater depth. A locally rooted reserve engineering group may require a different activation model.

For formation `j`:

```text
owned formations_j = ceiling[(simultaneous deployed demand_j x (1 + residual reserve fraction_j))
                             / mission availability_j]

personnel establishment_j = deployed positions_j
                          x shift factor_j
                          x rotation factor_j
                          x qualification fill factor_j
                          + school, depot, test, and command overhead_j
```

The factors must be tested separately. One enterprise-wide “tooth-to-tail” or rotation ratio would conceal the actual bottleneck.

GAO's findings on concurrent disasters, limited deployable workforce, and qualification mismatch show why nominal headcount is weak readiness evidence.[^gao25workforce][^gao26workforce] The proposed force should know which complete formations can cross the line of departure, not merely how many employees or reservists are enrolled.

## Components and the division of readiness labor

### Active component

The active component owns the no-notice, technically dense, capital-intensive, and continuously exercised core:

- standing headquarters and civil-integration cadres;
- theater opening and movement control;
- high-readiness water, power, communications, access, health, air, and maritime groups;
- strategic mobility and maintenance;
- nuclear, aviation, maritime, clinical, environmental, and engineering authority;
- schools, evaluation, laboratories, acquisition, depots, and test units; and
- the first two operating shifts for nationally scarce systems.

### Federal reserve

The federal reserve supplies complete follow-on units, specialist depth, long-duration rotations, and civil-sector skills. Collective tasks require collective units with assigned equipment and annual field certification. Individual reservists fill positions only where unit cohesion is not a performance condition.

### State and territorial resilience guards

These components provide local presence, daily hazard reduction, and regional mass while remaining nationally typed and inspected. They should contain complete units—especially route opening, community support, public health, communications, utility repair, ground fire, and distribution—not unstructured personnel pools. Federal funding buys a national readiness obligation as well as a governor-controlled capability.

### Tribal resilience compacts

Tribal nations should generate and command nationally funded formations through direct compacts. Their units may specialize in remote access, community continuity, communications, fire and landscape, water, health, cultural resources, and local infrastructure while meeting the same certification rules. They are not state subcomponents.

### Civil auxiliary

The auxiliary supplies pre-credentialed local knowledge, facilities, low-frequency specialists, and community networks. It is not counted in minimum ready capacity unless its contribution is typed, exercised, supported, and legally available.

### Certified industrial force

Industry provides surge production, repair, construction, transportation, technical field teams, and selected complete operating packages. A vendor enters the national readiness inventory only when the Department has verified:

- the specific people, plant, equipment, stocks, and subcontractors;
- priority under simultaneous commercial and government demand;
- mobilization, movement, and setup time;
- field maintenance and replacement depth;
- interoperability, data, safety, environmental, and credential requirements;
- pricing and liability under activation;
- participation in national exercises; and
- survival of supplier, utility, cyber, port, and transport disruption.

This is an industrial component of the establishment, not ordinary procurement. The Department must be able to mobilize Lockheed-scale engineering depth without confusing corporate existence with operational readiness.

## Provisional mature scale

The original quantitative workbook yielded approximately 302,000 active and 396,500 reserve personnel. Pass 23's [joint force allocation study](joint-force-allocation-and-order-of-battle.md) supersedes that top-down screen as the current force-generated reference. Its thirty-four formation families and ten simultaneous campaigns produce about 714,000 people deployed and 3.95 million affiliated billet-equivalents after rotation, components, institutional depth and the integrated utility force. Neither result is a validated table of organization; the scale jump is evidence that the earlier workforce did not generate this paper's mature promise.

A coherent mature posture would contain, at minimum:

- six service headquarters and their training, maintenance, safety, and acquisition systems;
- a joint Resilience Staff;
- domestic geographic commands derived from network and hazard analysis rather than inherited administrative regions;
- one Global Resilience Command;
- functional commands for mobility, sustainment, information and forecast, medical regulation, industrial mobilization, and training/doctrine;
- standing regional resilience forces with assigned active units and habitual reserve, state, tribal, industrial, and civil partners;
- nationally held scarce aviation, maritime, medical, utility, and technical formations;
- community interface detachments, forward stations, regional complexes, strategic mobility bases, depots, arsenals, ship and aviation maintenance, laboratories, and proving grounds; and
- force-generation depth sufficient for `3 catastrophic + 5 major + 2 global + 20 percent residual reserve` unless later demand modeling changes that standard.

The joint allocation model now distributes the force by formation and component rather than service percentage. Its coefficients remain provisional. Its intentionally coarse all-mass-at-once screens fail strategic movement and all ten damaged-theater reception cases. Pass 24's time-phased deployment-enterprise model closes the ten reference chains but still fails Cascadia and an allied megacity under correlated primary-path loss. Pass 25 resolves Cascadia into nine service islands and an item-level campaign that closes only by adding independent safe-zone origins, no-pier and shallow-draft paths, zero-host-utility bases and explicit supply, return and regeneration. Heavy engineering, health, mobility, community and theater-opening formations remain short of configuration-level evidence.

## Decisions that reject institutional preservation

The mature design makes the following choices explicit:

1. **FEMA does not remain the center of gravity.** Its legitimate civil coordination, assistance, insurance, grant, and recovery functions are redistributed; it does not define the operating force.
2. **No current emergency-support-function chart becomes the service structure.** The force is organized around delivered effects and complete consequence chains.
3. **The military is not the mobility, logistics, engineering, medical, or communications backstop of first resort.** Interdepartmental support remains possible, but Department readiness cannot be scheduled around defense availability.
4. **USACE, NDMS, wildfire mobilization, public-health teams, and search-and-rescue systems are evidence and transition sources, not ceilings.** Their people and practice may seed new services; their part-time or borrowed-capacity models do not constrain the mature state.
5. **Utilities and contractors are partners, not assumed absorbers of catastrophic risk.** The Department owns a substitution floor and an industrial mobilization system for correlated national demand.
6. **Volunteers, agreements, contracts, and catalog assets are not reported as ready units.** Only verified complete packages count.
7. **The Department builds permanent mass.** Elite reconnaissance and technical teams matter, but stabilization of millions of people also requires operators, trades, clinicians, drivers, maintainers, warehouse crews, community specialists, instructors, and replacement personnel at industrial scale.

This is the practical meaning of parity of seriousness. It is not copying uniforms or ranks. It is accepting that assured service projection requires deep institutions, redundant capacity, trained formations, logistics, industry, and generational professional investment.

## Acquisition consequence: procure formations

Each major acquisition program should deliver a **formation increment**, not merely a platform lot. A program baseline should include:

- productive systems and all distribution or access interfaces;
- operators, maintainers, licensed authorities, instructors, and replacement crews;
- transport fixtures, handling systems, movement data, and reception equipment;
- command, communications, sensing, cyber, and data systems;
- entry stocks and the steady-state supply chain;
- field repair, calibration, contamination control, depot tooling, and technical data;
- training devices, school seats, proving-ground capacity, and operational test;
- waste, emissions, residuals, retrograde, and environmental closure;
- host-owner transfer kits and data rights;
- block modernization and recapitalization; and
- the bases, berths, hangars, warehouses, utilities, and security required to keep it ready.

The cost of the platform is therefore only one line in the cost of a ready effect. This principle should govern the later renderings: a vehicle can be illustrated only when the formation it belongs to, the interfaces it depends on, and its share of the service outcome are known.

## Test program for the force design

The organizational architecture should advance through five evidence gates.

### F1 — analytical closure

- every design-reference mission produces a time-phased service-deficit vector;
- candidate formations have effect, footprint, time, dependency, and failure records;
- the allocation model closes service demand, support, movement, and residual reserve;
- no personnel, lift, fuel, host-support, waste, or transfer burden is double-counted or omitted.

### F2 — command-post closure

- standing headquarters plan two simultaneous unfamiliar campaigns;
- authorities, supported/supporting relationships, resource arbitration, and public reporting work under degraded information;
- civil, state, tribal, territorial, utility, health, industry, and international interfaces are exercised.

### F3 — deployment closure

- complete units alert, load, move, receive, stage, integrate, and begin sustained effect on measured timelines;
- theater-opening capacity is damaged or constrained during the test;
- the exercise records delivered civilian service rather than assets dispatched.

### F4 — endurance and replacement closure

- formations operate through at least one crew rotation and major maintenance cycle;
- fuel, feedstock, medical materiel, parts, waste, data, contracting, and responder support sustain output;
- contaminated or damaged equipment is recovered and repaired;
- a second campaign is activated before the first demobilizes.

### F5 — transfer and national regeneration closure

- local or partner owners accept systems without a service cliff;
- personnel and equipment return through health, repair, decontamination, retraining, and recertification;
- residual national readiness returns to its target in a measured interval;
- industrial production and depot flows replace loss and consumption.

The force design remains a hypothesis until it passes these gates.

## What should be engineered next

The WRG-50 proved that a seemingly simple output can imply a large formation and deployment mass. The next configuration studies should test whether that result generalizes or whether water is unusually heavy:

1. **Power Restoration Group** — critical-load archetypes, generation and storage mix, fuel or energy chain, cable and protection, connection labor, grid transfer, maintenance, and thermal-service coupling.
2. **Access and Route-Opening Group** — damage geometry, debris and material flow, equipment productivity, crossing classes, operator/maintenance depth, fuel, and route-throughput outcome.
3. **Mobile Acute-Care Group** — acuity demand, licensed shifts, diagnostics, oxygen, sterile processing, pharmacy, waste, utilities, patient regulation, receiving care, and replacement staff.
4. **Aerial Hazard-Control Wing** — cycle time, base network, weather, payload, accuracy, availability, maintenance, loading system, ground-force integration, and delivered objective yield.
5. **Theater-Opening Command** — Pass 24 supplies the first-order [National Resilience Deployment and Distribution Enterprise](../projection/joint-deployment-and-distribution-enterprise.md). Pass 25's [Cascadia campaign](../../proving/campaigns/cascadia-joint-resilience-campaign.md) adds actual load records, path classes, queues, bases, ninety-day supply, reverse flow and reconstitution. The remaining task is to replace design coefficients with asset-level surveys, complete manifests, stochastic damage and representative full-mission trials.

Pass 26's [Cascadia covariance and assurance study](../../proving/campaigns/cascadia-network-covariance-and-assurance.md) changes the organizational unit behind all five priorities. A formation or path receives independent campaign credit only when its origin, energy, communications, workforce, repair, technical release and civil interface can continue without the corresponding layers of adjacent formations. The Department must therefore generate **independently supportable campaign cells**, not merely interoperable functional units. Readiness and allocation systems need a dependency pedigree and correlation budget for every cell.

The provisional order of battle now exists as a falsifiable allocation model. It should not become stable force structure until at least one heavy technical formation, one labor-dense care formation, one mobility formation, one community formation and one theater-support formation close to R3 and survive a joint campaign-and-regeneration trial.

## Bottom line

The Department of Resilience becomes an equal instrument of national power only when it can answer four questions with names, numbers, and evidence:

1. Which complete formation owes each civilian effect?
2. Which command can employ it across a broken operating environment?
3. Which replacement, logistics, industrial, and training system keeps it available through simultaneous campaigns?
4. How quickly can the nation restore both the affected community and the readiness of the force?

The mature answer is not a federation of current agencies and not a fleet of dramatic platforms. It is a national establishment composed of permanent professional services, joint effect commands, theater-opening and sustainment formations, active and reserve depth, sovereign industrial capacity, and a measured chain from public objective to safely delivered and transferred civilian service.

[^jp333]: Joint Chiefs of Staff, [*Joint Publication 3-33: Joint Force Headquarters*](https://www.jcs.mil/Portals/36/Documents/Doctrine/pubs/jp3_33.pdf), June 9, 2022. Used by analogy for a trained integrating headquarters, service-generated forces, command relationships, sustainment, and transition; not adopted as civilian-response doctrine.
[^atp493]: Department of the Army, [*ATP 4-93: Sustainment Brigade*](https://www.benning.army.mil/mssp/PDF/atp4_93.pdf), August 2013, paras. 2-6–2-12. Used by analogy for theater opening, reception, staging, onward movement, distribution, and movement control.
[^nims]: Federal Emergency Management Agency, [*National Incident Management System*, 3rd ed.](https://training.fema.gov/EMIWeb/IS/IS700b/Handouts/National_Incident_Management%20System_Third%20Edition_October_2017.pdf), October 2017. Used for modular organization, manageable span, common terminology, resource management, and authority interfaces—not as a force-structure template.
[^gao25workforce]: U.S. Government Accountability Office, [*Disaster Assistance High-Risk Series: Federal Response Workforce Readiness*](https://www.gao.gov/products/gao-25-108598), GAO-25-108598, September 2, 2025.
[^gao26workforce]: U.S. Government Accountability Office, [*FEMA Workforce: Staff Reductions and Lack of Planning May Impact Mission Readiness*](https://www.gao.gov/products/gao-26-108427), GAO-26-108427, August 4, 2026.
