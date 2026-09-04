# Water, energy, and utility systems

## Strategic conclusion

The Department should build a coupled **water–energy–distribution architecture**. Large production platforms are technically plausible and sometimes transformative, but they are not universal answers. The binding problem often shifts from production to intake, electrical connection, elevation, pipe, storage, last-mile delivery, wastewater, concentrate, or licensed operation.

The design therefore uses a distributed ladder: small systems enter first and serve isolated users; regional systems create efficient sustained output; strategic platforms support very large coastal or river-accessible campaigns and function as national infrastructure reserves.

## Water mass and energy balance

For one million people:

| Delivered service | Water volume | Water mass | SWRO energy at 4 kWh/m³, excluding distribution |
|---|---:|---:|---:|
| 3.8 L/person/day immediate floor | 3,800 m³/day | 3,800 t/day | 15.2 MWh/day; 0.63 MW average |
| 15 L/person/day emergency target | 15,000 m³/day | 15,000 t/day | 60 MWh/day; 2.5 MW average |
| 20 L/person/day stabilized basic target | 20,000 m³/day | 20,000 t/day | 80 MWh/day; 3.3 MW average |
| 50 L/person/day expanded service | 50,000 m³/day | 50,000 t/day | 200 MWh/day; 8.3 MW average |

The Department of Energy uses roughly 3.0–4.7 kWh/m³ for seawater reverse osmosis in integrated water-energy analysis; its detailed bandwidth study uses 4.0 kWh/m³ for a conventional 50-percent-recovery RO unit and cites 2.7 kWh/m³ for an advanced operating example.[^doe-desal-energy][^doe-desal-bandwidth] Pretreatment, post-treatment, intake, concentrate management and distribution add energy and site dependence.

The table reveals two important facts:

1. desalination energy for emergency human consumption is large but not remotely beyond utility-scale generation; and
2. moving 15,000–50,000 metric tons of water every day is usually a harder logistics problem than making it.

## Pipeline feasibility

Pipe flow is approximately:

\[
Q = \frac{\pi D^2}{4} v
\]

A 0.5-meter internal-diameter line at 1.5 m/s carries about 0.295 m³/s, or 25,400 m³/day before outages and operational reserve—enough at the pipe head for roughly 1.7 million people at 15 L/day. A 1.0-meter line at the same velocity carries four times as much.

Elevation is consequential. Ideal pumping power is:

\[
P = \frac{\rho g Q H}{\eta}
\]

Moving 25,400 m³/day through 100 meters of total dynamic head at 75 percent efficiency requires about **0.385 MW**, not 4 MW as an earlier draft stated. For a 100-kilometer, 0.5-meter internal-diameter line at 1.5 m/s and an assumed Darcy friction factor of 0.015, friction adds about 344 meters of head; with 100 meters of static lift, pump power is approximately 1.71 MW before minor losses, surge allowance and local distribution. A coastal plant can therefore make emergency water with modest power relative to a reactor, while route length, diameter, elevation, pressure zoning and damaged networks determine the delivery burden. Pass 6 develops the corrected balance and complete water formation in [`17-water-system-engineering.md`](17-water-system-engineering.md).

### Verdict on drone-laid pipe

An aerial-drone fleet can survey the route, map hazards, deliver sensors and fittings, pull pilot lines, and guide alignment. It cannot efficiently carry the mass and withstand the reaction forces of a high-throughput main.

The credible architecture is:

- autonomous survey aircraft and ground rovers;
- uncrewed or optionally crewed route-clearance and trenching machines;
- distributed reels or rigid pipe modules moved by ground vehicle, barge or heavy lift;
- robotic jointing, anchoring, pressure testing and leak detection;
- booster-pump and storage nodes placed from a hydraulic model; and
- human technical authority for routing, water rights, crossings, energization and safety.

For the first days, above-ground flexible lines trade durability and protection for speed. Enduring stabilization shifts to semi-rigid or rigid mains with protected crossings and maintainable joints.

## Water system family

### W-1 Point Water Cell

**Role:** first entry, isolated neighborhoods, clinics, shelters and reconnaissance of source quality.

**Concept band:** 50–1,000 m³/day per cell depending on source; pallet to small-trailer scale; multibarrier configurable treatment; bladder or rigid storage; local laboratory; dispensing and tanker-fill points.

**Design features:** interchangeable pretreatment, membrane and disinfection stages; low-power safe mode; raw, potable and residual circuits physically keyed; telemetry that works offline; two-team operation; common consumables.

EPA's Water on Wheels system demonstrates the value of configurable mobile treatment, alternative power and compact deployment, and also highlights a non-hardware delay: many states lack a preapproval path for short-term emergency drinking-water systems.[^epa-wow] The Department would certify its W-1 family nationally before incidents.

### W-2 Regional Water Works

**Role:** stabilize a city sector, island, large shelter network or damaged utility zone.

**Concept band:** 5,000–50,000 m³/day in parallel 2,500–10,000 m³/day trains; brackish, fresh, seawater and contaminated-source variants.

**Formation:** intake and source-protection group; treatment trains; laboratory; storage; high-lift pumps; pipe and tanker distribution; wastewater/residuals; maintenance; operator replacement.

**Transport:** road/rail/roll-on-roll-off modules, with heavy pumps and tanks accepted where container limits reduce lifecycle efficiency.

### W-3 Strategic Water Works

**Role:** produce 50,000–250,000+ m³/day for a major coastal, island or river-accessible campaign; supply regional networks and smaller distribution cells.

This is a plant complex, not a single “desalination box.” It includes redundant intake, pretreatment, RO or hybrid treatment, remineralization, disinfection, laboratory, product storage, concentrate system, electrical plant, workshops, spares and shore connection.

IAEA studies have described floating desalination ranges of approximately 20,000–120,000 m³/day for multi-effect distillation and up to 250,000 m³/day for floating RO, including temporary-demand use.[^iaea-floating-desal] Those values establish physical plausibility, not readiness or cost for a disaster force.

### W-4 Rapid Water Grid

**Role:** connect W-1 through W-3 production to storage, critical facilities, distribution zones and repaired utility networks.

The family includes:

- flexible 100–500 mm rapid mains;
- larger semi-rigid and rigid pipeline sets;
- road, rail, river and structural crossing kits;
- booster stations and pressure-control nodes;
- modular reservoirs, bladders and elevated storage;
- tanker and container fill systems;
- metered public distribution points; and
- autonomous inspection and leak localization.

The acquisition unit is **delivered m³/day over a stated route profile**, not kilometers of pipe.

### W-5 Wastewater and Residuals Works

**Role:** prevent water supply and shelter expansion from creating an untreated-waste crisis.

Variants provide lift-station bypass, sewer isolation, modular biological treatment, disinfection, sludge dewatering, medical-waste interfaces and concentrate management. Water and wastewater formations deploy together unless an assessed local system can accept the load.

## Nuclear water–energy platforms

### Technical feasibility

Nuclear cogeneration and desalination are not speculative physics. IAEA documentation includes long operating experience with nuclear desalination and designs coupling small reactors to tens of thousands of tons per day of potable-water output.[^iaea-cogen] The NRC states that maritime nuclear reactors and floating nuclear power plants can be licensed under existing reactor frameworks, while acknowledging distinct maritime regulatory questions and coordination with the Coast Guard.[^nrc-maritime]

### Operational constraint

A reactor is not a generator trailer. Site hydrology, geology, seismic and flood conditions, emergency planning, security, cooling, grid or load behavior and environmental impacts are part of licensing.[^nrc-siting] A vessel cannot sail into an uncharacterized disaster port, tie up beside a displaced population and begin nuclear operation as if site approval were an electrical connector.

The operational concept must therefore use **pre-licensed operating envelopes and receiving sites**:

- protected home and regional stations;
- surveyed anchorages or moorings with exclusion, security and emergency arrangements;
- standardized shore power and water manifolds;
- pre-modeled intake, discharge, thermal and weather conditions;
- tug, salvage and storm-escape plans; and
- conventional backup capable of safe shutdown and continued critical water service.

### N-WEP: Nuclear Water–Energy Platform

**Role:** an enduring strategic reserve and global stabilization base, not first-wave entry.

**Initial concept band:** 100–300 MWe net export capability; 50,000–250,000 m³/day configurable water output; independent hospital, command, communications, workshops, aviation/boat support and crew accommodation; multiple shore connection points.

**Preferred architecture:** purpose-built floating power and process platform or ship, with physical separation between the nuclear island, public water train, hospital and cargo functions. Separation prevents one contamination, maintenance or licensing boundary from disabling the entire mission.

**Design question:** whether propulsion and process power should share one reactor system. Shared propulsion improves mobility but complicates certification, maintenance and port operation. A towable or self-propelled low-speed platform with a dedicated power plant may be superior to a high-speed nuclear ship. Both remain options pending mission and lifecycle comparison.

### Why nuclear is not automatically optimal

At 4 kWh/m³, a 100 MWe source could theoretically support 600,000 m³/day if desalination were the only load and all systems were ideal. Real mission demand includes pumping, critical grid support, hotel load, maintenance reserve and reliability. This large energy margin means the business case for nuclear rests less on RO energy than on:

- months-to-years endurance without fuel convoys;
- simultaneous grid, water, hospital and industrial support;
- forward global presence and assured national availability;
- high capacity in territories with constrained fuel infrastructure; and
- peacetime utilization sufficient to justify nuclear crew and maintenance systems.

Where a repaired grid, barge-mounted gas turbine, land microreactor, renewable-storage microgrid or conventional power ship can meet the effect faster and more cheaply, nuclear should not be selected for symbolism.

## Power system family

### P-1 Critical Facility Power Cell

**Role:** safe power for hospitals, water plants, shelters, communications, fuel and emergency services.

**Concept band:** 250 kW–5 MW; storage-backed; grid-forming; configurable AC/DC; integral protection, transformer and cable; hybrid diesel/gas/renewable variants; remote monitoring with manual control.

The module begins with a load and protection survey. It is rated in **net critical-load MW at required power quality**, not engine capacity.

### P-2 Community Grid Island

**Role:** energize a connected cluster of critical and community loads.

**Concept band:** 5–50 MW; multiple generation and storage modules; sectionalizing, switchgear, feeder repair, demand control, cyber-secure controller and synchronization.

DOE research shows that microgrids and distributed resources can support island operation and black start, but restoration requires coordinated generation, load, controls, protection and timing.[^doe-microgrid] The system is therefore a deployable utility formation rather than a generator fleet.

### P-3 Regional Grid Bridge

**Role:** temporary 50–300+ MW generation, substation replacement, black-start support and interconnection between surviving grid islands.

Components include turbine, reciprocating, fuel-cell or other generation; high-voltage switchyard; mobile transformers and substations; protection and control; grid-forming storage; fuel or energy supply; and utility command interface.

### P-4 Rapid Distribution System

**Role:** rebuild low- and medium-voltage service and selected transmission paths.

The family includes standardized poles and foundations, insulated and bare conductor variants, modular switchgear, pad and pole transformers, mobile substations, protection packages, service drops and cable bridges.

Autonomous aircraft pull pilot lines and survey alignment. Ground systems set poles or towers, tension conductors, establish grounding, inspect clearances and repair faults. Energization remains under licensed technical control.

### P-5 Thermal and Clean-Air Works

**Role:** translate energy into human survival more efficiently than universal electrical restoration.

Systems provide district or facility cooling/heating, high-efficiency heat pumps, chilled/hot-water distribution, clean-air shelters, filtration, thermal storage and building envelope repair. Effect is measured in people-hours within safe thermal and air-quality bands.

## Fuel architecture

Fossil-fueled systems remain valuable for rapid entry but create a continuing logistics obligation. Every concept reports:

- liters or mass per net MWh;
- storage and daily convoy demand;
- fuel quality and multi-fuel limits;
- spill and fire risk;
- maintenance interval;
- exhaust and noise burden near shelters and hospitals; and
- transition path to grid, pipeline, renewable or nuclear supply.

The Arsenal should use storage and renewable generation to reduce fuel burn and protect ride-through, not claim that batteries alone solve months of high-power demand.

## Requirement verdicts

| Concept | Verdict | Reason |
|---|---|---|
| Drone-surveyed and robot-installed emergency pipeline | Admit | Credible if drones handle information/light line and ground/marine systems handle mass, joints, pumps and crossings |
| Floating strategic desalination | Admit | Technically grounded; distribution and residuals must be co-designed |
| Nuclear water–energy platform | Admit to concept study; hold at alternatives gate | Plausible for pre-licensed enduring coastal/global service; must outperform non-nuclear portfolios and is not spontaneous incident entry |
| Rapid mobile nuclear reactor to arbitrary disaster site | Hold | Licensing, site, security, heat rejection and timeline presently conflict with R1–R3 response |
| Generator-only power fleet | Reject | Does not include load assessment, connection, protection, fuel, distribution or transfer |
| Networked critical-load microgrid family | Admit | Directly addresses the delivered-power requirement and supports black start |

[^doe-desal-energy]: U.S. Department of Energy, [*Capturing the Benefits of Integrated Resource Management for Water and Electricity Utilities and Their Partners*](https://www.energy.gov/sites/prod/files/2016/05/f32/Capturing%20the%20Benefits%20of%20Integrated%20Resource%20Management%20for%20Water%20%26%20Electricity%20Utilities%20and%20their%20Partners.pdf), 2016.
[^doe-desal-bandwidth]: U.S. Department of Energy, [*Bandwidth Study on Energy Use and Potential Energy Savings Opportunities in U.S. Seawater Desalination Systems*](https://www.energy.gov/sites/default/files/2017/12/f46/Seawater_desalination_bandwidth_study_2017.pdf), 2017.
[^epa-wow]: U.S. Environmental Protection Agency, [*Water-on-Wheels Mobile Water Treatment System*](https://www.epa.gov/emergency-response-research/water-wheels-mobile-water-treatment-system-wow-cart), updated June 25, 2026.
[^iaea-floating-desal]: International Atomic Energy Agency, [*Non-electric Applications of Nuclear Energy*](https://www-pub.iaea.org/MTCD/Publications/PDF/te_0923_scr.pdf), IAEA-TECDOC-923.
[^iaea-cogen]: International Atomic Energy Agency, [*Opportunities for Cogeneration with Nuclear Energy*](https://www-pub.iaea.org/MTCD/publications/PDF/P1862_web.pdf), Nuclear Energy Series NP-T-4.1, 2019.
[^nrc-maritime]: U.S. Nuclear Regulatory Commission, [*Maritime Nuclear Applications*](https://www.nrc.gov/reactors/new-reactors/advanced/modernizing/maritime-nuclear-apps), updated July 23, 2026.
[^nrc-siting]: U.S. Nuclear Regulatory Commission, [*Nuclear Power Plant Licensing at Brownfield and Retired or Retiring Fossil Fuel Sites—Considerations for Applicants*](https://www.nrc.gov/reactors/new-reactors/advanced/new-app/general-guidance/brownfield), updated August 2026.
[^doe-microgrid]: U.S. Department of Energy, [*Solar Integration: Distributed Energy Resources and Microgrids Basics*](https://www.energy.gov/cmei/systems/solar-integration-distributed-energy-resources-and-microgrids-basics), accessed September 4, 2026.
