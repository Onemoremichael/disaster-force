# Power restoration force engineering: from generator inventory to deployable utility

## Engineering judgment

The Department of Resilience should not buy a national fleet of emergency generators and call it a power force. It should field **deployable electric utilities** that can identify priority loads, isolate damaged systems, establish safe sources, form stable electrical islands, transform and distribute power, manage fuel and storage, protect people and equipment, restore or bypass grid nodes, convert electricity into thermal safety, synchronize with recovering utilities, and transfer operation without a second outage.

The key procurement object is a **Power Restoration Group** (`PRG`). Its effect is measured as:

> net critical-load megawatt-hours safely delivered at the required voltage, frequency, waveform, reliability, and point of use, plus people-hours protected inside defined thermal and air-quality envelopes.

Nameplate generation is an input. It is not the output.

This pass establishes a `PRG-100` reference formation with a maximum planning objective of **100 MW net continuous critical load**. That number is a modeling scale, not a claim that 100 MW protects a fixed population. A hospital district, water system, dense cooling-center network, industrial corridor, isolated island, or lightly damaged metropolitan network can convert the same power into very different civilian effects.

The most important design variable is not generation technology. It is the **network-reuse state**:

1. **Reuse:** safe existing substations, feeders, switchgear, protection, and building connections can carry most of the load;
2. **Bypass:** sources and loads survive, but failed nodes or corridors require mobile transformation, temporary feeders, sectionalizing, and protection; or
3. **Rebuild:** the Department must construct a substantial temporary distribution utility before generated power can reach users.

The same `PRG-100` output can therefore imply radically different mass, workforce, setup time, and operating risk. This finding should control the later model and every power-platform requirement.

## Why power restoration is a system problem

Electric service is simultaneous production, balance, network behavior, protection, and end use. At every moment:

```text
real power generated + imported + discharged from storage
    = real load served + conversion loss + network loss + storage charging
```

Reactive power, voltage, frequency, phase, fault current, inertia or synthetic response, harmonic performance, and grounding must also remain inside safe limits. A mechanical generator that can produce 1 MW on a test stand may be unable to start the intended motors, coordinate with downstream protection, energize a dead feeder, operate efficiently at the actual load, or synchronize with another source.

FEMA's critical-facility guidance treats sustained emergency power as a whole-facility design problem involving hazard exposure, system configuration, load, fuel, transfer, operation, and maintenance.[^fema1019] Sandia's microgrid design guide similarly begins with site-specific threats, outage tolerance, service priorities, existing infrastructure, and community decisions rather than a preferred technology.[^sandia-guide]

The Department must add a further complication: it enters after the site design assumptions may have failed. Drawings can be missing, switchgear submerged, relays misconfigured, fuel contaminated, grounds broken, loads altered, communications down, and responsible operators exhausted or absent. It must diagnose and reconstruct an electrically coherent system while other restoration work changes the network around it.

## The complete power mission thread

The `PRG` should contain twelve functions. A formation missing any one of them must report the dependency rather than claim complete power capacity.

### 1. Civil priority and load registry

The affected government establishes protected services and acceptable tradeoffs. The group converts those priorities into a load registry containing:

- facility or network node;
- civilian function and population served;
- `P0` no-break, `P1` survival, `P2` stabilization, and `P3` broader-recovery classification;
- real and reactive load by time step;
- maximum demand, minimum stable load, motor-starting and transformer-inrush behavior;
- voltage, phase, frequency, waveform, grounding, and power-quality needs;
- tolerable interruption and required ride-through;
- connection point, conductor, protection, isolation, and backfeed risk;
- existing emergency source, fuel, storage, and transfer equipment;
- dependence on water, communications, gas, transport, clinical systems, and staff; and
- conditions for utility acceptance and safe disconnection.

NREL's ComStock model publishes subhourly load profiles by building type, geography, and end use and can provide planning priors.[^comstock] Those priors cannot replace field measurements, single-line diagrams, operator knowledge, and the actual critical-load schedule.

### 2. Reconnaissance and electrical model

Survey teams build a living network model from utility data, drawings, imagery, field instruments, relay records, smart-meter or supervisory data, and physical inspection. The minimum model includes:

- source and load buses;
- conductor, cable, transformer, switch, breaker, fuse, relay, grounding, and sectionalizing state;
- normal and emergency ratings;
- probable fault locations and unsafe backfeed paths;
- power-flow, short-circuit, protection-coordination, motor-starting, transient, and harmonic cases;
- flood, fire, wind, ice, seismic, contamination, and access condition; and
- the current boundary between safe reusable plant and isolated damaged plant.

A schematic that shows where equipment is located is not an electrical model. Detailed modeling is the foundation for microgrid design because normal, islanded, and contingency states can behave differently.[^nrel-design]

### 3. Isolation, grounding, and work control

Before temporary power is introduced, the group must establish switching authority, lockout/tagout or equivalent work control, visible or verified isolation, grounds, arc-flash and step/touch protection, public exclusion, and coordination with line and facility crews. Energization is a licensed technical decision, not a command-timeline milestone.

The operating design must assume:

- damaged conductors can become unexpectedly energized;
- private generation and vehicle or building inverters can backfeed;
- floodwater, wet soil, debris, and damaged grounds change exposure;
- temporary topology invalidates familiar relay settings; and
- several organizations may believe they control the same device.

### 4. Source establishment

The group accepts source modules without being committed to one technology:

- reciprocating diesel, renewable diesel, natural-gas, or dual-fuel generation;
- simple- or combined-cycle turbines where size, fuel, setup, and emissions justify them;
- mobile battery and other storage systems;
- surviving hydroelectric, solar, wind, geothermal, industrial, campus, vehicle, or utility resources;
- barge-, rail-, or land-based generation;
- grid imports through a safe surviving intertie; and
- enduring nuclear or other strategic sources after their separate licensing and alternatives gates.

Every module publishes net rather than gross output, ambient derating, minimum stable load, ramp rate, start energy, black-start ability, reactive capability, fault-current behavior, fuel or energy consumption, auxiliary load, emissions, noise, cooling, maintenance interval, transport configuration, and failure modes.

### 5. Grid formation, black start, and synchronization

A dead electrical island needs at least one source able to establish voltage and frequency. Grid-following equipment cannot simply energize into a dead bus. DOE describes grid-forming inverters as capable of establishing voltage and frequency and potentially supporting black start, while grid-following inverters require an existing waveform.[^doe-unifi]

The restoration sequence is itself an engineered product:

1. verify isolation and dead-bus condition;
2. start the black-start source and its auxiliaries;
3. energize the shortest validated path;
4. establish voltage, frequency, grounding, protection, and communications;
5. pick up controlled load blocks within frequency and voltage limits;
6. start next sources while managing inrush and transient response;
7. expand or join islands only after synchronism and protection checks; and
8. transfer operational authority and eventually resynchronize with the utility.

NERC's black-start standard requires plans, facilities, personnel, source characteristics, cranking paths, switching, voltage and frequency limits, and return to normal operating authority.[^nerc-eop005] A Department formation should not displace those utility responsibilities. It should arrive with compatible modeling, test, source, controls, and staff capacity when the utility's own resources are damaged or insufficient.

### 6. Transformation, protection, and power quality

Source voltage rarely matches every load. The group needs a portfolio of:

- generator step-up and distribution step-down transformers;
- mobile substations and switchyards;
- breakers, reclosers, fuses, relays, synchronizing equipment, and sectionalizers;
- grounding and neutral systems;
- surge arresters, harmonic filters, reactive support, and power conditioning;
- metering and disturbance recording; and
- spare bushings, cables, connectors, control power, cooling, and insulating media.

The governing current relationship for balanced three-phase power is:

```text
I = P / (sqrt(3) x V x power factor)
```

At 100 MW and 0.90 power factor, approximate line current is:

| Nominal line voltage | Current carrying 100 MW |
|---:|---:|
| 13.8 kV | 4,649 A |
| 34.5 kV | 1,859 A |
| 69 kV | 930 A |
| 115 kV | 558 A |

This does not specify a conductor or substation. It demonstrates why metropolitan-scale emergency power cannot be distributed as a larger collection of low-voltage extension cords. Power must be divided among several feeders, transformed near loads, or moved at higher voltage, with fault duty and protection analyzed for the temporary topology.

DOE describes mobile transformers and substations as valuable for rapid and short-term restoration but not general replacements for permanent substations.[^doe-mobile] That distinction fits the Department: bypass equipment creates a restoration bridge while utility reconstruction proceeds.

### 7. Temporary distribution and connection

The distribution force provides:

- insulated surface cable and protected crossings for fast, bounded sites;
- temporary overhead or elevated medium-voltage feeders;
- modular poles, foundations, crossarms, conductor, arresters, grounding, and guying;
- cable bridges, trenching, duct, ramps, and fire/flood protection;
- pad- and pole-mounted transformers;
- facility quick-connect retrofits where preplanned;
- bespoke safe connections where they are not;
- sectionalizing and switching nodes;
- accessible public charging and medical-device continuity points; and
- inspection, patrol, vegetation/debris clearance, repair, and public protection.

Aerial drones may survey alignments and pull pilot line. Ground robots may handle cable, dig, place foundations, set poles, tension conductor, inspect joints, and enter hazardous areas. Neither changes the mass of copper or aluminum, transformers, poles, protection, and crossings. The productivity question is crew-and-system throughput under actual terrain and safety rules.

### 8. Storage and ride-through

Storage has at least six distinct jobs:

1. no-break bridge while a mechanical source starts;
2. P0 load ride-through during source trip;
3. grid-forming and frequency/voltage support;
4. motor-starting and transient support;
5. peak shaving so generators operate inside efficient loading bands; and
6. absorption of variable local generation.

Energy and power must be specified separately:

```text
storage energy required = protected MW x ride-through hours
                          / (usable depth of discharge x conversion efficiency)
```

For a 100 MW formation, 15 minutes at full load is 25 MWh before losses and reserve; four hours for a 20 MW P0 subset is 80 MWh. These are different missions and may require different storage architectures. “Battery-backed” without the protected load, duration, duty cycle, ambient condition, fire envelope, degradation, spare strategy, and recharge source is not a requirement.

### 9. Fuel and energy logistics

Combustion generation converts a damaged electrical network into a continuous fuel-distribution requirement. If average net heat rate is `H` Btu/kWh and the consistent fuel heat-content basis is `L` Btu per unit:

```text
daily fuel units = net MW x 24,000 kWh/MW-day x H / L
```

At 100 MW continuously and an illustrative 10,500 Btu/net-kWh heat rate, daily input is 25.2 billion Btu. At 137,000 Btu per gallon of diesel, that is approximately **184,000 gallons (696 m³) per day** before contingency, test, distribution loss, or idling. EIA defines net heat rate to include power consumed by plant auxiliaries and provides the conversion between heat rate and efficiency; its 2026 conversion reference gives 137,381 Btu per gallon of diesel.[^eia-heat][^eia-fuel]

This calculation is not a selected engine specification. It exposes the scale:

- three days of diesel at that rate is about 552,000 gallons;
- seven days is about 1.29 million gallons;
- a 30-day campaign consumes about 5.52 million gallons if the load and heat rate remain constant; and
- every blocked road, unavailable driver, damaged rack, contaminated batch, fire limit, and competing user becomes a power risk.

Natural gas can reduce liquid-fuel handling but is not “logistics free.” At the same heat input, the formation requires roughly 25,200 MMBtu/day; pressure, pipeline integrity, compressor electricity, firm contract status, local storage, and gas-electric interdependence matter. A 2023 FERC–NERC review found that black-start planning did not fully capture electric–natural-gas interdependencies and recommended joint planning.[^ferc-blackstart]

The formation must therefore track **assured energy-hours**, not storage-tank volume alone. Surviving grid imports, local hydro, renewable generation, efficiency, demand management, thermal storage, and batteries can reduce fuel burn. They cannot be credited until their availability during the design hazard is modeled.

### 10. Operations, control, and cyber-safe degraded mode

The group needs a utility operations center with:

- load and source forecasting;
- dispatch and unit commitment;
- feeder state and outage management;
- protection and switching records;
- fuel and storage state;
- weather and hazard intelligence;
- maintenance and work permits;
- operator logs and disturbance records;
- public and critical-user service status; and
- utility synchronization and transfer planning.

Connected digital control is valuable but cannot be the only safe state. Each island must support connected, communications-degraded, locally isolated, and manual-safe modes. Local protection must continue to function when wide-area communications are lost. Remote commands require authentication and positive control; loss of cloud connectivity cannot force loss of electric service.

### 11. Maintenance, spares, and reconfiguration

Continuous generation creates aggressive maintenance demand. The group needs line, substation, rotating-machine, power-electronics, storage, controls, fuel, and instrumentation maintenance; oil and coolant service; cable and connector repair; relay test and calibration; spare source modules; and depot reachback.

Maintenance must be modeled against the load schedule. Taking a 10 MW module offline is not acceptable merely because an interval is due. The formation needs enough reserve, dispatch flexibility, storage, and planned load reduction to preserve protected services while work occurs.

### 12. Utility transfer and demobilization

Temporary power is successful only if it can be removed without another outage. Transfer begins with the first survey and includes:

- authoritative as-built single-line and geographic records;
- equipment configuration, relay settings, test results, firmware, credentials, and maintenance history;
- ownership and operating responsibility;
- metering, cost, fuel, emissions, and environmental records;
- training and spare parts for the accepting owner;
- synchronization and staged load-transfer plan;
- disposition of temporary conductors, foundations, fuel systems, storage, and contaminated material; and
- restoration of streets, buildings, waterways, and sites.

## A reference PRG-100 architecture

### The effect contract

The reference formation should be able to accept a validated portfolio of up to 100 MW net critical load and create several stable islands or grid bridges. It is not required to carry every possible source, voltage, and distribution package simultaneously. It is a **force-generation family** with a common headquarters, engineering and safety system, and selectable mission sets.

Reference planning requirements:

| Parameter | Reference design question |
|---|---|
| Net load | Up to 100 MW continuously delivered after auxiliary and network loss |
| Load classes | Separate P0, P1, P2 and interruptible blocks with stated outage tolerance |
| Island geometry | One to ten electrical islands; no single geometry presumed |
| Response | P0 entry cells in hours; first island in days; full effect driven by network state |
| Endurance | 30-day initial campaign with planned rotations and transition to lower-logistics sources |
| Source mix | Technology-neutral portfolio selected by fuel, grid, site, climate, noise, emissions and duration |
| Storage | Sized separately for start, ride-through, grid formation, transients and fuel reduction |
| Voltage | Low-, medium- and selected high-voltage interfaces matched to regional classes |
| Network reuse | Reuse, bypass and rebuild cases modeled separately |
| Failure | Continue protected service after the defined source, feeder, control or fuel-route contingency |
| Transfer | Utility-compatible configuration, data, testing, training and staged withdrawal |

### Common headquarters and technical authority

Every `PRG-100` requires:

- command and civil/utility integration;
- chief electrical engineer and independent energization authority;
- load-registry and service-effects cell;
- network modeling, protection, controls, cyber, telecommunications, metering, and geospatial teams;
- switching, safety, work-control, environmental, fuel, fire, battery, and industrial-hygiene authority;
- movement, site, contracting, supply, maintenance, workforce, and responder-support staff;
- technical data and configuration control; and
- transfer and restoration-planning staff.

This permanent brain is as important as the source fleet. A collection of generators cannot safely self-organize into a temporary utility.

### Mission sets

The group draws from six mission sets.

| Mission set | Principal contents | Effect |
|---|---|---|
| Critical Facility Power Cells | 0.25–5 MW source/storage blocks, local transformation, protection, cable, quick-connect or field connection | hours-scale P0/P1 facility continuity |
| Community Grid Islands | multiple sources, storage, medium-voltage distribution, controls, service transformers and sectionalizing | 5–25 MW stable district islands |
| Regional Grid Bridge | 50–300+ MW mobile transformation, switching, reactive support, protection and source/intertie options | bypass failed grid nodes or connect surviving islands |
| Rapid Distribution System | surface cable, overhead feeder, poles/foundations, transformers, service drops, crossings and construction teams | connect source to usable loads |
| Thermal and Clean-Air Works | chillers, heat pumps, boilers where needed, air handling, filtration, thermal storage, duct or water distribution and building interface | protected people-hours rather than raw MW |
| Utility Repair and Transfer | diagnostics, components, controls, line/substation repair, commissioning, records and owner training | accelerate durable restoration and remove temporary systems |

The source fleet, storage fleet, substation fleet, line system, fuel system, and workforce must be common enough to combine but specialized enough to respect different voltage, hazard, and application classes.

## Three network-reuse configurations

### Configuration A — reuse

**Condition:** safe distribution plant and most building connections survive. The deficit is source power, a bounded number of failed devices, or an upstream interruption.

The group concentrates on load validation, isolation, source and storage deployment, a limited number of transformation points, protection settings, fuel or grid intertie, and utility operations. Existing feeders carry most of the power.

**Dominant constraints:** source and fuel availability, black start, transformer compatibility, protection, load pickup, reactive power, and utility authority.

**Force implication:** lowest construction mass and fastest path to high output. This case should not be used as the planning basis for a severe earthquake, flood, fire, or wind event unless inspection supports it.

### Configuration B — bypass

**Condition:** sources and important load clusters survive, but one or more substations, feeders, controls, or corridors do not.

The group installs mobile substations or transformers, temporary medium-voltage trunks, sectionalizing, communications, and local distribution while utility crews repair permanent plant.

**Dominant constraints:** voltage portfolio, transport geometry, site foundations and clearances, conductor route, protection, crossings, synchronism, and spare components.

**Force implication:** power-platform mass may remain manageable while electrical construction, traffic, permitting, public safety, and commissioning control the schedule.

### Configuration C — rebuild

**Condition:** extensive distribution and service infrastructure is unsafe or absent.

The group creates temporary district islands with new feeders, transformation, service points, thermal nodes, and public access. It may deliberately avoid recreating the pre-disaster topology, instead concentrating service at hospitals, water and wastewater nodes, shelters, cooling/heating centers, food and pharmacy hubs, communications, fuel, transit, and civic nodes.

**Dominant constraints:** route access; poles, foundations and cable; conductor and transformer mass; field crews; right-of-way; protection studies; building connections; public exclusion; and inspection.

**Force implication:** this is a public-works campaign, not a generation deployment. Full 100 MW effect may take weeks, and a smaller but spatially intelligent network may protect more people sooner than an attempt to recreate household service broadly.

## Electrical geometry drives the formation

### Divide load into survivable islands

One 100 MW island concentrates failure and demands larger transformation and fault management. Twenty 5 MW islands multiply sites, crews, controls, fuel drops, and synchronization tasks. The design should optimize cluster count against:

- location of protected loads;
- surviving feeder topology;
- source module size and minimum loading;
- conductor route and voltage;
- ability to shed noncritical load;
- failure consequence;
- fuel and maintenance access;
- noise, emissions, flood and fire separation;
- operator and communications burden; and
- later synchronization and transfer.

The default model should not preselect five 20 MW islands because the arithmetic is convenient. It should allow the load and damaged network to select the topology.

### Conductor loss and route length

For one three-phase segment with per-phase resistance `R` and current `I`:

```text
real conductor loss = 3 x I^2 x R
```

Resistance changes with conductor material, area, temperature, joints, and length. Lower current through higher voltage reduces loss and conductor requirement, but raises transformation, insulation, clearance, switching, protection, and technical demands. A later workbook must model feeder-by-feeder current, impedance, voltage drop, losses, fault duty, conductor mass, route, crossings, poles or cable protection, and installation tempo.

### Transformer compatibility is an industrial problem

DOE reports that distribution-transformer lead times grew from three to six months in 2019 to 12–30 months in 2023, while the United States used more than 80,000 distribution-transformer variants.[^doe-transformers] This is precisely the kind of fragmented industrial design space the Department could change.

The Resilience Arsenal should establish:

- a bounded set of multi-ratio or rapidly configurable mobile transformer families;
- common accessories, bushings, monitoring, protection, transport fixtures, and control power;
- modular high-voltage and medium-voltage switchgear;
- stocked adaptation kits for regional voltage, vector group, grounding, connector, and protection differences;
- government reference interfaces and technical data;
- multiple domestic sources for cores, conductor, insulation, bushings, tap changers, power electronics, and controls;
- transport and installation systems designed with the transformer; and
- proving grounds able to energize, overload, fault, repair, and reconfigure complete mobile substations.

The answer is not one universal transformer. It is a controlled portfolio that covers the largest share of real networks with the fewest certified configurations.

## Thermal protection is an energy mission, not an appliance list

Extreme heat, cold, and smoke make the value of a megawatt dependent on the system it serves. The power force should compare at least four strategies:

1. restore existing building cooling, heating, ventilation, filtration, and elevators;
2. create high-capacity neighborhood thermal-safety and clean-air centers;
3. deploy modular district chilled- or hot-water loops and thermal storage; and
4. move medically or functionally vulnerable people to safer buildings or regions.

The effect ledger should report:

```text
protected people-hours = sum over sites and intervals
                         (people safely accommodated x compliant hours)
```

It should also report transport access, queuing, overnight use, disability access, air quality, indoor temperature and humidity, filtration, water, sanitation, clinical support, staffing, and backup duration. A cooling center whose intended users cannot reach it or remain safely inside has low delivered effect even if the chiller operates.

Thermal systems couple electrical and building physics. For circulating fluid:

```text
thermal transfer = mass flow x specific heat x temperature change
```

Electrical input then depends on chiller, heat-pump, fan, pump, control, and distribution efficiency under actual ambient conditions. A later configuration model should use climate- and building-specific load profiles rather than an assumed number of watts per person.

## Source portfolio strategy

### Fast combustion core

Combustion sources remain valuable for initial response because they are dispatchable, transportable, understood, and can carry high load in a small site. The Department should purpose-design them for:

- parallel operation and grid formation;
- high ambient temperature, cold, altitude, salt, smoke, dust, flood splash, vibration, and repeated transport;
- low-load efficiency through modular dispatch;
- rapid service and module exchange;
- controlled noise and emissions near populated sites;
- multi-fuel capability where it produces real logistical resilience;
- integral fire detection, spill control, heat rejection, and exhaust management;
- accessible maintenance without de-energizing the whole island; and
- standardized data, protection, connectors, grounding, transport, and lifting.

### Storage as stability and logistics leverage

Storage should be purchased against defined duties, not a universal “hours” target. High-power systems may handle start and fault ride-through; energy-dense systems may protect P0 loads or shift variable generation; thermal storage may serve cooling more efficiently than electrical storage. Fire propagation, isolation, damaged-module removal, transport state of charge, thermal management, and post-incident disposal belong in the formation design.

### Local generation and demand reduction

Surviving solar, wind, hydro, combined heat and power, industrial generation, building storage, controllable loads, and vehicle fleets can be integrated after electrical and contractual validation. DOE notes that ordinary grid-tied solar generally disconnects during outages unless it has the correct inverter and storage architecture.[^doe-solar]

Efficiency is deployable capacity. Every 1 MW of continuous load safely removed avoids 24 MWh of daily generation, associated fuel or storage, conductor loss, and maintenance. The group should include rapid controls, recommissioning, temporary envelope, shading, ventilation, heat-pump, motor, lighting, and scheduling teams where they reduce service burden faster than additional generation can be deployed.

### Strategic and enduring sources

Barge-mounted turbines, grid imports, local fuel pipelines, new renewable fields, and pre-licensed nuclear water–energy platforms may become superior during long campaigns. They require different setup, site, environmental, workforce, and security systems. The `PRG` should accept their output through common electrical interfaces; it should not make any one source a prerequisite for power restoration.

## Workforce and unit composition

The deployed workforce is driven less by plant operators than by distributed inspection, electrical construction, protection, connection, fuel, maintenance, and 24-hour operations.

A complete group requires at least these occupational blocks:

| Block | Principal professions |
|---|---|
| Command and civil integration | incident leaders, utility liaisons, public administrators, tribal and community specialists, public information |
| System engineering | power-system, protection, controls, grounding, rotating-machine, power-electronics, storage, civil, structural, fire and environmental engineers |
| Load and network survey | electricians, lineworkers, substation technicians, facility engineers, metering, geospatial, data and inspection teams |
| Generation and storage operations | operators, mechanics, electricians, battery and inverter technicians, emissions and fire specialists |
| Substation and protection | transformer, breaker, relay, test, oil, controls, grounding and high-voltage technicians |
| Distribution construction | line crews, cable crews, equipment operators, pole/foundation and crossing teams, vegetation/debris support |
| Fuel and energy | terminal, quality, transport, storage, pipeline/gas liaison, spill and fire teams |
| Utility operations | dispatchers, switching authorities, outage management, forecasting, cyber, communications and data |
| Sustainment and maintenance | supply, transport, workshops, calibration, parts, contracting, responder support and waste |
| Safety and transfer | energization authority, electrical safety, industrial hygiene, environmental compliance, commissioning, documentation and training |

This pass does not assign final headcount. The network state creates at least three workforce regimes:

- **reuse formation:** operations, protection, source, fuel and bounded connection labor dominate;
- **bypass formation:** substation, cable, route, commissioning and traffic/public protection expand; and
- **rebuild formation:** line construction, building connection, inspection, material handling, logistics and replacement crews can dominate the group.

The configuration workbook should derive people from positions, shifts, concurrent sites, crew productivity, maintenance, relief, technical authority, and construction duration. A provisional range stated before route and equipment definition would be less informative than the variables that generate it.

## Deployment and theater burden

### Entry package

The first-entry package should be air-mobile where useful and contain:

- utility and civil liaison;
- electrical reconnaissance, instruments, modeling and geospatial systems;
- switching, safety, grounding and damage-assessment teams;
- communications and local power for the headquarters;
- a small number of `P0` facility cells with connection kits;
- fuel and source assessment; and
- site, route and reception planning.

Its task is to preserve immediate life-safety loads and turn uncertainty into a configuration. It should not create the illusion that the 100 MW formation is air-deployable.

### Main body

Transformers, generation, storage, switchgear, poles, conductor, cable, fuel plant, workshops, handling equipment, and construction fleets move primarily by rail, sealift, barge, and heavy road. The modal mix depends on source and network state. Hazardous battery and fuel cargo, high/wide transformers, axle limits, bridge damage, crane access, and minimum bend radius can determine routes.

### Sustainment tail

The formation imposes daily theater demand for:

- fuel or other energy;
- lubricants, coolant, filters, treatment chemicals, and emissions consumables;
- transformer and switchgear materials;
- cable, connectors, poles, foundations, grounding, arresters, relays, breakers, and fuses;
- battery thermal management and damaged-module quarantine;
- test and calibration equipment;
- replacement crews and responder support;
- waste oil, fuel, coolant, contaminated soil, damaged batteries, cable and equipment retrograde; and
- security and traffic control provided by legitimate civil authorities.

The power group should report gross generation, auxiliary use, network loss, delivered load, curtailed load, unserved critical energy, daily fuel/energy, emissions, service by tier, and expected endurance.

## Degraded modes and failure cases

The `PRG-100` configuration model should include at least these cases:

| Failure or condition | Required analysis |
|---|---|
| Loss of largest source module | frequency/voltage response, storage ride-through, load shedding, protected load retained |
| Loss of one feeder or transformer | island reconfiguration, overload, repair time, critical nodes isolated |
| Fuel route interrupted | assured energy-hours, load priority, local source integration, alternate transport |
| Gas supply or compressor power lost | dual-fuel reality, stored fuel, startup and emissions consequences |
| Storage block unavailable | black-start, transient, P0 ride-through and generator dispatch changes |
| Control network lost | local protection, manual operation, staffing and safe-state behavior |
| Incorrect or missing drawings | survey time, modeling uncertainty, energization limits |
| Flood, fire, smoke, heat, cold, wind or salt exceeds reference | derating, relocation, fire/exposure control, alternative site |
| Ground fault or protection miscoordination | fault duty, isolation zone, public and worker exposure, restoration sequence |
| Skilled crew loss or fatigue | alternate authority, shift coverage, reduced topology, replacement time |
| Utility recovers earlier than expected | synchronization, staged transfer, stranded fuel/stock and rapid demobilization |
| Campaign lasts 90 rather than 30 days | overhaul, fuel transition, spares, emissions, workforce rotation, recapitalization |

“N+1” is not an adequate degraded-mode statement unless the largest contingency, location, common dependencies, switching time, and service consequence are specified.

## Industrial architecture

The Department should create a power-restoration industrial sector with the depth of a major national-security enterprise:

- **system integrators** responsible for complete `PRG` configurations and interfaces;
- **source primes** for rugged modular generation, storage and power electronics;
- **grid-equipment primes** for configurable transformers, substations, switchgear, protection and control;
- **rapid-network primes** for poles, foundations, conductor, cable, service interfaces, construction robotics and route systems;
- **thermal-systems primes** for district and building cooling, heating, filtration and storage;
- **digital utility firms** for offline-capable operations, electrical models, protection data, cyber and field instrumentation;
- **public yards and depots** with reference designs, surge tooling, repair, test and fallback production;
- **material reserves** for conductor, electrical steel, insulation, bushings, breakers, power semiconductors and specialized fluids; and
- **allied production and export programs** built around controlled interfaces rather than proprietary lock-in.

The Department's demand could reduce the current fragmentation of transformer and temporary-power specifications, fund multi-ratio and flexible-transformer research, establish multiple production sources, and keep national test and repair capacity warm. The export product would be more than hardware: certified utility islands, deployment doctrine, training, spares, digital models, and long-term maintenance.

## Relationship to the six services

The Infrastructure Restoration Service generates and technically governs the `PRG`. Operations require habitual support:

| Supporting formation | Contribution |
|---|---|
| Land Engineering | route clearance, foundations, poles, trenching, crossings, crane pads, debris, site drainage |
| Air Response | reconnaissance, first-entry cells, critical spares, specialists, remote access |
| Maritime Response | barge generation, island/coastal movement, port power, fuel and heavy transformer transport |
| Health Protection | hospital and medical-device load definition, clinical consequence, health-facility transfer |
| Community Stabilization | cooling/heating-center access, shelter and food nodes, vulnerable-user registry, public information |
| Theater Opening Command | port, rail, road, cargo handling, staging and onward movement |
| Theater Sustainment Command | fuel, repair parts, responder support, workshops, waste and replacement flow |
| Resilience Information Group | communications, geospatial model, cyber, data exchange and public service status |

In a grid-failure campaign, the Life-Support Utilities Command may be supported. In a heat emergency, the Community Continuity Command may be supported and the `PRG` becomes one input to protected people-hours. Supported relationships change with the civilian objective.

## Quantitative model specification

The next workbook should contain at least fourteen linked sheets:

1. **Summary and gate** — case, service effect, mass, workforce, fuel, time, failure results, maturity;
2. **Controls** — load, duration, network state, topology, voltage, source mix, climate, access and contingency;
3. **Critical-load registry** — P0–P3 loads, time series, power quality, dependencies and outage tolerance;
4. **Network nodes and reaches** — buses, transformers, feeders, routes, voltage, impedance, ratings and reuse state;
5. **Power flow** — real/reactive balance, current, loss, voltage drop and loading;
6. **Source fleet** — net rating, derating, minimum load, ramp, black-start, heat rate, maintenance and mass;
7. **Storage and controls** — MW, MWh, duties, efficiency, usable fraction, thermal/fire envelope and control mode;
8. **Protection and grounding** — fault-current cases, relay/breaker portfolio, grounding, safe energization evidence;
9. **Distribution construction** — cable, conductor, poles, foundations, crossings, service points, productivity and mass;
10. **Fuel and energy** — daily demand, storage, modes, transport, routes, local resources and assured energy-hours;
11. **Thermal works** — building/site loads, systems, people-hours, power, water, air quality and access;
12. **Deployment and lift** — equipment manifest, packaging, transport class, route, handling, staging and setup sequence;
13. **Workforce and force generation** — positions, crews, shifts, relief, maintenance, rotations, school/depot overhead;
14. **Failure modes, checks and sources** — contingencies, manual-safe operation, formulas, bounds, evidence and R3 gate.

At least three controls must materially recalculate the formation:

- network state: reuse, bypass, rebuild;
- source case: liquid-fuel dominant, pipeline-gas/hybrid, surviving-grid/local-resource; and
- mission: facility continuity, district island, regional bridge, or thermal protection.

The model must not hide conductor or transformer quantities inside a generic “distribution package,” and it must not infer critical load from population alone.

## Technical maturity decision

This pass advances the conceptual architecture but does not close a hardware configuration.

| System | Prior state | New state | Reason |
|---|---:|---:|---|
| P-1 Critical Facility Power Cell | R1 | R2 | Complete facility-survey, source, storage, protection, connection, fuel, maintenance and transfer thread now defined |
| P-2 Community Grid Island | R1 | R2 | Topology, black start, grid formation, load blocks, distribution, control and synchronization requirements bounded |
| P-3 Regional Grid Bridge | R1 | R2 | Mobile transformation, voltage/current geometry, protection, reactive support and utility interface defined at concept level |
| P-4 Rapid Distribution System | R1 | R2 | Route, conductor, transformer, construction, connection, safety and inspection chain defined; quantities remain open |
| P-5 Thermal and Clean-Air Works | R1 | R1+ | Outcome metric and architecture improved, but climate/building loads, equipment and distribution remain insufficiently bounded |
| PRG-100 integrated formation | new | R2 | Effect contract, mission sets, network states, operating functions, failure library, industrial structure and model specification established |

No system reaches R3. The `PRG-100` lacks:

- a sourced critical-load archetype library and selected design mission;
- a solved electrical one-line and network topology;
- source, storage, transformer, switchgear, protection, conductor, pole and cable configurations;
- steady-state, short-circuit, transient, harmonic, motor-starting and protection studies;
- a full equipment and consumables manifest;
- verified construction, connection and commissioning rates;
- route and transport packaging;
- occupation-level shifts and rotation;
- reliability, maintenance, fuel-disruption and manual-mode results;
- thermal-load and people-access closure; and
- utility and field demonstration.

Rendering remains prohibited. A future image must show the formation's electrical topology, source/storage blocks, substations, feeders, work-control boundaries, fuel or energy flow, thermal nodes, maintenance, and supporting force—not merely an impressive generator vehicle.

## Research findings

1. A deployable power capability is a temporary utility, not a generator inventory.
2. Network-reuse state—reuse, bypass, or rebuild—is as important as megawatts and can change the formation by multiples in construction mass, labor, and time.
3. One hundred net megawatts at 13.8 kV implies approximately 4,649 A at 0.90 power factor; metropolitan emergency distribution therefore requires several feeders or higher-voltage movement, transformation, protection, and sectionalization.
4. A 100 MW continuous combustion case at an illustrative 10,500 Btu/net-kWh consumes about 184,000 gallons of diesel-equivalent per day. Fuel assurance can dominate endurance.
5. Storage jobs must be separated. Full-load 15-minute stabilization and four-hour P0 ride-through are different power, energy, safety, and logistics designs.
6. Black start is an ordered restoration process involving sources, cranking paths, switching, voltage/frequency control, load pickup, protection, staff, and return of authority—not a checkbox on a generator.
7. Transformer and voltage compatibility are force and industrial-base problems. A controlled configurable portfolio is more credible than either one universal unit or tens of thousands of utility-specific designs.
8. A rapid distribution system is a construction formation. Drones and robotics can improve survey, pilot line, handling, inspection, and exposure but do not eliminate conductor, pole, transformer, protection, grounding, crossing, and crew burdens.
9. Thermal protection may create more survival value per megawatt than broad electrical restoration, but only if building physics, clean air, transport, accessibility, water, sanitation, staffing, and safe occupancy are included.
10. The `PRG-100` should be source-neutral at formation level. Fast combustion, storage, surviving local resources, grid bridges, barges, renewables, and enduring strategic sources enter through certified interfaces according to mission conditions.
11. Power restoration is a major industrial opportunity: modular source fleets, flexible transformers, mobile substations, rapid networks, grid-forming power electronics, thermal systems, offline utility control, depots, testing, training, and exportable complete utility islands.
12. P-1 through P-4 advance to R2; P-5 remains R1+; the integrated `PRG-100` enters at R2. None is ready for rendering.

## Bottom line

If the Department of Resilience treats power with the seriousness of force projection, it will not arrive with a generator and ask where to plug it in. It will arrive with the authority, electrical model, sources, storage, substations, protection, conductors, construction crews, fuel system, operators, maintainers, thermal-service design, replacement depth, and utility-transfer pathway required to create safe electrical service across a broken network.

The next pass should turn this architecture into a configuration workbook. Its decisive comparison is not diesel versus batteries or mobile turbines versus nuclear power. It is how the complete `PRG-100` changes across **reuse, bypass, and rebuild** network states while delivering the same 100 MW net effect.

[^fema1019]: Federal Emergency Management Agency, [*Emergency Power Systems for Critical Facilities: A Best Practices Approach to Improving Reliability*, FEMA P-1019](https://www.fema.gov/sites/default/files/2020-07/fema_p-1019_final_02-06-2015.pdf), September 2014.
[^sandia-guide]: Brooke M. Garcia et al., Sandia National Laboratories, [*Microgrid Conceptual Design Guidebook*](https://www.sandia.gov/research/publications/details/microgrid-conceptual-design-guidebook-2022-2022-04-19/), SAND2022-4842R, April 2022.
[^comstock]: National Renewable Energy Laboratory, [*ComStock Analysis Tool*](https://www.nrel.gov/buildings/comstock.html), accessed September 4, 2026; public results include 15-minute building-stock load profiles by geography, building type, and end use.
[^nrel-design]: National Renewable Energy Laboratory, [*Microgrid Design Process*](https://www.nrel.gov/docs/fy13osti/57744.pdf), NREL/FS-7A40-57744, 2013.
[^doe-unifi]: U.S. Department of Energy, [*UNIFI Consortium*](https://www.energy.gov/cmei/systems/unifi-consortium), accessed September 4, 2026.
[^nerc-eop005]: North American Electric Reliability Corporation, [*EOP-005-3: System Restoration from Blackstart Resources*](https://www.nerc.com/globalassets/standards/reliability-standards/eop/eop-005-3.pdf), approved November 2017.
[^doe-mobile]: U.S. Department of Energy, [*The Benefits of Using Mobile Transformers and Mobile Substations for Rapidly Restoring Electrical Service*](https://www.energy.gov/oe/articles/benefits-using-mobile-transformers-and-mobile-substations-rapidly-restoring-electrical), August 2006.
[^eia-heat]: U.S. Energy Information Administration, [*What is the efficiency of different types of power plants?*](https://www.eia.gov/tools/faqs/faq.php?id=107&t=7), accessed September 4, 2026.
[^eia-fuel]: U.S. Energy Information Administration, [*Energy conversion calculators*](https://www.eia.gov/energyexplained/units-and-calculators/energy-conversion-calculators.php), accessed September 4, 2026; 2026 estimate of 137,381 Btu per gallon of ultra-low-sulfur distillate fuel.
[^ferc-blackstart]: Federal Energy Regulatory Commission and North American Electric Reliability Corporation, [*FERC–NERC–Regional Entity Joint Blackstart Availability Study in Texas*](https://www.ferc.gov/sites/default/files/2023-12/Blackstart%20Report.pdf), December 2023.
[^doe-transformers]: U.S. Department of Energy, [*Supply Chain and Market Analysis: Distribution Transformers*](https://www.energy.gov/oe/supply-chain-and-market-analysis), accessed September 4, 2026.
[^doe-solar]: U.S. Department of Energy, [*Solar and Resilience Basics*](https://www.energy.gov/cmei/systems/solar-and-resilience-basics), accessed September 4, 2026.
