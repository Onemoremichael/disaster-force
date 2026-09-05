# Information, autonomy, and common enablers

## Design judgment

The Department of Resilience should treat information, communications, computation, positioning, logistics, maintenance, and robotics as operational infrastructure. They are not headquarters support functions. Each is a delivered service that must survive loss of commercial power, terrestrial backhaul, cloud access, positioning signals, local technical staff, and normal supply chains.

The information objective is not a perfect common picture. It is timely reduction of consequential uncertainty: who is at risk, which services have failed, which routes and nodes work, what capacity is actually producing, what demand is unmet, and what decision must be made next.

## Five-layer communications architecture

| Layer | Users and effect | Design requirement |
|---|---|---|
| Personal safety | affected people, responders, sensors | alerts, distress, location consent, low-bandwidth messaging and accessible public information |
| Incident | teams, vehicles, aircraft, vessels and local command | push-to-talk, data, telemetry, position, tasking and life-safety priority |
| Area | multiple incidents and jurisdictions | interoperable voice/data, spectrum coordination, roaming, identity and gateway services |
| Backhaul | field systems to national/allied networks | diverse satellite, terrestrial, microwave, airborne and surviving commercial paths |
| Public continuity | community institutions and population | temporary broadband, charging, broadcast, call centers, service portals and restoration support |

Each layer must have a minimum isolated mode. A field hospital does not need national cloud access to administer medication safely; an autonomous pump must stop safely if its control link fails; a community should receive warnings through more than smartphone data service.

NIST's deployable public-safety work identifies coverage, standalone operation, multiple backhaul options, power, interoperability, usability, and rapid power-on as core requirements.[^nist-deployable] The Department should acquire these as an integrated network product line rather than as incident-by-incident collections of radios and satellite terminals.

## Communications system families

### C-1: responder mesh kit

Human-portable and vehicle kits create local voice, data, position, sensor, and distress networks. They provide:

- multiband and standards-based interoperability;
- local identity and role control;
- store-and-forward messaging;
- gateways to public-safety, military, amateur, commercial, maritime, aviation, and allied systems where authorized;
- replaceable batteries and several charging paths;
- simple configuration by trained operators rather than vendor engineers; and
- offline maps, forms, medical references, and language tools.

### C-2: incident network node

A road-, air-, or boat-mobile node provides local radio access, private cellular or equivalent broadband, Wi-Fi, edge computing, sensor ingestion, spectrum monitoring, and several backhaul choices. It operates within minutes, not days, and can serve independently when upstream links are absent.

Nodes form a self-discovering federation. Loss of one node reduces capacity rather than collapsing the incident network.

### C-3: airborne coverage and relay system

Tethered aerostats, rotorcraft, fixed-wing aircraft, and high-altitude platforms serve different endurance, weather, airspace, and coverage needs. The Department should buy coverage-hours at defined bandwidth and availability, not generic aircraft.

The system includes launch and recovery, spectrum authority, weather limits, backhaul, edge services, maintenance, aviation coordination, and ground-network integration. It cannot assume a clear sky, uncongested spectrum, or continuous satellite link.

### C-4: strategic backhaul and sovereign emergency cloud

The Department requires contracted and owned capacity across multiple commercial and government satellite or terrestrial providers, portable gateways, protected national data centers, regional edge centers, and a disconnected-operating environment.

The architecture should prevent one provider, orbital layer, ground station, proprietary license server, or identity service from becoming a fleet-wide failure. Sensitive health, location, immigration, tribal, commercial, and infrastructure data remain governed by purpose and role; emergency does not erase civil rights.

### C-5: public continuity package

This family restores the minimum digital public sphere: multilingual and accessible warnings, community charging, temporary connectivity, benefit and reunification access, rumor correction, public-service status, broadcast/radio, and channels for people without devices or accounts.

The Department should publish machine-readable service status and uncertainty. It should not turn response into compulsory enrollment in one federal identity or application.

## Observation and decision systems

### O-1: rapid damage and service survey

Survey teams combine satellite and airborne imagery, uncrewed aerial and ground sensing, utility telemetry, crowdsourced reports, field inspection, and local knowledge. The output is not merely a damage map. It is a versioned service-state record:

```text
location × population/function × service × quality × time × confidence × source
```

This record feeds the mission-engineering model and exposes where reported production has not become delivered service.

### O-2: infrastructure digital twin and dependency graph

The Department should maintain planning models for critical national and regional systems before disasters: power, water, fuel, communications, health, transport, food, industrial supply, and public facilities. These models need enough fidelity to estimate failure propagation and routing, not a universal real-time replica of every asset.

Owners retain control of proprietary and security-sensitive operating details. The Department sets data interfaces, exercises degraded-data assumptions, and maintains public or synthetic fallback layers so private data withdrawal cannot halt operations.

### O-3: Earth-observation constellation and data agreements

Space-based observation is valuable for persistent wide-area weather, fire, flood, ground deformation, communications damage, vegetation, thermal, and night-light indicators. The appropriate architecture is mixed:

- enduring federal environmental and scientific missions;
- assured commercial imagery and analytic capacity;
- allied data exchange;
- hosted payloads and small satellites where a unique revisit or sensor gap persists; and
- airborne/local sensing for clouds, smoke, resolution, and rapid tasking gaps.

The Department should not duplicate a full civil space agency. It should own mission requirements, priority access, ground processing, analytic validation, and selected gap-filling assets.

### O-4: mission decision environment

Decision software should show demand, uncertainty, access, resource commitments, alternative courses, downstream dependencies, and time value. Optimization can propose allocations, but accountable officials choose when priorities implicate life, equity, property, or sovereign relationships.

Every recommendation records assumptions and data age. Operators can inspect why a route, evacuation, water allocation, energization, or fire mission was proposed.

## Autonomous and robotic force

### Employment doctrine

Robotics are justified when they do at least one of four things:

1. remove people from lethal or contaminating exposure;
2. sustain repetitive work beyond human endurance;
3. distribute sensing or delivery at otherwise impossible scale; or
4. perform precision work where damaged access prevents conventional equipment.

Labor substitution alone is not a sufficient strategic case. Remote supervision, recovery, charging, communications, spares, decontamination, certification, and cybersecurity remain real force burdens.

### R-1: aerial survey and light-delivery family

Small and medium aircraft map, inspect, sample, relay communications, mark routes, pull pilot lines, deliver urgent medical or repair payloads, and monitor hazards. Variants need standardized mission bays, batteries or fuels, control protocols, remote identification, geofencing, weather characterization, and safe loss-of-link behavior.

### R-2: heavy cargo shuttle

Large uncrewed aircraft or optionally crewed vehicles move repeat loads along surveyed corridors. The concept is valuable for islands, mountains, severed roads, and hazardous zones, but only if ground handling and landing-node throughput match airborne capacity.

No payload-range claim counts without reserve energy, weather diversion, communications loss, alternate landing, loading time, battery/fuel logistics, and maintenance availability.

### R-3: hazardous earthwork and fireline system

Optionally crewed dozers, excavators, loaders, trenchers, compactors, masticators, and carriers conduct fireline, debris, levee, landslide, contaminated-soil, and demolition work. Their common autonomy kit provides perception, precision positioning alternatives, supervised control, geofencing, work recording, and immediate local stop.

The machine must retain a protected local-control mode. Fleet software failure cannot immobilize the heavy-engineering force.

### R-4: water and utility inspection/repair system

Ground, surface, underwater, and aerial robots inspect pipe, lines, substations, tunnels, levees, bridges, intakes, sewers, tanks, and confined spaces. Specialized systems cut, clean, patch, place sensors, pull conductors or hose, and make bounded connections.

Robots do not eliminate excavation, isolation, certification, or energization authority. Their strongest case is finding faults faster and reducing exposure.

### R-5: warehouse, depot, and distribution automation

The Department can obtain its largest routine autonomy gains in controlled environments. Automated handling, inventory, inspection, cold chain, kit assembly, loading, and parts movement improve readiness visibility and reduce deployment error. Systems should use open logistics identities and permit manual operation during software outage.

### R-6: clinical and community-support robotics

Admitted applications include telepresence, pharmacy and laboratory handling, disinfection, materials movement, mobility assistance, and remote vital-sign collection. Diagnosis, treatment consent, triage priority, custody, and benefits decisions remain human-accountable.

## Common logistics architecture

### One item identity, several levels of truth

Every serialized major asset and controlled stock should have a Department identity linked to configuration, owner, location, readiness, maintenance, calibration, shelf life, cyber baseline, transport constraints, and mission history. Data confidence and timestamp are shown explicitly.

This is not a promise that all inventory is visible continuously. Offline transactions synchronize later, and manual counts remain part of assurance.

### Interchange and repair hierarchy

The Arsenal should design systems around four repair levels:

| Level | Location | Work |
|---|---|---|
| Operator | point of use | inspect, clean, replenish, replace simple modules, safe isolation |
| Field | deployed formation | diagnose, exchange line-replaceable units, fabricate simple parts, calibrate |
| Regional | resilience complex | overhaul subsystems, structural repair, software reconstitution, test |
| National depot | specialized industrial site | remanufacture, reactor/airframe/hull overhaul, major modification, life extension |

Maintenance time, test equipment, technical publications, and qualified technicians are included in unit readiness. A stored platform without a repair and calibration system is a display asset.

### Mission-module logistics

Each deployable module carries a digital and physical placard stating:

- mass, dimensions, center of gravity, lifting and tie-down points;
- transport modes and restrictions;
- required power, fluids, data, foundations, clearances, and environmental limits;
- crew and skill requirements;
- setup, shutdown, decontamination, and repacking time;
- consumables and waste by operating hour;
- maintenance interval and critical spares; and
- compatible Department interface revisions.

Module standardization should reduce connection work, not conceal an incomplete product. A desalination module still needs intake, pretreatment, concentrate, pumping, storage, quality assurance, and delivery.

## Energy and software independence

The common equipment architecture should avoid fleet-wide dependence on one fuel or proprietary digital service. This does not require every platform to be multifuel or open source. It requires portfolio resilience:

- electrical systems support common voltage and protection interfaces;
- batteries use a controlled number of form factors and chemistry safety cases;
- liquid-fuel systems state quality tolerance and conversion limits;
- software has escrow or sovereign sustainment rights for mission-critical functions;
- critical devices do not require subscription validation to start;
- security updates can be staged and rolled back;
- time, positioning, identity, and maps have local fallback; and
- operators can enter a safe manual mode.

## Test and evaluation environment

The Department needs proving grounds that reproduce smoke, heat, salt, floodwater, debris, ash, dust, cold, contaminated environments, damaged utilities, congested spectrum, disconnected networks, short airfields, austere shorelines, and mass-casualty workflow. Systems are tested as formations across the complete thread.

A communications kit is evaluated while pumps, medical devices, robots, aircraft, utilities, public users, and local networks compete for service. An autonomous dozer is evaluated with dust-obscured sensors, lost positioning, communications interruption, humans nearby, and a field repair. A logistics system is evaluated with deliberate data corruption and offline nodes.

## Requirement verdicts

| Concept | Verdict | Governing condition |
|---|---|---|
| One universal national disaster cloud | Reject | Disconnection, provider concentration, rights, latency and local authority require federation |
| Federated sovereign emergency data plane | Admit | Must operate connected, degraded, isolated and manual-safe |
| Dedicated resilience satellite constellation | Hold | Buy only unique sensing/revisit/communications gaps after federal, commercial and allied capacity is modeled |
| Airborne communications layer | Admit | Coverage-hours include launch, weather, spectrum, backhaul, power and maintenance |
| Heavy robotic construction force | Admit | Optionally crewed, locally stoppable, field repairable and integrated with engineering authority |
| Drone delivery as general logistics replacement | Reject | Payload, ground handling, weather, energy and maintenance preserve a narrower priority-cargo role |
| Autonomous lethal or coercive capability | Reject | Outside the Department's mission and civil authority model |
| Common mission-module interfaces | Admit | Interface openness must not force false containerization or one vendor's internal design |
| Proprietary-cloud-dependent critical equipment | Reject | Essential functions require disconnected and sovereign sustainment modes |

## Common architecture control

The cross-Department rules are specified in [The common resilience technical architecture](common-technical-architecture.md). The information and autonomy layer must operate across `D0` connected, `D1` intermittent, `D2` isolated and `D3` manual-safe states; carry action authority from `A0` observation through `A4` life-, rights- or irreversible decisions; and preserve identity, time, location, measurement, configuration, authority, uncertainty and outcome. It must also contain correlated fleet failure through diversity, partitions, canary updates, independent measurement, rollback and physical inhibits. A common model or signed update is not trusted merely because it is common or signed.

[^nist-deployable]: National Institute of Standards and Technology, [*Public Safety 700-MHz Broadband Deployable Systems*](https://www.nist.gov/programs-projects/public-safety-700-mhz-broadband-deployable-systems), updated March 26, 2025.
