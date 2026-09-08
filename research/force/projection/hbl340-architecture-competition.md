# `HBL-340` architecture competition

## A ground-coupled hybrid-lift system for strategic civil force projection

- **Research status:** requirements competition; behavior model only
- **Decision:** retain `H2 GCH-340` as the provisional universal research reference
- **Admission:** none; all seventy representative evidence gates remain open
- **Rendering:** blocked
**Quantitative companion:** [`hbl340-architecture-competition.xlsx`](../../../models/force/projection/hbl340-architecture-competition.xlsx)

## 1. Executive judgment

The `HBL-340` requirement cannot be satisfied by scaling a conventional cargo airship until it carries 340 tonnes. The governing physical problem occurs after arrival: the cargo leaves but the vehicle's buoyancy does not. A fully buoyant carrier that unloads a complete `HBL-340` payload can become hundreds of tonnes positively buoyant at the exact moment when it is closest to damaged terrain, people and improvised infrastructure.

Four clean-sheet architectures were therefore competed against the same payload, range, receiver, weather, time, reset and industrial requirements. Only one closes every declared behavior screen without assuming prepared anchors, imported ballast, intact destination cranes or a second heavy transport system at the receiver. The provisional reference is `H2 GCH-340`, a **ground-coupled hybrid lifting body** deliberately underbuoyant while loaded. Static helium lift carries about 71 percent of gross departure mass; aerodynamic lift closes the remaining cruise burden; a distributed landing system transfers that same burden into weak ground during unloading; and sixty tonnes of internal buoyancy authority controls the much smaller positive-lift state after the payload leaves.

This is not a zeppelin with a larger cargo bay. It is a new strategic transport category:

- approximately 1,003 tonnes at loaded departure;
- an 850,000-cubic-metre lifting volume;
- a 305.9-metre equivalent length and 72.8-metre equivalent diameter before real structural shaping;
- 350 tonnes of maximum aerodynamic-lift capacity;
- 144 megawatts of installed propulsion across twelve pods;
- 1,575 megawatt-hours of segmented onboard energy;
- sixty square metres of distributed ground contact;
- twenty isolated lift cells, six energy buses and twelve contact sectors; and
- a declared 142-hour concurrent reset critical path.

At the national force boundary, forty-three ready atmospheric pairs require eighty-six operational vehicles, eighteen reserve vehicles and eight development or test articles: 112 clean-sheet aircraft in total. The architecture-specific `HBL-340` program is $932.25745 billion over twenty-five years. Replacing the generic liftship account in `DCP-2` raises that reinforcement package from $933.2764 billion to $1.51723385 trillion and the associated national comparator from $8.31641795 trillion to $8.9003754 trillion.

These numbers are not estimates of a known aircraft. They are disciplined design hypotheses used to expose the institution, technology, industrial base and test program that a real Department of Resilience would have to create. The selection is provisional and behavioral. It authorizes deeper research, not procurement, readiness credit or exterior rendering.

## 2. The decision inherited from `DCP-2`

The preceding [`DCP-2` physical configuration](tafg1-dcp2-physical-configuration.md) fixes the payload rather than the vehicle. Each atmospheric carrier must accept two governed dry blocks and two segregated wet packs:

| Requirement | Value |
| --- | ---: |
| usable payload rating | 340 t |
| assigned mission payload | 317.5 t |
| usable cargo cube | 1,400 m³ |
| usable load deck | 352 m² |
| one-way design range | 4,000 km |
| inherited origin release and load | 16 h |
| carrier transit and placement ceiling | 18 h |
| receiver service build | 8 h |
| relative public-service ceiling | 42 h |
| receiver clear area | 420 × 420 m |
| receiver bearing floor | 60 kPa |
| maximum public transfer | 4 h |
| return-to-certified-load ceiling | 168 h |

The vehicle must preserve load order, custody, hazard separation, offline configuration, balance and independent public-service release. It must place the payload at an unprepared receiver under damaged-region conditions without borrowing a decisive capability from the terrain cell. The carrier is one part of a two-mode assurance formation, not a standalone logistics asset.

The competition adds physical questions that a payload rating cannot answer: tare mass, lift regime, offload transition, structure, propulsion, energy, weather, landing, emergency recovery, base size, workforce, production, cost and representative proof.

## 3. The governing contradiction is unloading

The declared hot-high buoyant mass coefficient is:

```text
[(1.225 kg/m³ air − 0.179 kg/m³ helium) × 0.80 density factor] / 1,000
= 0.0008368 tonnes per cubic metre
```

A fully buoyant architecture sized around a thousand-tonne vehicle therefore needs more than a million cubic metres of lifting volume. That is demanding but not conceptually surprising. The discontinuity appears when 340 tonnes of payload is removed.

For a conventional buoyant carrier:

```text
loaded equilibrium: static lift ≈ dry vehicle + payload
after unloading:     static lift ≈ dry vehicle + 340 t excess
```

The receiver must then provide some combination of downward aerodynamic force, gas compression, gas loss, water or solid ballast, tether reaction, ground contact or immediate replacement cargo. Each answer changes the formation:

- **gas venting** consumes a strategic lifting medium and creates a replenishment chain;
- **internal compression** requires machinery, containment, heat management and structural mass proportional to the authority demanded;
- **water ballast** assumes a source, quality tolerance, pumping rate and receiver access that may not exist;
- **prepared anchors** convert a supposedly unprepared receiver into fixed infrastructure;
- **external ballast** imports nearly another payload and creates a circular logistics problem;
- **aerodynamic downforce** demands power and control in the most hazardous low-altitude state; and
- **airborne winching** keeps the vehicle exposed to wind while concentrating a large suspended load over the receiver.

The architecture contest therefore treats **universal transfer** as a hard gate. A carrier receives that label only if it can unload within the declared receiver without external ballast, prepared anchors or intact heavy infrastructure. Conditional transfer remains useful, but it cannot carry the universal `DCP-2` claim.

## 4. Four clean-sheet rivals

| ID | Architecture | Governing mechanism | Gross mass | Hot-high static lift | Universal offload gap | Receiver / weather result | Decision |
| --- | --- | --- | ---: | ---: | ---: | --- | --- |
| `H1` | `VBC-340` rigid variable-buoyancy monohull | full static lift plus large gas-compression plant | 1,150 t | 1,213.36 t | 123.36 t after 280 t internal authority | too long; declared weather miss | fail |
| `H2` | `GCH-340` ground-coupled hybrid lifting body | partial static lift, aerodynamic cruise lift and distributed landing reaction | 1,003 t | 711.28 t | 0 t after 60 t internal authority | passes declared geometry, bearing and weather screens | **provisional reference** |
| `H3` | `TGC-340` twin-hull buoyant gantry | two buoyant hulls and suspended transfer gantry | 1,276 t | 1,380.72 t | 324.72 t | too long and wide; declared weather miss | fail |
| `H4` | `DBX-340` detachable ballast-exchange carrier | full static lift and separable payload pod | 1,117 t | 1,188.256 t | 331.256 t universally; 0 t with 340 t external ballast | geometry fits; declared weather miss | conditional transfer only; universal fail |

All four rivals close the declared gross-lift reserve and onboard-energy arithmetic. That does not make them equivalent. `H1` and `H3` fail at the receiver because their remaining internal authority cannot absorb the unloaded lift. `H4` closes only by capturing 340 tonnes of external ballast, meaning its apparent transport gain depends on another complete destination logistics chain. `H2` changes the state transition itself.

The result should not be read as a general proof that hybrid lift is superior. It is a proof about this mission grammar: a very heavy payload, long range, unprepared receiver, weak ground, strict time, no external ballast and complete unloading. A prepared coastal terminal or a cyclic freight route with guaranteed replacement cargo could rationally select another architecture.

## 5. The `GCH-340` physical reference

### 5.1 Lift regime

The selected reference is deliberately underbuoyant at loaded departure:

| Quantity | Value |
| --- | ---: |
| dry operating mass | 663 t |
| design payload | 340 t |
| gross departure mass | 1,003 t |
| static hot-high lift | 711.28 t |
| static share of gross mass | 70.915% |
| aerodynamic lift required in cruise | 291.72 t |
| maximum aerodynamic-lift capacity | 350 t |
| total lift capacity | 1,061.28 t |
| total-lift reserve | 5.81% |

The architecture does not hover freely at full load. It takes off and remains airborne only while the aerodynamic system supplies the difference between static lift and gross mass. That makes low-speed control, distributed propulsion, abort logic and landing contact primary systems rather than secondary details.

After unloading, the 663-tonne dry vehicle sits beneath 711.28 tonnes of static lift. The resulting 48.28-tonne positive-lift state is inside the declared sixty-tonne internal buoyancy authority. The machinery is still unprecedented at this scale, but the architecture reduces its required authority by roughly an order of magnitude compared with a fully buoyant payload transition.

### 5.2 Equivalent envelope

The workbook converts volume to a first-order prolate reference using aspect ratio `AR = 4.2`:

```text
equivalent diameter = [6V / (π × AR)]^(1/3) = 72.84 m
equivalent length   = AR × diameter          = 305.94 m
```

Those are bounding calculations, not an exterior design. A real vehicle may use a flattened lifting body, multiple lobes, a deep structural keel, integrated control surfaces, distributed landing bays and non-ellipsoidal cargo volumes. The 305.9-by-72.8-metre result establishes scale and receiver compatibility; it does not stabilize a shape for rendering.

Twenty independently isolatable lift cells are the provisional fault-containment grammar. Their geometry, pressure regime, load path, inspection access and relationship to the cargo keel remain open design questions. The primary structure and envelope are allocated 245 tonnes in the mass statement. Failure to realize that mass, while retaining damage tolerance and field repair, defeats the architecture.

### 5.3 Propulsion, aerodynamic lift and energy

The inherited 4,000-kilometre mission inside the atmospheric clock forces a 240-kilometre-per-hour cruise. At the declared reference condition:

```text
speed                            66.67 m/s
design air density               0.980 kg/m³
equivalent frontal area          4,167.45 m²
hull drag coefficient            0.050
propulsive efficiency            0.780
parasite power                   38.785 MW
aerodynamic lift power           20.383 MW
hotel and mission power           8.000 MW
cruise power                     67.168 MW
```

The aerodynamic-lift power term uses a declared lift-to-drag ratio of twelve. This is a research assumption with enormous leverage. It must be replaced by full-scale aerodynamic evidence, including control authority, gust response, icing and propulsion–hull interaction.

Twelve propulsion pods provide 144 megawatts installed. One pod represents twelve megawatts, leaving 132 megawatts after a single loss—above the eighty-megawatt placement demand. Six isolated energy buses contain a declared 1,575 megawatt-hours. Cruise and placement consume:

```text
67.168 MW × 16.667 h + 80 MW × 1.25 h
= 1,219.473 MWh
```

The resulting energy reserve is 29.15 percent before detailed route, degradation, thermal-management and emergency-diversion distributions. The energy system is not presumed to be a scaled battery. The force requirement is technology-neutral: electrochemical, fuel-electric, superconducting distribution, high-temperature generation or another architecture may compete, provided it satisfies mass, thermal, casualty, safety, turnaround and industrial-lineage constraints.

The mass statement allocates 105 tonnes to mission energy. Supplying 1,575 megawatt-hours inside that line implies fifteen kilowatt-hours per kilogram of onboard energy mass before a more conservative accounting of tanks, containment and thermal protection. A conventional battery-only interpretation therefore fails the declared architecture. The reference implicitly demands a high-specific-energy fuel-electric or comparably radical generation system, with conversion equipment carried in the separate 105-tonne propulsion allocation. Representative tankage, crashworthiness, fire isolation, boil-off or exhaust, refueling rate and lifecycle supply must either close that boundary or force more volume, mass and cost into the vehicle. This is precisely the kind of contradiction the Department's research enterprise is meant to acquire rather than assume away.

### 5.4 Ground-coupled transfer

On contact, the same 291.72 tonnes previously supplied by aerodynamic lift becomes ground reaction. Sixty square metres of distributed contact produce:

```text
291.72 t × 9.81 kN/t / 60 m² = 47.70 kPa
```

That leaves 12.30 kilopascals of declared margin to the receiver's sixty-kilopascal bearing floor. The contact system may ultimately be an active air cushion, a multi-foot walking arrest system, distributed tracked bogies or a hybrid of them. The competition selects the required behavior, not the mechanism.

The transfer sequence is provisional:

1. the receiver establishes a 420-by-420-metre controlled zone and a four-kilometre degraded-navigation approach lane;
2. the vehicle approaches with aerodynamic lift carrying the loaded deficit;
3. distributed contact progressively accepts ground reaction while active propulsion controls yaw, gust and rebound;
4. the vehicle completes structural arrest before cargo release begins;
5. unloading follows the signed service-dependency order while the buoyancy system tracks changing mass;
6. after the payload leaves, internal authority cancels the 48.28-tonne positive-lift state; and
7. the vehicle either departs empty under a new lift schedule or enters controlled recovery.

The force therefore needs a receiver landing-control profession independent of the flight deck. Vehicle safety and public-service release remain separate authorities.

## 6. Weather, emergency and failure behavior

The reference carries declared—not demonstrated—capability thresholds of thirty-two metres per second station wind, forty metres per second gust and 120 minutes of protected icing. The inherited receiver requirements are thirty, thirty-eight and 120 respectively. Meeting arithmetic thresholds earns no readiness credit.

The architecture distributes critical functions across twelve propulsion pods, six energy sectors, twenty lift cells, twelve contact sectors and three local control lanes. Sixteen failure worlds test representative internal cuts, network denial, crew casualty, receiver conditions and whole-mode loss. Fifteen retain a public effect in the behavior model. Loss of the atmospheric path transfers the `DCP-2` mission to the independently governed terrain cell. Simultaneous denial of both atmospheric and terrain modes remains outside the present guarantee.

This distinction prevents a common analytical error. Internal fault tolerance can preserve the vehicle; formation diversity can preserve the public mission after vehicle loss. They are different layers of resilience. `GCH-340` does not have to survive every conceivable failure if `DCP-2` retains a physically independent service path, but a minor pod or cell casualty should not consume that strategic reserve.

Emergency landing and recovery remain open. A vehicle more than 300 metres long cannot assume an ordinary alternate airport, commercial tow fleet or improvised hangar. The program must create degraded alternates, mobile structural stabilization, segmented energy isolation, heavy tow and recovery systems, field lift-cell repair and a national route for returning damaged articles to depot.

## 7. Reset and campaign tempo

The selected carrier must return to a certified load state within 168 hours. Five workstreams run concurrently:

| Workstream | Declared path | Margin to ceiling |
| --- | ---: | ---: |
| structure, envelope and lift cells | 142 h | 26 h |
| propulsion, energy and thermal system | 126 h | 42 h |
| distributed contact and cargo system | 126 h | 42 h |
| crew, autonomy and mission-state reconstruction | 40 h | 128 h |
| receiver and atmospheric-base handback | 94 h | 74 h |

The structure and lift-cell path governs. Its declared clock contains shutdown and isolation, recovery and handback, decontamination, sixty-four hours of inspection, thirty hours of repair allowance, and fourteen hours of recertification and reload.

This model assumes uncongested parallel work on one returning article. A mature force model must add fleet queueing, depot casualty, scarce inspection equipment, structural-repair distributions, cannibalization rules, contaminated returns and overlapping campaigns. The current result is a vehicle architecture target, not a national sortie-rate proof.

## 8. Base, workforce and formation consequences

The reference expands the atmospheric base from the prior 2.2-square-kilometre assumption to 2.8 square kilometres. Each base needs two signed load towers, six independent energy buses, large-area weather and approach control, segmented lift-gas handling, contact-system maintenance, structural inspection and a separate public-service release chain. The declared capital increment is $420 million per ready package before the wider program accounts.

Architecture-specific labor adds forty-two deployed people, ninety-two affiliated positions and sixteen minimum-watch positions to `DCP-2`:

| Function | Deployed | Affiliated | Minimum watch |
| --- | ---: | ---: | ---: |
| distributed-contact operations | 12 | 26 | 4 |
| weather and icing cell | 6 | 13 | 2 |
| high-power energy specialists | 6 | 13 | 2 |
| receiver landing control | 12 | 26 | 4 |
| structural health and envelope repair | 6 | 14 | 4 |
| **HBL architecture addition** | **42** | **92** | **16** |

The revised `DCP-2` boundaries are 528 deployed people, 1,157 affiliated positions and a 174-person minimum watch. These additions are not generic support percentages. Each one exists because a physical architecture created a distinct safety, control, maintenance or receiver task.

## 9. A new industrial sector, not a boutique fleet

Forty-three ready `DCP-2` packages require two `HBL-340` vehicles each. A twenty-percent attrition and overhaul pool and eight development articles produce:

| Article class | Quantity |
| --- | ---: |
| operational vehicles | 86 |
| attrition and overhaul reserve | 18 |
| development and test | 8 |
| **total production** | **112** |

The declared twenty-five-year ramp peaks at eight aircraft per year. It requires two final integration lines, two qualified structural lineages, three propulsion suppliers, two energy-system lineages and two landing-system lineages. Peak direct program employment is 24,000; the wider supplier, depot and service ecosystem reaches 65,000.

This is the institutional analogue of a major military-aircraft enterprise. The Department would need an airworthiness authority, experimental ranges, climate-flight test, large-composite manufacturing, megawatt airborne power, lift-gas machinery, robotic cargo systems, low-pressure heavy landing technology, national recovery assets and a permanent technical school system. The value is larger than disaster inventory. These capabilities can spill into heavy civil transport, remote construction, grid restoration, offshore industry, climate adaptation and partner-force exports.

The production sensitivity exposes a second constraint. Raising assigned hard-access groups from twenty-two to thirty increases ready packages from forty-three to fifty-nine and total required articles from 112 to 150. The baseline two-line schedule still produces only 112. The stressed result therefore requires a deliberate rate or line expansion; higher force demand cannot be represented only as a larger cost cell.

## 10. Program economics

| Program account | `H1` | `H2` | `H3` | `H4` |
| --- | ---: | ---: | ---: | ---: |
| ready-pair lifecycle | $550.4000B | $524.6000B | $670.8000B | $602.0000B |
| development and test articles | $29.6000B | $27.2000B | $34.4000B | $31.2000B |
| reserve vehicles | $57.6000B | $52.2000B | $68.4000B | $61.2000B |
| architecture R&D | $110.0000B | $120.0000B | $130.0000B | $105.0000B |
| production tooling | $90.0000B | $85.0000B | $110.0000B | $95.0000B |
| base capital expansion | $23.6500B | $18.0600B | $32.2500B | $25.8000B |
| base operating expansion | $13.5966B | $10.19745B | $16.99575B | $14.95626B |
| full-scale proving | $75.0000B | $60.0000B | $80.0000B | $70.0000B |
| certification and training | $35.0000B | $35.0000B | $40.0000B | $35.0000B |
| **architecture program** | **$984.8466B** | **$932.25745B** | **$1,182.84575B** | **$1,040.15626B** |

`H2` is the least costly complete program among the declared rivals, but cost does not select it. It is selected because it alone passes the universal behavior screen. The H4 label `CONDITIONAL` applies only to transfer with a 340-tonne external ballast chain; the architecture still fails the universal weather-and-receiver decision.

The non-HBL remainder of the configured `DCP-2` account is $584.9764 billion. Substituting the selected architecture produces:

| Boundary | Value |
| --- | ---: |
| `HBL-340` architecture program | $932.25745B |
| non-HBL `DCP-2` remainder | $584.9764B |
| **revised `DCP-2` program** | **$1.51723385T** |
| dynamic one-region `F1-C1` base | $7.38314155T |
| **revised national boundary** | **$8.9003754T** |
| increase above Pass 82 national boundary | $583.95745B |

At thirty assigned groups, the model requires fifty-nine ready packages, 150 articles, a $1.74034825 trillion `DCP-2` program and a $9.441045 trillion national boundary. Restoring twenty-two groups returns every baseline exactly.

The magnitude is a research result. The earlier residual “saving” against unconfigured duplication has disappeared because the liftship is now charged as a complete industrial and operational system. Like-depth configuration can overturn apparent efficiencies. No comparison with full duplication should be reopened until `ATUT-170` and the duplication control are configured to the same physical depth.

## 11. Mission-driven technology campaigns

The selected reference creates eleven technology and proving campaigns totaling $215 billion inside the wider program:

| Campaign | Account | Decisive contradiction |
| --- | ---: | --- |
| hybrid-lift structure and cells | $28B | an 850,000-m³ hull must remain damage-tolerant after cell loss |
| distributed high-authority propulsion | $24B | 240-km/h cruise and 38-m/s gust control with one pod out |
| mission energy and thermal control | $18B | more than 1 GWh must remain segmented and safe aloft |
| ground-coupled arrest and unloading | $22B | 292 t of reaction must enter weak ground without rebound or excursion |
| buoyancy-transition control | $12B | at least 60 t of rapid internal authority without structural damage |
| icing, lightning and severe weather | $16B | a huge surface must retain lift and control in damaged-region weather |
| offline flight and receiver control | $10B | network denial cannot prevent safe approach and transfer |
| cargo restraint and unload order | $12B | the service dependency graph must remain physically accessible |
| emergency landing and recovery | $18B | loss of one site cannot strand a strategic article |
| production learning and digital certification | $25B | 112 vehicles must become a reproducible fleet, not bespoke prototypes |
| compound public-service proving | $30B | vehicle arrival must become safe, repeatable service and reset |

The important innovation policy is not any one speculative component. It is the decision to acquire the whole contradiction. Each campaign receives a representative article, a decisive trial, a failure condition, an industrial output and an independent evidence owner. The Department acts as lead market, systems integrator and public-service certifier without allowing the builder to certify its own mission result.

## 12. Evidence and falsification

Seventy evidence gates remain open. Twenty-eight apply the common mass, lift, geometry, energy, transfer, weather and clock tests to all four rivals. Twenty-six deepen the selected `H2` architecture. Sixteen govern production, supplier ancestry, basing, civil release, workforce, fleet quantity and rendering.

The architecture should be rejected or materially redesigned if any representative program demonstrates that:

- the complete dry mass exceeds the lift and receiver closure after realistic structural reserve;
- the lift-to-drag ratio or drag coefficient makes the inherited clock or energy mass unattainable;
- gust, icing or lightning protection consumes the declared control and energy margins;
- the ground-contact system cannot remain below the bearing floor during asymmetric arrest or unloading;
- sixty tonnes of internal authority cannot control hot-high offload, abort and reload transitions;
- one pod, bus, lift cell, contact sector or control-lane loss propagates into vehicle loss;
- cargo order, balance or restraint prevents four-hour transfer;
- the 142-hour reset path cannot be repeated across fleet queues and contaminated returns;
- two independent production and supplier lineages cannot retain configuration equivalence; or
- vehicle arrival cannot repeatedly produce public-service release inside the inherited hour-42 path.

No pass count is a probability, and no declared margin is a confidence interval. The workbook separates assumptions, formulas, behavior worlds and evidence gates precisely so a coherent concept cannot be mistaken for observed capability.

## 13. Institutional implications

The selected architecture changes what an equal civil instrument of power means.

First, **receivers become national infrastructure**. The force does not merely own aircraft; it owns surveyed weak-ground landing zones, offline approach control, public release teams, mobile bearing reinforcement and recovery routes.

Second, **maintenance becomes operational mass**. Structural-health personnel, climate-flight release, megawatt energy specialists and contact-system operators are formation elements. They cannot be represented as a later percentage of acquisition cost.

Third, **airworthiness must be subordinate to public-service proof but independent of operations**. A safe flight that cannot unload or leaves an unsafe power-and-water system has failed the mission. A useful payload cannot justify unsafe flight. The Department needs separate vehicle, receiver and public-service acceptance authorities joined by a signed mission state.

Fourth, **industrial plurality is part of resilience**. Two integration lines are insufficient if they depend on one lift-cell chemistry, one energy-control kernel or one structural repair process. Qualified substitute lineages must be designed into the acquisition program rather than sought after a crisis.

Fifth, **innovation at this scale is a strategic economic policy**. Large hybrid-lift structures, megawatt civil aviation, robotic heavy transfer, climate-flight operations and rapid field recovery can become exportable capability families. Partner access should be governed as interoperable public-service capacity, not as surplus equipment transfer.

## 14. What is now stable—and what is not

The competition stabilizes five research conclusions:

1. the 340-tonne payload cannot be treated as a sufficient vehicle specification;
2. offload transition, not buoyant cruise alone, governs universal receiver compatibility;
3. a deliberately underbuoyant, ground-coupled hybrid is the only current rival that closes the declared universal behavior screen;
4. the atmospheric carrier is a roughly trillion-dollar national industrial program rather than a small formation equipment line; and
5. external geometry remains too immature for responsible rendering.

The competition does **not** stabilize a hull shape, material system, energy source, propulsion layout, landing mechanism, lift-cell geometry, flight-control law, weather envelope, measured reliability, production rate or operating cost. It does not admit `H2`, select a contractor or claim the Department-wide force is fully costed.

The next connected pass should compete physical `ATUT-170` architectures under the same discipline: transported and gross mass, deck geometry, ground pressure, distributed traction, articulation, slope and debris mobility, water crossing, route preparation, self-recovery, convoy control, energy, maintenance, base demand, workforce, production and full-scale proving. Only after the atmospheric and terrain carriers are both physically configured should the project reconcile `DCP-2`, test like-depth alternatives and reconsider whether requirements renderings are informative rather than premature.
