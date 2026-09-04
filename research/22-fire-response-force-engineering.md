# Fire response force engineering: from airtanker inventory to fire-control system

## Engineering judgment

The Department of Resilience should not buy a larger collection of conventional airtankers and call it a fire force. It should field a **national fire-control system** able to find an ignition, establish decision-quality understanding, place an effective intervention before escape, build and hold control features, prevent an ember-driven community conflagration, protect populations from smoke and heat, sustain the campaign through day and night, and leave behind a verified, recoverable landscape and community.

The central acquisition object is therefore not an aircraft. It is an integrated operational effect:

> probability that a threatening ignition is intercepted before escape; protected objectives and expected loss avoided when it is not; durable fire edge controlled and verified; structures and people kept inside defined survivability envelopes; and responder exposure displaced without transferring intolerable risk to the public or environment.

Gallons dropped, flight hours, aircraft counts, acres treated, dozer miles and people mobilized are inputs. They are not success.

This pass reaches four first-principles conclusions.

1. **One fire force cannot optimize both immediate interception and extended campaigning.** The Department needs a geographically distributed **Ignition Intercept Network** (`IIN`) and a deployable **Integrated Fire Control Group** (`IFCG`). They share standards and data, but their posture, equipment, readiness and economics differ.
2. **Aviation cannot create durable control by itself.** An aerial intervention changes fire behavior for some interval and geometry. Its value depends on placement, fire interaction, follow-up ground work, line holding and verification. The unit of design is an air–ground–base mission cycle.
3. **The night is an engineering frontier, not an immutable pause.** Persistent sensing, portable airspace management, instrument-grade navigation in obscuration, optionally piloted aircraft, autonomous ground machines and robotic logistics could create a safe second shift. NASA is already testing enabling pieces, but an operational system requires substantially more integration, certification and evidence.[^nasa-acero][^nasa-second]
4. **A trillion-dollar fire portfolio should purchase discovery as well as equipment.** Clean-sheet aircraft, cooperative autonomy, new agent chemistry, robotic fireline systems, community ember shields, high-rate expeditionary bases and probabilistic fire forecasting require a 25-year experimental enterprise comparable in seriousness—not institutional form—to military research, test and acquisition.

The current U.S. system is evidence, not the design ceiling. NIFC describes a federal aviation system of roughly 200–300 aircraft, almost all contracted, spanning tankers, scoopers, helicopters, air attack, smokejumper, infrared and utility missions.[^nifc-aircraft] GAO documented a large-airtanker fleet that fell from 44 in 2002 to eight by early 2013, alongside limited evidence about effectiveness and modernization choices.[^gao-airtankers] The 2002 federal blue-ribbon review found the then-current large-aircraft system unsustainable after fatal structural failures in old converted aircraft.[^blue-ribbon] Those facts do not imply that contracting or conversion is always wrong. They demonstrate why a greenfield, peer-scale institution should derive its force from the fire-control mission rather than inherit an available-airframe market.

No rendering is authorized by this pass. It establishes force composition, equations, experimental programs and configuration questions that must exist before external geometry is credible.

## The operational object: control a coupled fire–community system

Wildland fire is not a static target. It is a moving combustion process coupled to fuels, terrain, atmosphere, suppression action, infrastructure, human movement and, in the wildland–urban interface, structure-to-structure fire. Operational decisions must therefore manage at least six linked states:

1. **ignitions:** location, cause, age, confidence and accessibility;
2. **fire behavior:** direction, rate of spread, intensity, flame length, spotting, crown activity and uncertainty;
3. **control geometry:** natural barriers, constructed line, treated edge, firing operations, water or retardant effects, breach probability and holding status;
4. **civilian objectives:** people, evacuation routes, utilities, health facilities, watersheds, housing, industry, cultural resources and ecological values;
5. **campaign capacity:** aircraft, bases, crews, machines, water, agent, fuel, maintenance, airspace, communications and relief; and
6. **secondary consequences:** smoke, heat, debris flow, erosion, water contamination, power loss, displacement and post-fire access.

NWCG fire-behavior guidance treats rate of spread, flame length, fireline intensity, spotting and arrival time as distinct decision variables; model outputs must be critiqued against observations rather than accepted as truth.[^nwcg-behavior][^wfdss] The Department's fire picture should therefore be a **versioned probabilistic estimate**, not a single authoritative perimeter.

### A time race, not a dispatch count

For each new ignition, the first governing quantity is:

```text
T_intercept = T_detect
            + T_verify
            + T_decide
            + T_launch
            + T_transit
            + T_target
```

where `T_target` ends only when the first intervention capable of changing the outcome reaches the correct place. An alert, dispatch or aircraft overhead is not an intercept.

In the simplest radial approximation, a fire spreading at effective rate `r` has area:

```text
A(t) = pi x (r x t)^2
P(t) = 2 x pi x r x t
```

Real fires are not circles and `r` is not constant. Wind, slope, fuel moisture, fuel structure, plume dynamics and spotting can make this approximation badly wrong. Its value is conceptual: area grows with the square of delay even when spread speed is constant, while perimeter grows linearly. A force that removes ten minutes from sensing but adds twenty minutes in verification, launch or target coordination has not improved interception.

The next model must represent `T_intercept` as a distribution by region, weather, base state, airspace and false-alarm environment. It must also report the fraction of ignitions for which the force arrives before a scenario-specific **escape time**, not an average response time that conceals the tail.

### Durable control, not line production

A fire edge becomes controlled only when a connected set of features prevents spread with acceptable breach probability through the decision horizon. Define:

```text
L_required(t) = reachable perimeter or control-feature requirement at time t

L_effective(t) = sum of constructed or natural segments
                 x segment continuity
                 x probability of holding
                 x verification state
```

A necessary but insufficient campaign condition is:

```text
dL_effective/dt > dL_required/dt
```

over the critical interval. If spotting repeatedly crosses the line, a natural feature is misclassified, a dozer segment cannot be held, or an aerial line delays rather than stops spread, nominal production overstates control.

Official fireline production tables show why a single rate is misleading. Published hand-crew values vary substantially by fuel type, crew type and whether the work is initial or sustained; the Forest Service's underlying research emphasized wide variation and the need for standardized measurement and probability distributions.[^nwcg-production][^usfs-production] The fire-force model must therefore sample production and hold probability by fuel, slope, method, shift, fatigue and access. It must never multiply one optimistic chains-per-hour number by a national crew count.

## Two forces, one fire-control architecture

### 1. Ignition Intercept Network

The `IIN` is a distributed readiness network intended to act while fires are still small enough for time to dominate mass. It is not a miniature campaign group parked everywhere. A regional cell contains:

- persistent and event-driven sensing;
- human verification and fire-behavior analysis;
- immediately available rapid-attack aircraft and precision rotorcraft or uncrewed equivalents;
- small autonomous and crewed ground-control teams;
- pre-surveyed water, agent, landing, access and communications nodes;
- local structure/ember protection caches;
- integrated airspace and public-safety coordination; and
- escalation authority that calls a campaign group before the local force is exhausted.

Its decisive measures are:

```text
P(intervention before escape)
P(control by specified hour | intervention)
tail response time by ignition class
false-negative and false-positive burden
crew and aircraft availability during correlated demand
```

The network should be geographically optimized against ignition likelihood, consequence, access, weather covariance and relief-base survivability. Equal spacing is not readiness. Nor is seasonal movement enough if smoke, lightning or wind creates correlated demand across several regions.

The `IIN` needs local trust and authority. Automated detection may nominate an ignition and an optimization system may recommend resources, but accountable people validate the event and approve consequential action. GAO's review of emerging detection technologies found material tradeoffs among satellites, aircraft, uncrewed systems, cameras and ground sensors; cloud, data latency, verification, interoperability and privacy all remain constraints.[^gao-detection][^gao-ai]

### 2. Integrated Fire Control Group

The `IFCG` is a joint campaign formation for escaped fires, multi-fire complexes and threatened communities. It is assembled from permanent Air Response Service, Land Engineering Service, Infrastructure Restoration Service, Health Protection Service and Joint Sustainment Command formations. A reference group should include the following battalion-scale functions; exact unit counts remain a modeling result.

| Function | Campaign effect | Core formations |
|---|---|---|
| Command, modeling and allocation | one civil priority picture, probability-weighted objectives and accountable decisions | incident integration, fire intelligence, safety, liaison, legal/environmental, allocation cell |
| Persistent sensing and airspace | continuous fire/ember/weather map and safe mixed operations | satellite/data reachback, high-altitude persistence, airborne sentinels, portable airspace nodes, communications relay |
| Rapid aerial attack | high-cycle precise action on new starts and breaches | `FA-2` squadrons, forward reload/refuel sections |
| Amphibious suppression | repeated water delivery where source geometry permits | `FA-3` squadrons, water reconnaissance and contamination control |
| Heavy aerial line | long, controlled agent placement for campaign objectives | `FA-4` squadrons, heavy-base and agent plants |
| Precision vertical action | inaccessible point attack, lift, rescue, sensor and hose support | `FA-5` rotor/VTOL squadrons with separated mission configurations |
| Ground access and line | connected control features through terrain and hazardous zones | `FG-1` mobility engines, crews, `FG-2` robotic line companies, common work machines |
| Water and agent network | source-to-nozzle/drop continuity | `FG-3` pump/relay/hose units, tanks, treatment, agent quality and environmental control |
| Community defense | prevent ember and structure-to-structure propagation | `FG-4` structure clusters, municipal structural-fire integration, evacuation-route defense |
| Smoke and thermal protection | reduce population and workforce exposure | `P-5` clean-air/cooling works, monitoring, occupational-health and public-health cells |
| Sustainment and regeneration | maintain round-the-clock output rather than peak arrival | fuel, maintenance, parts, food, rest, medical, decontamination, replacement crews, transport and depot reachback |
| Post-fire stabilization | prevent a controlled fire from becoming the next disaster | watershed, slope, debris, power, water, road and environmental teams |

The group does not replace local incident authority or prescribe one national tactic. It supplies a complete, typed force that can be placed under a lawful supported command. The Department generates and sustains the force; the incident commander or designated civil authority employs it.

### Why the two-force split matters

Interception favors distributed basing, immediate availability, small loads, rapid cycles, local knowledge and a high number of independent actions. Campaigning favors heavy throughput, robust maintenance, airspace density, large bases, deep sustainment and multi-day rotation. Combining both in one platform or organization produces predictable compromise:

- a heavy aircraft may move too slowly through alert, loading and base queues for a nearby initial attack;
- a small rapid aircraft may impose excessive sorties and base burden in a long line-building mission;
- a local crew held for national campaign duty degrades the intercept network;
- a national reserve fragmented across local events may be unavailable when a complex escapes; and
- a system sized to average seasonal demand can fail when lightning creates many simultaneous ignitions.

The readiness model must therefore protect an `IIN` availability floor while separately managing a national campaign reserve, training fleet, maintenance pool and strategic reconstitution stock.

## The aerial mission cycle

### Aircraft productivity is a closed loop

For aircraft family `a` at target `j`, one mission cycle is:

```text
t_cycle(a,j) = t_queue
             + t_load_or_scoop
             + t_taxi_and_depart
             + t_outbound
             + t_airspace_and_target
             + t_delivery
             + t_inbound
             + t_recovery
             + t_turn_inspection
```

Daily cycles are limited by the greatest binding constraint among operating hours, crew duty, aircraft endurance, maintenance, base throughput, water/agent supply, airspace capacity, visibility, wind, smoke, terrain and tactical demand. A paper aircraft with a large tank can have low delivered effect if any of these constraints lengthens the loop.

The USFS Aerial Firefighting Use and Effectiveness study classified outcomes ranging from no interaction or failed line through reduced intensity, point protection, delayed spread and halted spread. It found that effectiveness varies with aircraft, fire, objective, terrain, fuel, behavior and ground engagement.[^afue] This supports an objective-yield model:

```text
E_delivered(a,j,d) = payload(a)
                   x feasible_cycles(a,j,d)
                   x A_dispatch(a,d)
                   x Y_placement(a,j,d)
                   x Y_fire_interaction(a,j,d)
                   x Y_ground_completion(j,d)
                   x V_objective(j,d)
```

where:

- `A_dispatch` is probability the complete aircraft–crew–base system is dispatchable;
- `Y_placement` is the fraction placed at the required geometry and coverage;
- `Y_fire_interaction` is the probability and duration of the intended behavior change;
- `Y_ground_completion` is the probability that line or point protection is completed and held; and
- `V_objective` weights the civilian or ecological objective rather than the fluid volume.

This is not a literal universal unit. It is a requirement that the model retain each link instead of collapsing them into gallons.

### Drop geometry

If payload `G` is delivered uniformly at coverage level `C` gallons per 100 square feet across swath width `W` feet, a theoretical line length is:

```text
L_theoretical_ft = 100 x G / (C x W)
```

A 3,000-gallon load at `C = 4` and `W = 60 ft`, for example, has a theoretical uniform length of 1,250 feet. That is not 1,250 feet of durable fireline. Wind shear, canopy interception, evaporation, gating, terrain, aircraft path, agent properties, fire intensity, discontinuities and ground follow-up reduce realized effect. NWCG training materials explicitly identify topography, aircraft, gating, wind and fuel as drop variables and distinguish coverage levels and agent systems.[^nwcg-s270]

Clean-sheet design should instrument the drop. Flow, door state, position, attitude, wind estimate and observed plume geometry should produce an after-action coverage estimate. Ground and airborne sensors should then observe whether the tactical hypothesis was correct. Every operational delivery becomes evidence, with privacy and incident-data controls.

## Purpose-built aircraft families

The product line remains plural. No universal fire aircraft should be pursued.

### `FA-1` Persistent Fire Sentinel

`FA-1` is a system family rather than one airframe: high-altitude long-endurance aircraft, lower-altitude mapping aircraft, high-altitude pseudo-satellites and uncrewed scouts sharing calibrated sensor and data interfaces. It provides:

- multispectral and thermal detection;
- perimeter, intensity, plume, ember and weather estimation;
- communications relay and navigation augmentation;
- aircraft and ground-force common operating picture;
- post-drop and post-line assessment; and
- persistent overwatch through crew change and darkness.

The requirement is bounded by coverage-hours at stated resolution, detection probability, false alarm rate, latency, geolocation error, weather envelope, communications availability and revisit. Endurance without verified information is not persistence.

### `FA-2` Rapid Attack Aircraft

`FA-2` is optimized for the intercept clock and repeated small-to-medium precision deliveries, not maximum payload. A clean-sheet program should explore roughly 800–2,000-gallon mission modules while treating that band as provisional. Discriminating requirements include:

- alert-to-airborne time and forward-base autonomy;
- short-cycle loading, fueling and inspection;
- high hot/high climb and terrain performance;
- low-speed handling and gust tolerance with safe escape energy;
- precise variable-flow delivery rather than one fixed salvo;
- fatigue life under the actual fire-mission spectrum;
- two-pilot, reduced-crew and optionally piloted configurations evaluated separately;
- maintainability by line-replaceable modules; and
- instrumented structural and drop health.

The winner may carry less fluid than an adapted transport and still create more protected value per day.

### `FA-3` Regional Amphibious Suppressor

`FA-3` is optimized for repeated water or mixed-agent cycling from suitable water bodies. The provisional 2,000–4,000-gallon band is less important than:

- minimum safe water length, width, depth, obstacle clearance and turn geometry;
- sea-state and crosswind envelope;
- scoop intake damage tolerance and debris rejection;
- invasive-species, pathogen, salinity and chemical-transfer control;
- corrosion protection and rapid washdown;
- high-cycle hull and wing fatigue monitoring;
- on-aircraft dosing or mixing without unsafe cross-contamination; and
- basing alternatives when water geometry fails.

Water is not a free magazine. Source suitability, transit, ecological transfer and surface congestion are formation inputs.

### `FA-4` Heavy Line Builder

`FA-4` is a purpose-built campaign aircraft for long, controlled line and high-consequence point protection. The provisional 8,000–15,000-gallon exploration band must compete against multiple smaller aircraft on **delivered objective yield**, not payload prestige. The clean-sheet design space includes:

- distributed or segmented constant-center-of-gravity tanks;
- independently controlled gates and variable coverage profiles;
- active load alleviation and structural health monitoring;
- engines and flight controls optimized for repeated heavy–light cycles, turbulence and contaminated environments;
- high dispatch reliability and rapid field maintenance;
- runway, pavement, taxi, loading and escape-path compatibility;
- high-throughput loading interfaces; and
- safe operation in mixed traffic without creating an airspace bottleneck.

This program must be prepared to conclude that two aircraft classes outperform one heavy class. A large demonstrator is not an acquisition commitment.

### `FA-5` Precision Lift and Suppression Rotorcraft

`FA-5` covers hover-dependent suppression, crew and equipment insertion, rescue, sensor placement, hose support and inaccessible logistics. These missions should share components only where commonality does not create a compromised cabin, rotor, tank or certification basis. Important technologies include:

- high hot/high power margin;
- precise internal or low-drag delivery systems;
- low-downwash modes or stand-off delivery where people and structures are exposed;
- obstacle and wire sensing;
- degraded-visual-environment navigation;
- active rotor/load monitoring;
- rapid mission-module change with configuration control; and
- optionally piloted heavy-lift or expendable variants for the most hazardous intervals.

Nominal external lift is not useful lift after altitude, temperature, fuel reserve, hover power, bucket or tank drag and route constraints.

## The ground control system

### `FG-1` Wildland Mobility Engine

The Department needs terrain and interface variants rather than a single national engine. Common requirements are crew survivability, pump-and-roll stability, communications, thermal observation, water/agent metering, self-recovery, maintainability and safe evacuation. The machine should publish:

- water and agent delivered at nozzle at stated head and duty;
- pump curve, draft performance and mobile operating limits;
- grade, side-slope, turning, obstacle and soil envelope;
- radiant heat and ember protection duration;
- filtered crew-air and egress performance;
- rollover and burnover protection;
- refill cycle and water-source compatibility; and
- field repair time and recovery method.

### `FG-2` Autonomous Fireline Tractor

`FG-2` should begin as an **optionally crewed work system**, not a promise of general autonomy. A carrier family may accept dozer, masticator, excavator, rake, mulcher, plow, pump and recovery tools. Its purpose is to transfer the highest-heat, smoke, rollover and falling-object work away from people while maintaining human control over objectives and firing decisions.

Required capabilities include:

- local perception through dust, smoke, flame, darkness and vegetation;
- terrain, rollover and entrapment prediction;
- machine-readable line geometry and quality;
- supervised cooperative work among several machines;
- local safe stop and physical emergency intervention;
- operation through intermittent communications;
- remote recovery or sacrificial abandonment plan;
- protected energy storage, hydraulics, tires/tracks, sensors and compute;
- rapid tool and wear-part replacement; and
- complete action and override logs.

NIST's emergency-response robot program provides an appropriate measurement philosophy: test mobility, dexterity, sensing, endurance, communications, durability, reliability, autonomy, logistics, safety and operator proficiency with repeatable methods.[^nist-robots] The Department should build fire-specific variants of those test methods rather than accept autonomy claims from demonstration videos.

### `FG-3` Long-Reach Water and Hose System

`FG-3` is a mobile water utility for fire control. It contains source reconnaissance, intakes, pumps, treatment or debris exclusion, flexible hose and rapid pipe, booster relays, temporary storage, manifolds, monitors, hydrant interfaces, robotic placement, leak detection and recovery. Its engineering balance is:

```text
source yield >= delivered flow + leakage + refill demand + reserve recovery

total dynamic head = elevation head + friction head + minor losses + terminal pressure

shaft power = density x gravity x flow x total dynamic head / efficiency
```

As with the WRG-50 water formation, drones may survey and pull pilot lines; they do not carry away the mass of pipe, pumps and water. The fire variant trades potable quality for debris, ecological and equipment compatibility, but must prevent cross-connection and unacceptable source damage.

### `FG-4` Structure and Ember Protection System

Community defense is not simply a larger hose lay. NIST identifies radiation, direct flame, ember exposure and structure-to-structure propagation as distinct WUI pathways, with embers responsible for much structure loss.[^nist-wui-spread] A deployable system should combine:

- parcel and neighborhood exposure mapping;
- rapid clearance of critical near-structure fuels and combustible accumulations;
- temporary vent, eave, opening, deck and roof-edge protection;
- targeted wetting, mist, gel or other qualified agent delivery;
- ember-flux and heat-flux sensors;
- remote exterior inspection for incipient ignition;
- autonomous or remotely operated point suppression;
- protected local water, power and communications; and
- structure-to-structure break planning with municipal fire services.

The effect metric is `P(cluster survival | exposure class)` and population safely sheltered or evacuated—not the number of houses sprayed. Materials must be tested after ultraviolet, moisture, dirt, installation error and storage aging. A recent Forest Service study found that candidate multilayer intumescent coatings lost performance after natural weathering, illustrating why a fresh laboratory coupon is not field readiness.[^usfs-coating]

## Fire bases are combat logistics without combat purpose

### `FA-6` Fire Aviation Base System

An airtanker base is a production system with queues and shared constraints. For resource `k`:

```text
throughput_k <= min(
    loading-position capacity,
    agent-mix capacity,
    water-source capacity,
    ramp and taxi capacity,
    fuel capacity,
    maintenance release capacity,
    crew and airspace capacity
)
```

Each base configuration must state:

- aircraft families and maximum simultaneous positions;
- service-time distributions by load and agent;
- water, concentrate, mixing, test and storage capacities;
- fuel type, daily draw, resupply and protected reserve;
- pavement, runway, taxi, obstacle and emergency-response requirements;
- maintenance levels, spares, tooling, washdown and corrosion control;
- environmental containment and waste handling;
- power, communications, weather, lighting and airspace nodes;
- sleeping, food, hygiene, clinical and fatigue-management capacity; and
- degraded operation after loss of any one critical resource.

NWCG maintains separate standards for airtanker-base operations and airtanker use and coordination, reinforcing that base and airspace systems are part of aviation capability.[^nwcg-pms508][^nwcg-pms514] A future expeditionary base should add modular agent plants, autonomous ground handling, digital queue control, condition-based maintenance, high-rate safe loading and deployable water production—but each innovation must be verified against human escape paths, chemical exposure and fault containment.

### The agent is a weapon only in the engineering sense

Water, foam, gel, water enhancers and long-term retardants produce different effects and environmental burdens. A precision agent system should select chemistry and coverage for the tactical objective, mix as late as practical, record batch quality and placement, and observe the result. It must also prevent attractive but harmful substitutions.

Forest Service qualification includes product testing, toxicity and environmental review, lot acceptance and aircraft-loading quality control.[^usfs-chemicals][^usfs-retardant-seis] EPA research on fluorine-free structural-fire foams warns that removal of one problematic chemical class does not automatically make a high-surfactant formulation benign; toxicity, breakdown products and environmental fate still require testing.[^epa-foam] The fire innovation program should seek biodegradable, low-toxicity, lower-logistics agents, but claims such as “green” or “PFAS-free” are not performance or safety evidence.

## The continuous sensing and decision system

### Layered sensing

No sensor layer is sufficient alone. The Department should procure a federated sensing architecture:

1. **strategic layer:** dedicated and hosted satellite payloads, commercial and allied data, lightning and weather systems;
2. **persistent regional layer:** high-altitude aircraft and pseudo-satellites positioned for forecast risk;
3. **tactical airborne layer:** crewed and uncrewed mapping, plume sampling and communications relay;
4. **fixed landscape layer:** calibrated optical/thermal cameras and weather/air-quality stations;
5. **edge layer:** expendable heat, ember, wind, line and equipment sensors; and
6. **human layer:** public reports, crews, dispatchers, utilities, tribal and land managers, and local fire services.

Every observation carries time, location, calibration, uncertainty, provenance and access rights. The system reports disagreement; it does not hide it in a blended picture.

### The fire digital twin

The phrase “digital twin” is admitted only if it means a continuously updated ensemble of explicit models, observations and uncertainty. It should estimate:

- current and possible future fire geometry;
- arrival-time and exposure distributions for objectives;
- sensor detectability and blind areas;
- control-line completion and breach probabilities;
- aircraft cycle and base queues;
- resource exhaustion and relief times;
- evacuation-route viability;
- smoke and heat exposure; and
- consequences of alternative actions.

The ensemble may combine physics-based spread, empirical models, stochastic spotting, weather ensembles, infrastructure graphs and machine learning. Machine learning should accelerate detection, association, quality control and surrogate computation; it should not conceal rare-event uncertainty or allocate life-safety resources without review. GAO specifically identifies limited rare-event data, inaccurate outputs and continuing need for human analysts in wildfire-detection AI.[^gao-ai]

The system's forecasts must be scored after every operational period. Calibration, missed events, false certainty, action sensitivity and human overrides become institutional evidence. A model that cannot be audited in disconnected operation is advisory only.

### Safe 24-hour mixed airspace

The Department should set a 25-year objective of safe, productive operations across the full day where weather and tactics permit. This does not mean ordering current daytime aircraft to fly blind at night. It means creating a new airspace and vehicle system with:

- portable incident airspace management;
- common cooperative surveillance and authenticated identity;
- detect-and-avoid across crewed, remotely piloted and optionally piloted aircraft;
- navigation robust to smoke, terrain, lost satellite navigation and degraded communications;
- shared target, route and abort geometry;
- lost-link behaviors and protected contingency volumes;
- instrumented drop/line deconfliction;
- human-readable automation intent and manual-safe modes; and
- certification for progressively more complex operations.

NASA's ACERO program is developing portable airspace management and remotely piloted operations to extend wildfire missions into darkness and low visibility.[^nasa-acero-test] That is an enabling precedent, not a fielded national architecture. The Department should fund the missing vehicle integration, communications assurance, human factors, certification, tactics and full-scale exercises.

## Protecting people is part of fire control

Wildfire smoke is a mixture whose composition and concentration change with fuel, fire behavior and weather. NIOSH notes potential occupational exposure to carbon monoxide, particulate matter and WUI contaminants, alongside heat, exertion and long shifts.[^niosh-health][^niosh-smoke] A mature force should treat workforce and population protection as production constraints, not medical afterthoughts.

The `IFCG` therefore includes:

- personal exposure monitoring and cumulative career records;
- filtered rest, sleep, command and maintenance spaces outside the smoke plume where possible;
- work–rest, hydration, cooling and replacement capacity;
- respiratory protection research compatible with heat and exertion;
- decontamination for WUI combustion products and agent exposure;
- mobile clean-air and cooling centers with accessible transport;
- public air-quality sensing and risk communication;
- home filtration and power support for people unable to relocate; and
- clinical surveillance and referral for responders and vulnerable populations.

Thermal and clean-air effect should be counted as **people-hours inside a defined temperature and particulate envelope**, with access, occupancy and power availability measured. The power and health services can provide `P-5` modules, but the fire group owns the demand forecast and operational integration.

## An Advanced Resilience Projects Agency fire program

### Institution

The Department should use its **Advanced Resilience Projects Agency** (`ARPA-R`) and a service-level Fire Technology Directorate. `ARPA-R` pursues high-risk cross-service breakthroughs; the directorate matures mission systems, test infrastructure and acquisition programs. Neither owns operational acceptance. An independent Resilience Test and Evaluation Authority verifies safety, effect, maintainability and degraded modes.

The institutional analogy to military innovation is functional:

- stable multi-year mission funding;
- technically credible program managers with bounded tenure and authority;
- competing prototypes rather than early paper standardization;
- government-owned reference architectures, interfaces and test data;
- operational experimentation with instrumented users;
- independent developmental and operational test;
- multiple production paths and surge rights; and
- willingness to end programs that fail the effect metric.

It should not reproduce military secrecy by default. Most interfaces, safety evidence, environmental data and performance methods should be public so states, tribes, allies and commercial operators can interoperate and improve the field. Restricted information is limited to genuine security, privacy, protected ecological or infrastructure concerns.

### Ten technology campaigns

#### 1. Minutes-to-intercept

Build national detection, verification and predictive-positioning systems that reduce the complete `T_intercept` distribution. Research problems include small-fire detection under cloud and canopy, false-alarm rejection, edge processing, sensor-tasking, uncertainty fusion and pre-decision logistics.

#### 2. Fire digital twin and causal operations research

Create calibrated ensemble forecasts and learn the causal contribution of tactics rather than merely correlating activity with outcomes. Instrument drops, lines, weather, fire behavior and objectives; preserve counterfactual uncertainty; publish evaluation sets.

#### 3. Cooperative autonomy and the second shift

Develop mixed crewed/uncrewed airspace, degraded-visual navigation, safe ground autonomy, human–machine teaming, resilient communications and lost-link behavior. The objective is added safe effect-hours, not removal of people as an ideological goal.

#### 4. Clean-sheet rapid-attack flight system

Prototype several airframe and propulsion approaches optimized for alert time, forward basing, high-cycle fatigue, precision flow and dispatch availability. Compete the entire aircraft–base–crew loop.

#### 5. Clean-sheet heavy and amphibious flight systems

Explore heavy segmented delivery, load alleviation, constant-center-of-gravity tanks, corrosion-resistant scooping systems and optional piloting. Require full-scale drop grids and life-cycle fatigue articles before fleet selection.

#### 6. Robotic fireline and water network

Develop optionally crewed tractors, cooperative machines, robotic hose/pipe placement, autonomous pump relays, remote recovery and machine-readable line quality. Test in smoke, heat, dust, slope and communications loss.

#### 7. Precision agent science

Develop lower-toxicity suppressants and enhancers, on-platform mixing, real-time coverage sensing and tactical agent selection. Couple fire performance to environmental fate, corrosion, aquatic and terrestrial effects, occupational exposure, production scale and storage aging.

#### 8. Community ember shield

Develop rapidly installed, weathered and exposure-rated systems for openings, edges, decks, roofs, vegetation, local sensing and incipient suppression. Validate at parcel and neighborhood scale against realistic ember flux, wind, radiation and structure-to-structure propagation.

#### 9. Expeditionary high-rate fire base

Build modular mix, fuel, water, maintenance and traffic systems capable of predictable surge throughput. Explore autonomous ground handling and hot-loading concepts only inside a safety case that proves containment, egress and error recovery.

#### 10. Human endurance and exposure displacement

Develop heat-compatible respiratory protection, cooled and filtered mobile work/rest systems, exposure sensors, human-performance models, remote operation ergonomics and career health surveillance. Count risk transferred to remote operators, maintenance crews and nearby communities.

### Technology maturity map

| Horizon | Operationally available or integrable | Requires major engineering | Requires scientific or regulatory breakthrough |
|---|---|---|---|
| 0–5 years | multi-source detection fusion; better cameras and airborne mapping; portable airspace trials; instrumented drops; supervised ground machines; modular base pilots; clean-air/rest modules | common data architecture; confidence-calibrated twin; robust fire-specific robot tests; deployable high-rate base; community-defense kits | broad unsegregated night suppression; high-autonomy lethal-environment work without close supervision |
| 5–12 years | regional intercept cells; operational sensor constellations; second-shift reconnaissance/logistics; limited robotic line companies | clean-sheet rapid aircraft; optionally piloted suppression; coordinated robot fleets; validated new agents; neighborhood ember defense | routine dense mixed airspace in obscuration; trustworthy prediction of extreme spotting and WUI propagation |
| 12–25 years | scaled clean-sheet fleets; persistent national sensing; common allied interfaces; mature automated logistics | high-density 24-hour air–ground campaigns; adaptive agent delivery; autonomous recovery and field repair | robust control under the most extreme plume-driven fires; comprehensive community-scale ignition prediction |

The third column is not a promise. It is a portfolio of hypotheses with termination criteria.

## Proving grounds and evidence infrastructure

Military-scale innovation requires places where systems can fail safely and measurements can be trusted. The Department should operate or contract a distributed National Fire Systems Test Complex with:

1. full-scale drop grids with wind, canopy and coverage measurement;
2. flight-load and fatigue laboratories reproducing the actual mission spectrum;
3. instrumented scoop lanes and corrosion/contamination facilities;
4. smoke and degraded-navigation airspace ranges;
5. robotic terrain, rollover, thermal, perception and lost-link courses;
6. fireline production and hold experiments across representative fuels and slopes;
7. live-fire ember, radiation and structure-cluster facilities;
8. agent chemistry, environmental-fate and long-term weathering laboratories;
9. deployable-base throughput and fault-injection exercises;
10. workforce heat, smoke, fatigue and human–automation laboratories; and
11. campaign exercises that join sensing, airspace, aircraft, ground, base, health and post-fire effects.

Testing must distinguish:

- component performance;
- subsystem performance;
- integrated mission-thread performance;
- operational effect in a representative environment;
- lifecycle availability and maintainability;
- safe degraded behavior; and
- effect after operator, installation and data errors.

A spectacular prototype flight does not close any of the latter six.

## Industrial base and acquisition structure

The Department should deliberately create a civil resilience industrial sector capable of clean-sheet design, serial production, depot maintenance and export—not one vertically integrated fire monopoly. The desired structure includes:

- two or more competing aircraft design and integration houses;
- propulsion, flight-control, tank, gate, sensor and corrosion specialists;
- autonomous heavy-equipment and fire-robot integrators;
- pump, hose, rapid-pipe, water and agent suppliers;
- base-system and ground-handling integrators;
- satellite, airborne and edge-sensing firms;
- public-interest fire-model and data institutions;
- test, certification and environmental laboratories;
- regional maintenance, overhaul and training centers; and
- state, tribal, municipal and allied production/repair partners.

Government owns the mission data dictionary, safety interfaces, digital thread, test methods, integration reference and surge-production rights. Contractors can retain competitive implementation intellectual property. This prevents both total commoditization and prime-contractor lock-in.

Programs should use three acquisition lanes:

1. **experimental lane:** rapidly competed prototypes and field experiments with no production promise;
2. **mission-system lane:** incremental integration of mature components under open interfaces; and
3. **fleet lane:** independently tested, configuration-controlled systems with depot, training, spares, software, environmental and retirement plans funded from the start.

The Department should buy availability and effect where measurable, not transfer sovereign fleet design entirely to short-term service contracts. Commercial operators may remain important, particularly for surge and specialized missions, but the government needs an organic technical baseline and enduring fleet floor.

## Workforce and readiness

The force cannot sustain a 24-hour campaign by doubling a 16-hour day. NIFC's 2026 mobilization standards retain a standard 14-day assignment context and note that crew rotation—not just platform possession—can constrain helicopter continuity during high activity.[^nisrm] NIOSH describes wildland firefighting as involving heat, smoke, prolonged exertion, long shifts and repeated assignments.[^niosh-health]

Each deployable function must publish:

```text
deployed positions per shift
x shifts per day
x relief factor
x qualification pipeline factor
+ command, maintenance, logistics, medical, training and depot positions
= force-establishment billets
```

The next configuration model should use at least four personnel pools:

- incident deployed;
- immediate regional or national reserve;
- recovery, leave and medical restriction;
- training, test, depot and institutional support.

It must model scarce qualifications separately: incident aviation leadership, pilots by type, mechanics, airspace managers, agent/base specialists, fire-behavior analysts, dozer and robot supervisors, pump engineers, occupational-health staff and structure specialists. A generic “firefighter” count cannot substitute among them.

Autonomy changes this balance but does not make it zero. It adds remote operators, software assurance, sensor maintenance, cyber defense, field recovery and data staff. The honest comparison is exposure-adjusted, shift-complete effect per total institutional billet.

## Illustrative trillion-dollar fire enterprise

The following is a **capital and RDT&E thought experiment**, not an independent cost estimate, budget recommendation or claim about current wildfire spending. It asks what a 25-year, $1 trillion national investment could deliberately create if it were treated like a strategic industrial program. Annual personnel, routine operations and incident consumption are outside the table and must be modeled separately.

| Portfolio | 25-year amount | Share | What the tranche purchases |
|---|---:|---:|---|
| RDT&E and advanced prototypes | $120B | 12% | the ten technology campaigns, competing demonstrators, digital infrastructure and transition funding |
| Purpose-built aviation fleets | $250B | 25% | intercept, sentinel, amphibious, heavy and precision-lift aircraft plus initial spares and training systems |
| Ground control, robotics and water | $150B | 15% | engines, optionally crewed work machines, pump/hose/pipe systems, recovery and support fleets |
| Sensing, communications and decision systems | $100B | 10% | space/air/ground sensing, resilient networks, compute, models, data and regional operations nodes |
| Bases, water, agent and logistics infrastructure | $100B | 10% | fixed and expeditionary bases, agent plants, fuel/water systems, environmental containment and transport |
| Depots, schools, ranges and certification | $80B | 8% | overhaul, training, test complexes, fatigue articles, environmental and operational test |
| Community and critical-corridor defense | $100B | 10% | prepositioned ember-defense systems, clean-air/thermal nodes, evacuation-route and interface works |
| War reserve equivalent and reconstitution | $50B | 5% | attrition, consumable, spare, replacement and industrial-surge stock |
| Program reserve and unsuccessful pathways | $50B | 5% | uncertainty, terminated prototypes, alternate designs and schedule/cost risk |
| **Total** | **$1,000B** | **100%** | **capital and research portfolio only** |

The deliberate inclusion of unsuccessful pathways matters. A research portfolio that assumes every clean-sheet aircraft, autonomy stack or chemical program succeeds is not ambitious; it is financially unserious.

### Illustrative $120 billion RDT&E allocation

| Campaign | Amount |
|---|---:|
| Persistent sensing and minutes-to-intercept | $15B |
| Fire digital twin, causal analysis and decision science | $10B |
| Cooperative autonomy, airspace and degraded navigation | $18B |
| Clean-sheet fixed-wing and rotorcraft demonstrators | $30B |
| Robotic ground control and water networks | $18B |
| Suppressant chemistry, exposure and ecology | $8B |
| Expeditionary bases and logistics | $10B |
| Proving grounds, certification and independent test | $8B |
| Human endurance, structure protection and transition reserve | $3B |
| **Total** | **$120B** |

These round numbers expose portfolio priorities and enable later sensitivity analysis. They do not establish program costs. The next financial pass should use reference-class aircraft and infrastructure schedules, technology-risk distributions, production learning, depot and software costs, inflation conventions and independent schedule risk.

## Failure cases the force must survive

| Failure | Hidden false claim | Required degraded response |
|---|---|---|
| detection layer misses or mislocates an ignition | persistent sensing guarantees awareness | independent sensor paths, uncertainty display, human/local reporting and search patterns |
| false alarms saturate verification | detection speed equals action speed | confidence triage, regional surge analysts and protected high-consequence channels |
| weather closes one aircraft family | fleet count equals available effect | heterogeneous air/ground alternatives and protected campaign reserve |
| primary airtanker base is unusable | aircraft can operate anywhere with pavement | alternate bases, mobile agent plants, forward arming/refill concepts and explicit runway/logistics limits |
| water source is unavailable or ecologically prohibited | scoop cycle is geographically universal | land-based loading, alternate agents, ground control and water reconnaissance |
| communications fail in smoke and terrain | autonomy removes connectivity dependence | bounded local behavior, safe stop/return, preloaded plans, physical markers and human fallback |
| digital twin is confidently wrong | more computation removes uncertainty | ensemble disagreement, forecast scoring, field observation, red-team models and manual authority |
| aerial line is not held | gallons dropped equal containment | ground-completion probability, visible dependency and reassignment of objective |
| autonomous tractor is disabled in the fire area | unmanned means expendable without consequence | protected shutdown, location beacon, remote recovery and abandonment plan that does not obstruct egress |
| agent harms water, soil or responders | new chemistry is environmentally safe by label | qualification, batch traceability, exclusion zones, monitoring and alternate agent |
| base throughput collapses under surge | nominal loading time scales linearly | queue model, multiple service cells, fault isolation, reserve plant and dispersal |
| responder relief fails | aircraft or machine availability equals crew availability | independent personnel readiness, relief transport, filtered rest and mission curtailment thresholds |
| community remains after evacuation routes fail | structure defense is a property-only mission | accessible movement, shelter-in-place criteria, clean air/power and public accountability |
| post-fire rain mobilizes debris | containment ends the disaster | slope, watershed, debris, road, water and warning transition team |

## The next configuration model

Pass 12 should build an editable `IFCG` workbook rather than select an airframe. The model should contain at least:

1. `Read Me and Sources`;
2. `Controls`;
3. `Fire Cases` with ignition, spread, intensity, spotting, terrain, weather and objectives;
4. `Detection and Intercept` with full response-time distributions;
5. `Fire Growth` with low/base/high and stochastic escape cases;
6. `Aircraft Families`;
7. `Air Mission Cycle`;
8. `Drop Geometry and Yield`;
9. `Airspace Capacity`;
10. `Air Base Throughput`;
11. `Ground Line Production`;
12. `Line Hold and Breach`;
13. `Ground Robotics`;
14. `Water and Agent Network`;
15. `Structure and Ember Defense`;
16. `Smoke and Thermal Protection`;
17. `Deployment Manifest`;
18. `Workforce and Rotation`;
19. `Readiness and Concurrency`;
20. `Technology Roadmap`;
21. `Cost and RDT&E`;
22. `Failure Modes`; and
23. `R3 Evidence Gate`.

It should compare three force states:

- **intercept cell:** one region, simultaneous new ignitions, minutes-to-action objective;
- **reinforced initial attack:** several cells and a light campaign echelon managing a developing complex; and
- **IFCG campaign:** 24-hour escaped-fire and WUI defense with deep sustainment.

At minimum, model outputs must include:

- probability of effective action before escape;
- tail rather than only average intercept time;
- objective-weighted delivered aerial yield;
- effective line production, completion and hold probability;
- base, water, agent, fuel and airspace utilization;
- structure clusters and people-hours protected;
- crew exposure-hours displaced and newly created;
- aircraft, machine and base availability;
- deployed mass and strategic movement;
- shift-complete personnel and institutional billets;
- concurrent regional cells and campaign groups supportable; and
- sensitivity to loss of a base, sensor layer, communications, water source or aircraft family.

## Requirement and evidence gate

This pass advances the integrated `IFCG` to `R2` and its component families to the states recorded in the requirement register. `R2` means the mission, formation, governing relationships, major interfaces and discriminating unknowns are explicit. It does not mean the design is feasible, affordable or selected.

No fire concept reaches `R3` until evidence closes all of the following:

1. regional ignition and consequence cases with uncertainty;
2. complete detection-to-effective-action distributions;
3. fire growth and escape models calibrated to representative cases;
4. aircraft–base–crew mission cycles by family;
5. instrumented placement and fire-interaction yield;
6. line-production distributions and hold/breach behavior;
7. water, agent, fuel and base throughput balances;
8. mixed-airspace safety and degraded communications;
9. vehicle loads, fatigue, propulsion, stability and maintainability;
10. robotic perception, stop, recovery and productivity evidence;
11. structure-defense performance after realistic weathering and installation error;
12. responder and public exposure protection;
13. itemized deployment and sustainment manifests;
14. workforce qualifications, shifts, rotation and training pipelines;
15. concurrent-force availability and reconstitution;
16. environmental fate and waterway controls;
17. lifecycle cost, industrial capacity and production schedule; and
18. independent operational testing of the complete air–ground–base mission thread.

The rendering gate is downstream of these requirements. A future rendering must show the aircraft or machine inside its mission cycle: loading, sensors, crew or control station, maintenance access, water/agent path, connectors, support vehicles, safety envelope and formation. Exterior form alone would conceal the design problem.

## What this pass changes

This pass changes the Department of Resilience concept in five material ways.

- It replaces “a fire aviation program” with two operational systems: a distributed `IIN` and a deployable `IFCG`.
- It makes effective intervention and durable control the outputs, placing aircraft, bases, ground line, water, structure protection and health in one balance.
- It treats safe night and obscured operations as a major national technology campaign rather than accepting daylight as the permanent frontier.
- It gives `ARPA-R`, a fire technology directorate and independent test authority necessary roles in generating the force—not overhead added after procurement.
- It interprets a $1 trillion fire investment as an industrial and scientific transformation with deliberate prototype failure, not simply an order for more current equipment.

The next research gain comes from a configuration workbook that forces the intercept and campaign systems to close numerically. More visual description before that model would create false confidence.

## Pass 12 configuration result

The specified workbook is now complete. Its principal finding strengthens the two-force architecture: in the WUI screen, an Ignition Intercept Cell has an 81.2% modeled probability of acting before the 50-minute escape threshold but lacks the production margin to close the growing control feature, while the IFCG reaches only 33.4% before escape but produces 411.80 km/day of effective line and a +4.77 km/h closure margin. The workbook also exposes airspace, retardant, robotic-line, deployment-mass and workforce dependencies that aircraft counts alone conceal.

See [Fire response force configuration model](23-fire-configuration-model.md) and the editable [fire response force engineering workbook](../models/fire-response-force-engineering.xlsx). `IIN` and `IFCG` advance to `R2+`; all 18 evidence gates remain open and no rendering is authorized.

## Sources

[^nasa-acero]: NASA, “Advanced Capabilities for Emergency Response Operations,” accessed September 4, 2026, https://www.nasa.gov/directorates/armd/aosp/aamp-acero/.
[^nasa-second]: NASA, *Advancing Aerial Mobility for Improved Wildland Firefighting Operations*, 2024, https://ntrs.nasa.gov/citations/20240011383.
[^nifc-aircraft]: National Interagency Fire Center, “Aircraft,” accessed September 4, 2026, https://www.nifc.gov/resources/aircraft.
[^gao-airtankers]: U.S. Government Accountability Office, *Wildland Fire Management: Improvements Needed in Information, Collaboration, and Planning to Enhance Federal Fire Aviation Program Success*, GAO-13-684, August 2013, https://www.gao.gov/products/gao-13-684.
[^blue-ribbon]: U.S. Forest Service and Bureau of Land Management, *Federal Aerial Firefighting: Assessing Safety and Effectiveness*, Blue Ribbon Panel Report, December 2002, https://www.fs.usda.gov/sites/default/files/media_wysiwyg/fed.aerial.ff_.assessing.safety.effectivenss.brp_.2002.pdf.
[^nwcg-behavior]: National Wildfire Coordinating Group, “Observing Current Fire Behavior” and “Evaluating Expected Fire Behavior,” PMS 437, accessed September 4, 2026, https://www.nwcg.gov/publications/pms437/fire-assessment/observing-current-fire-behavior and https://www.nwcg.gov/publications/pms437/fire-assessment/evaluating-expected-fire-behavior.
[^wfdss]: Wildland Fire Management Research, Development and Application, “WFDSS Automated Basic Fire Behavior,” accessed September 4, 2026, https://wfmrda.nwcg.gov/wfdss-automated-basic-fire-behavior-bfb.
[^nwcg-production]: National Wildfire Coordinating Group, *Crew, Engine, and Dozer Production Rates*, 2021, https://www.fs.usda.gov/t-d/nwcg/files/NWCG_production_tables_2021.pdf.
[^usfs-production]: U.S. Forest Service, *Handcrew Fireline Production Rates—Some Field Observations*, 1982, https://research.fs.usda.gov/treesearch/27310.
[^gao-detection]: U.S. Government Accountability Office, *Wildfire Detection: Technologies and Challenges*, GAO-25-108161, 2025, https://www.gao.gov/products/gao-25-108161.
[^gao-ai]: U.S. Government Accountability Office, *Wildfire Management: Technologies for Forecasting, Detection, Mitigation, and Response*, GAO-25-108589, June 26, 2025, https://www.gao.gov/products/gao-25-108589.
[^afue]: U.S. Forest Service, *Aerial Firefighting Use and Effectiveness (AFUE) Final Report*, 2020, https://www.fs.usda.gov/sites/default/files/2020-08/08192020_afue_final_report_0.pdf.
[^nwcg-s270]: National Wildfire Coordinating Group, *Basic Air Operations, S-270 Student Workbook*, https://training.nwcg.gov/dl/s270/s-270-sw.pdf.
[^nist-robots]: National Institute of Standards and Technology, “Performance of Emergency Response Robots,” accessed September 4, 2026, https://www.nist.gov/programs-projects/performance-emergency-response-robots.
[^nist-wui-spread]: National Institute of Standards and Technology, “How Fire Spreads in the WUI,” updated September 11, 2023, https://www.nist.gov/el/fire/resources/hazard-mitigation-methodology-hmm/how-fire-spreads-wui.
[^usfs-coating]: U.S. Forest Service Research and Development, “Evaluation of multi-layer intumescent coatings for enhanced fire protection of wood: Effect of weathering,” 2026, https://research.fs.usda.gov/treesearch/81006.
[^nwcg-pms508]: National Wildfire Coordinating Group, *NWCG Standards for Airtanker Base Operations*, PMS 508, April 2026, https://www.nwcg.gov/publications/pms508.
[^nwcg-pms514]: National Wildfire Coordinating Group, *NWCG Standards for Airtanker Operations*, PMS 514, February 2026, https://www.nwcg.gov/publications/pms514.
[^usfs-chemicals]: U.S. Forest Service, “Lot Acceptance and Quality Assurance,” accessed September 4, 2026, https://www.fs.usda.gov/rm/fire/wfcs/laqa_2.php.
[^usfs-retardant-seis]: U.S. Forest Service, *Nationwide Aerial Application of Fire Retardant on National Forest System Land: Final Supplemental Environmental Impact Statement*, 2023, https://www.fs.usda.gov/sites/default/files/2023-11/AerialFireRetardant-FinalSEIS.pdf.
[^epa-foam]: U.S. Environmental Protection Agency, “Studying the Breakdown of Fluorine-Free Firefighting Foams and Their Effects on the Environment,” updated 2026, https://www.epa.gov/chemical-research/studying-breakdown-fluorine-free-firefighting-foams-and-their-effects-environment.
[^nasa-acero-test]: NASA, “Wildland Fire Tech Tested,” accessed September 4, 2026, https://www.nasa.gov/aeronautics/wildland-fire-tech-tested/.
[^niosh-health]: National Institute for Occupational Safety and Health, “Wildland Firefighter Health: Some Burning Questions,” September 28, 2020, https://www.cdc.gov/niosh/bulletin/2020/wildland-firefighter-health.html.
[^niosh-smoke]: National Institute for Occupational Safety and Health, “Wildland Fire Smoke,” updated 2026, https://www.cdc.gov/niosh/outdoor-workers/about/wildfire-smoke.html.
[^nisrm]: National Interagency Fire Center, *2026 National Interagency Standards for Resource Mobilization*, 2026, https://www.nifc.gov/sites/default/files/NICC/3-Logistics/Reference%20Documents/Mob%20Guide/2026/2026%20National%20Interagency%20Standards%20for%20Resource%20Mobilization.pdf.
