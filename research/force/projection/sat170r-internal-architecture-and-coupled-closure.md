# `SAT-170R` internal architecture and coupled closure

## Purpose and decision

Pass 85 established that the terrain carrier could not be treated as a heavy transporter with an energy module and soft-ground equipment added afterward. Energy mass changed gross mass; gross mass changed route energy and ground contact; contact hardware changed mass again. Pass 86 asks the harder question: can the resulting vehicle actually be arranged in space while preserving payload access, crew survival, damaged-route passage, independent public-service release and recovery after a credible local casualty?

The provisional answer is yes, but not in the form previously implied.

The twenty-three-metre payload spine cannot remain one rigid body. At the registered twenty-five-metre turn radius, its chord sagitta is about 2.80 metres. Added to the 9.5-metre transit body, the resulting 12.30-metre swept width exceeds the twelve-metre route envelope before contact-pod motion or control error is considered. The selected `P4` behavior reference therefore divides the vehicle into **four 11.5-metre rigid bodies connected by three active joints**. The middle two bodies carry four payload positions each; the forward and aft bodies contain mirrored pairs of energy citadels. The payload remains one governed service block, but no rigid payload position crosses the center joint.

The bridge changes as well. A twenty-metre clear gap does not require twenty metres of carried bridge. It requires twenty-five metres of installed bridge after allowing 2.5 metres of bearing at each end. If the vehicle must still cross after one module is unavailable, five five-metre modules are insufficient: one loss leaves only twenty metres. The carrier must travel with six modules so that five remain available after the declared loss.

Those corrections make bridge structure a second gross-mass feedback beside energy. Solving the two together produces a **547.185-tonne tare**, **717.185-tonne rated gross**, **667.031 megawatt-hours of onboard deliverable energy**, and **285 square metres of deployed contact**. The vehicle is not a marginal enlargement of Pass 85. It is a different internal architecture with a more honest system boundary.

The mission arithmetic still closes. A four-vehicle terrain cell reaches civil public service at relative hour 43.57 and absolute hour 49.57, later than the atmospheric cell’s hour 47.92. The terrain path therefore becomes the governing `DCP-2` clock with 4.43 hours remaining to the hour-54 boundary. The bridge reset path reaches hour 166, leaving two hours to the 168-hour ceiling. Both margins are narrow enough that representative delay, rework or maintenance distributions can overturn them.

The companion [executable workbook](../../../models/force/projection/sat170r-internal-architecture-and-coupled-closure.xlsx) contains eighteen sheets: assumptions, architecture competition, spatial zones, mass and balance, thirty-four mass packets, contact and turn geometry, energy and heat rejection, bridge and route closure, payload and crew, casualty worlds, receiver geometry and clock, reset and workforce, production and cost, a technology program, 140 evidence gates and 190 terminal checks. All 190 checks pass; the formula-error scan is empty. All 140 evidence gates remain open and strict readiness credit is zero.

Exterior rendering remains blocked. This pass defines a provisional internal topology and a proving burden, not a certified shape.

## 1. The design object is a moving service plant

`SAT-170R` is easy to misunderstand if it is described as a large off-road vehicle. The terrain cell does not merely carry 635 tonnes from one intact logistics node to another. Four carriers must each accept one complete 158.75-tonne service block, travel 800 kilometres across progressively damaged routes, open the last discontinuities, enter an independently governed receiver, unload without a common strategic machine, and contribute to lawful public service. The cell must retain its mission meaning after denial of the atmospheric path.

That makes the carrier a moving service plant with seven simultaneous obligations:

1. preserve the registered payload as an identifiable, accessible and balanced service block;
2. propel the complete vehicle through the route without relying on a host grid or host cooling water;
3. spread dynamic load over damaged ground after one contact pod is lost;
4. carry and place the infrastructure needed to cross a route discontinuity;
5. keep a local energy or mobility casualty from consuming the whole vehicle;
6. protect enough people and control authority to reach a safe state; and
7. fit the terrain receiver while retaining unload, repair and exclusion clearances.

These are not additive features. Their interfaces decide the architecture. A bridge stored through a crew escape route, a tank removable only across the payload deck, a cooling surface that occupies the only unload face, or a joint that cuts through a restrained service block does not produce a complete carrier even if each subsystem passes independently.

The governing design rule is therefore spatial and causal:

> Every required function must have a place, a load path, an energy path, a heat path, an access path, a failure boundary, a removal direction and a release authority inside the same mission configuration.

## 2. Competing complete arrangements

Four internal arrangements face twenty non-substitutable gates. The gates cover payload cube and deck demand, bilateral unloading, joint placement, turning and sweep, three-axis balance, four fire zones, one-sector containment, route and stationary cooling, failed-module removal, pod sweep, bridge survival after one module loss, two separated crew refuges, two egress paths, hour-45 relative service and hour-168 reset.

| Reference | Arrangement | Gates passed | Governing failure |
|---|---|---:|---|
| `P1` | rigid payload raft over a central plant | 11/20 | rigid turn, casualty concentration, access and reset |
| `P2` | four-body deck with one-sided energy and service spine | 15/20 | one unload face, asymmetric loss and weak energy separation |
| `P3` | fore–aft twin power blocks with five-module bridge | 17/20 | bearing reserve disappears after one bridge-module loss |
| `P4` | four-body deck with mirrored quadrant energy citadels | 20/20 | provisional behavior reference; no evidence gate closed |

`P1` fails because structural simplicity is purchased with operational impossibility. Its twenty-three-metre rigid center body exceeds the turn envelope, and the central plant makes energy, payload access and crew movement share one casualty domain.

`P2` recognizes articulation but preserves a one-sided service spine. Nominal packaging improves, yet a fire, deformation or obstruction on that side consumes both the local energy sector and one unload face. The layout is also laterally biased in precisely the conditions—soft ground, pod loss and partial unloading—in which balance matters most.

`P3` is close enough to be instructive. Fore and aft energy separation, four rigid bodies and bilateral payload access all work in the model. It fails because it interprets “twenty-metre bridge” as twenty metres of hardware. A physical crossing requires bearing length in addition to clear span. Once one of five modules is unavailable, the promised crossing no longer exists.

`P4` is selected because it is the only arrangement in which all twenty behaviors can coexist. Selection does not mean truth. It means the architecture deserves the next dollar of destructive testing more than the alternatives under the same declared requirements.

## 3. Four rigid bodies, one governed payload

The selected vehicle remains 46 metres long, 9.5 metres wide in transit, 11.8 metres wide in its deployed operating condition and 9.5 metres high. Its longitudinal grammar is symmetric enough to balance but not so symmetric that it hides distinct human roles.

| Zone | Longitudinal extent | Principal contents | Governing boundary |
|---|---:|---|---|
| nose crush and recovery | 0.0–1.7 m | recovery eyes, sacrificial structure, fire drain outlet | energy tanks cannot reach the impact face |
| forward energy body | 1.7–9.5 m | citadels `E1` and `E2`, generators, inverters and coolers | no common tank, sump, bus or cooling loop |
| forward refuge buffer | 9.5–11.5 m | six-seat mission refuge, barriers and exits | no egress crosses an energy bay |
| cargo body `C1` | 11.5–23.0 m | four dry positions, one wet-pack interface, handling bay | no restrained payload crosses the center joint |
| cargo body `C2` | 23.0–34.5 m | four dry positions, handling and bridge keel bay | same governed block, separate rigid structure |
| aft refuge buffer | 34.5–36.5 m | four-seat recovery refuge, independent controls | local black start and distinct egress |
| aft energy body | 36.5–44.3 m | citadels `E3` and `E4` | mirrored but not commonly supplied |
| tail crush and recovery | 44.3–46.0 m | recovery eyes, sacrificial structure, drain outlet | aft module extraction remains possible |

The three joints lie at 11.5, 23.0 and 34.5 metres. Each is assigned a provisional thirty-degree yaw range and eighteen-degree pitch and roll capability. The vehicle must coordinate all twelve contact pods around the joints; “articulation” cannot mean passive hinges behind a conventional tractor.

The central joint changes the meaning of payload continuity. Cargo body `C1` and cargo body `C2` are physically independent 11.5-metre structures, yet their eight positions remain one serial manifest, one load plan and one service release. A joint cannot be used to justify pre-release cross-loading or to make half a service block count as delivered capability.

This is a useful institutional distinction. Physical modularity is desirable; mission fragmentation is not. The configuration authority must know both the mechanical body to which an item is restrained and the civil service block to which it belongs.

## 4. Coupled mass closure

Energy and bridge structure both grow with rated gross mass. Treating either as a fixed allowance would make the other calculation false.

Let:

- `G` be rated gross mass;
- `M_f` be fixed non-energy, non-bridge mass including rated payload;
- `H` be fixed energy hardware mass;
- `E_w` be fixed route-work energy;
- `a` be route energy per tonne of gross mass;
- `r` be the energy reserve fraction;
- `s` be usable electrical energy per tonne of consumable;
- `B_f` be fixed bridge-launch, mat, robot and restraint mass; and
- `k_b` be carried bridge structural mass per tonne of rated gross.

The bridge mass is:

\[
M_b=B_f+k_bG
\]

and the complete energy mass is:

\[
M_e=H+\frac{(1+r)(aG+E_w)}{s}.
\]

The rated gross fixed point is therefore:

\[
G=\frac{M_f+B_f+H+(1+r)E_w/s}
{1-k_b-(1+r)a/s}.
\]

The bridge feedback coefficient is 0.0462051 tonne per tonne gross. The reserve-adjusted energy coefficient is 0.1585317. Their combined feedback is 0.2047368, leaving a positive closure denominator of 0.7952632. A finite first-order solution exists under the declared coefficients.

| Mass element | Pass 86 mass |
|---|---:|
| structure, three joints and fire boundaries | 87.600 t |
| propulsion and partitioned distribution | 68.000 t |
| complete energy system | 187.347 t |
| `TAP-285` mobility system | 103.600 t |
| payload handling | 24.000 t |
| bridge and route kit | 56.138 t |
| control, dual refuges and life safety | 20.500 t |
| **tare** | **547.185 t** |
| rated payload | 170.000 t |
| **rated gross** | **717.185 t** |
| assigned mission payload | 158.750 t |
| **mission gross** | **705.935 t** |

The vehicle retains 11.25 tonnes between the assigned block and rated payload. That is a configuration allowance, not spare payload available for unrelated cargo.

The increase from Pass 85’s 648.451-tonne rated gross is 68.734 tonnes. The bridge reserve, spatial safety structure and contact growth directly add mass; their energy and bridge feedback then amplify it. The lesson is larger than one vehicle: first-principles programs need configuration accounting early enough that “allowances” cannot remain independent after the physics has joined them.

## 5. Mass packets, stability and local support

A whole-vehicle center of gravity can look acceptable while one support station is overloaded. The model therefore divides structure, propulsion, four energy sectors, six mobility pairs, payload handling, route equipment, two refuges and four payload quarters into thirty-four mass packets. Each packet is mapped to the two adjacent support stations or assigned directly to one station.

The six station reactions are approximately 108.04, 119.64, 132.66, 132.66, 116.97 and 107.21 tonnes. Their sum reconciles to rated gross. The largest station carries 1.1098 times the average, below the provisional 1.15 control limit. After the registered dynamic factor, the largest local pod demand is 83.91 tonnes; a one-pod redistribution case produces 82.48 tonnes. Both sit below the new 85-tonne structural target, with only 1.09 tonnes of margin in the nominal worst station.

Rated center of gravity is 22.82 metres from the nose, essentially centered along the 46-metre vehicle, and 3.768 metres above ground. The first-order geometric screens produce a 51.58-degree transit rollover angle and 57.44-degree deployed angle. These are static geometric limits, not operating permissions. Suspension travel, soil deformation, liquid motion, joint phase, braking, payload release order and control latency can all create earlier loss of margin.

The mass-packet compiler should become an operational artifact. Before departure, measured tank quantities, payload serials, module states and pod health should compile to signed limits for speed, slope, joint command, unloading order and recovery. Network denial must not prevent a vehicle from refusing an unsafe configuration locally.

## 6. `TAP-285`: contact as an active structure

The contact system is now sized from the revised gross mass rather than inherited from the prior carrier.

With one of twelve pods unavailable, a 1.15 dynamic factor and 1.10 pod-imbalance factor, compounded pressure is:

\[
p=\frac{717.185\times9.81\times1.15\times1.10}
{285\times11/12}=34.07\ \text{kPa}.
\]

The result is below the thirty-five-kilopascal screen by 0.93 kilopascal. That is a design target, not evidence of mobility in mud, peat, ash, debris, ice or flood sediment.

Each pod supplies 12.92 square metres in transit and 23.75 square metres when deployed. A provisional four-metre-wide contact patch changes from 3.23 to 5.94 metres long, requiring 1.35 metres of extension at each end. Six bilateral station pairs sit at 4.0, 12.5, 19.5, 26.5, 33.5 and 42.0 metres.

This geometry is more than a track extension. Each pod must steer, brake, sense normal and shear load, coordinate around three joints, reject debris, isolate after seal or drive failure and permit recovery without exposing the crew beneath a 700-tonne machine. The likely technology is a family of replaceable load modules with local controllers and mechanically safe degraded modes, not twelve copies of one conventional undercarriage.

The twenty-five-metre turn requires about 26.59 degrees of joint yaw. An 11.5-metre rigid body has about 0.67 metre of chord sagitta, producing a 10.17-metre first-order swept width inside the twelve-metre screen. The minimum deployed footprint gap is 1.06 metres and the provisional joint-to-pod sweep clearance is 1.97 metres. By contrast, the 23-metre control body produces 12.30 metres of swept width and fails. The control is deliberately retained in the workbook because it proves the third joint is an architectural requirement rather than aesthetic preference.

## 7. The bridge is part of the vehicle’s mass loop

The bridge requirement is a twenty-metre clear discontinuity with 2.5 metres of usable bearing at each end. Five five-metre modules form the required twenty-five-metre installed structure. Six modules travel.

The first-order structural screen assumes that eighty percent of rated vehicle mass is supported in the governing bridge state, applies a 1.20 crossing dynamic factor, and treats the clear span as a simple span. The dynamic supported-mass equivalent is 688.50 tonnes and the total design bending moment is 33.77 meganewton-metres. With a 2.4-metre truss depth, a 600-megapascal allowable chord stress, metallic-equivalent density and a factor of three for webs, deck, joints, buckling and cross-bracing, the installed five-module structure is 27.61 tonnes. The carried six-module structure is 33.14 tonnes; launcher, approach mats, robots and restraints bring the route kit to 56.14 tonnes.

This calculation is intentionally conservative and incomplete. It does not establish local wheel-load distribution, joint stiffness, fatigue, lateral stability, bearing failure, hydraulic uplift, scour, damaged approaches or material manufacturability. Its function is to prevent bridge mass from remaining a free constant while those questions are pursued.

The six modules are stored as paired half-width leaves in split-keel cassettes beneath the two cargo bodies. The complete stowage claim is 96.35 cubic metres against 115 cubic metres assigned. One adjacent contact pod retracts, half-width leaves eject laterally, route robots carry them to the leading end, and two robotic erectors assemble five modules and place approach mats. The provisional deployment target is 1.75 hours.

No crew member should have to work beneath a suspended module or enter the primary crush zone for routine placement. The bridge program therefore needs autonomous handling, machine-verifiable joints, embedded load sensing and a safe hold state as fundamental features—not optional automation added after a manual bridge is designed.

After one module loss, five remain and the twenty-five-metre physical bridge survives. After two losses, only twenty metres remain and the vehicle must hold or reroute. The atmospheric cell preserves the whole `DCP-2` service guarantee, but the terrain path loses its own crossing claim. This boundary is explicit rather than hidden in a generic redundancy statement.

## 8. Four energy citadels and independent heat rejection

The 187.347-tonne energy system contains 132.347 tonnes of mission consumable and fifty-five tonnes of fixed conversion, containment and thermal hardware. Mission energy is 567.686 megawatt-hours; the 17.5-percent reserve raises onboard deliverable energy to 667.031 megawatt-hours.

Four nine-megawatt sectors are arranged as two forward and two aft citadels. Each sector owns its tank cassette, generator, inverter, protected bus lane, cooler, vent, drain, suppression trains and end-directed removal path. Normally open cross-ties may support restoration, but the vehicle must complete the registered maximum route case with one entire sector unavailable. Twenty-seven megawatts remain against a calculated 24.55-megawatt route demand.

Per sector, the model allocates 166.76 megawatt-hours of deliverable energy and 33.09 tonnes of consumable. The liquid occupies 39.70 cubic metres at the declared delivered-energy density; tank utilization expands the cassette to 48.42 cubic metres. Fixed hardware requires 28.65 cubic metres and isolation, cooling and removal clearance add eighteen. Total demand is 95.07 cubic metres against a 102.34-cubic-metre bay. The 7.27-cubic-metre reserve is small enough that tank geometry, ducts, structural frames, valves, cable bend radius or maintenance envelopes can reopen the vehicle length.

Heat rejection may not depend on a river, floodwater or municipal supply. At a provisional 42-percent electrical efficiency and 68-percent exhaust share of waste heat, the remaining coolant load is 10.85 megawatts at maximum route demand. Ninety-six square metres of fixed radiator surface, derated to seventy percent for smoke and fouling, reject 12.10 megawatts in the route state. At full stationary output, 168 square metres of deployed surface reject 16.46 megawatts against 15.91 required. With one sector out, 126 square metres reject 12.35 megawatts against 11.93 required.

These are coefficient-level behaviors, not a design of a cooler. The research program must discover how to package large surface area without consuming unload access, how to clean it in ash and mud, how to survive debris and branches, and how to prevent a local fluid or fan failure from propagating across citadels.

## 9. Payload and crew are coequal configuration owners

All four registered payload blocks weigh 158.75 tonnes, but their cube and deck demand differ. The largest block uses 772 cubic metres and the largest deck case uses 176 square metres. The two cargo bodies provide 800 cubic metres and 184 square metres through eight dry cradles plus a segregated wet-pack well.

Each cradle can side-shift to either side. The vehicle does not assume that a receiver loader reaches beneath it, that one side remains accessible, or that a failed energy module can be moved across the cargo deck. Bilateral unloading is a survival behavior: an obstruction, soft shoulder, fire boundary or disabled pod on one face does not automatically deny every payload position.

Using the full 800-cubic-metre allowance over the 184-square-metre deck produces a 4.348-metre usable cargo height. With a four-metre deck datum, the cargo top is 8.348 metres, below the 9.5-metre vehicle envelope. All four registered block center-of-gravity cases remain inside the declared longitudinal and lateral limits.

Crew are not placed in leftover volume. A six-seat forward mission refuge and four-seat aft recovery refuge sit in separate two-metre buffers between cargo and energy bodies. Each has two independent exits, local black start and access to distinct control lanes. The maximum modeled internal egress path is six metres against a seven-metre screen. No normal egress route crosses an energy bay or payload zone.

The forward refuge owns mission command; the aft refuge owns recovery and safe withdrawal if the forward space is denied. That does not mean either refuge has been proven survivable. The 120-minute fire boundary, toxic-product control, smoke management, crash pulse, overturn escape and remote operation remain open representative tests.

## 10. Casualty logic changes the meaning of redundancy

Subsystem loss cases are not credible if they ignore co-location. A forward energy sector and its neighboring pod may share impact, fire, deformation, debris and control damage. The design-basis local casualty therefore removes both together: three energy sectors and eleven pods must close at the same time.

The workbook distinguishes four outcomes that ordinary redundancy tables often collapse:

- the vehicle remains physically safe;
- the vehicle retains controlled movement;
- the terrain cell retains its hour-45 relative-service claim; and
- the complete `DCP-2` formation still produces a service effect.

A locked articulation joint may permit slow withdrawal but deny the route clock. Loss of both sectors at one end may leave a safe vehicle without leaving a mission vehicle. Loss of one complete `SAT-170R` makes the four-carrier terrain cell incomplete; the atmospheric cell preserves the formation-level effect, but the terrain cargo is not quietly redistributed before release. Loss of both access modes remains outside the declared guarantee.

The most important failure world is evidentiary. If a representative sector fire crosses a bulkhead, if a common coolant path spreads damage, if an arc corrupts multiple buses or if removal requires crossing an occupied refuge, `P4` loses its behavior reference even if the spreadsheet arithmetic remains intact. Modeled isolation is a test proposition, not a fact.

## 11. Receiver geometry and the mission clock

Four vehicles occupy a two-by-two terrain receiver grid. A seventy-two-metre longitudinal pitch and thirty-eight-metre lateral pitch create 26.0 metres of end separation and 26.2 metres of side separation between vehicles. With fifteen metres of extraction clearance at the outer ends and ten metres of outer side-work space, the grid needs 148 by 69.8 metres. It fits within the 200 by 100-metre transfer core and 220 by 140-metre controlled receiver.

All vehicles point in the same direction. The front row retains forward energy-module extraction; the rear row retains aft extraction. Bilateral cargo movement keeps at least twelve metres of side-work space. Quadrant vents and drains face outward. A failed energy cassette can be isolated in place until after public release or a mission abort; repair is not silently inserted before service.

The revised critical path is:

| Task | Duration | Finish |
|---|---:|---:|
| origin load, citadel seal, joint and measured-CG release | 8.75 h | 8.75 h |
| 500 km degraded hard route | 10.00 h | 18.75 h |
| 220 km broken or saturated route | 6.875 h | 25.625 h |
| 80 km off-road and obstacle route | 4.444 h | 30.069 h |
| contact transition, survey, bridge and route work | 4.75 h | 34.819 h |
| unload, thermal deployment, assay and civil release | 8.75 h | 43.569 h |

The six-hour regional activation offset places absolute terrain public service at hour 49.569. The 45-hour relative ceiling retains 1.431 hours; the absolute hour-54 boundary retains 4.431 hours. Since air service remains at hour 47.917, terrain now governs complete dual service.

An optional post-release cross-tie can be complete at hour 51.569. It does not change either cell’s release. This preserves the Pass 85 rule that federation begins after independent service, not before it.

## 12. Reset, people and industrial depth

Reset is a collection of concurrent technical releases, not a single maintenance duration. The pod path reaches 164 hours, energy citadels 156, structure and joints 142, bridge and route equipment 166, crew and control records 52, and receiver and route handback 120. Bridge inspection, joint metrology and reload govern at hour 166.

That two-hour margin is an institutional signal. The force cannot claim a seven-day reset because an average overhaul fits. It needs preplanned exchange modules, parallel metrology capacity, spare bridge leaves, trained inspectors, recovery fixtures and sufficient depot bays to keep the longest path from becoming a queue.

The spatial correction adds sixty deployed personnel, 144 affiliated positions and a sixteen-person minimum watch above Pass 85. The new specialties include energy-citadel and fire-boundary technicians, ultra-heavy modular bridge teams, load and articulation engineers, field module-recovery teams and crew-survival specialists. The revised `DCP-2` boundary is 700 deployed personnel, 1,557 affiliated positions and a minimum watch of 226. The wider terrain industrial ecosystem grows from 95,000 to 118,000 workers in the research comparator.

Those jobs are not support overhead around the machine. They are the capability. A department that funds advanced materials but not independent configuration authority, or autonomous bridge handling but not field metrology, has funded demonstrations rather than a force.

## 13. Program and fiscal consequence

The baseline program retains 43 ready four-vehicle terrain packages, 172 operational vehicles, thirty-five reserve vehicles and twelve development and test articles: 219 vehicles in total. The architecture requires five final integration lines, four energy-citadel lineages, three pod lineages, three bridge lineages and seven compound proving ranges. The provisional operational production peak is fifteen vehicles per year.

| Program element | 25-year research comparator |
|---|---:|
| ready-set lifecycle | $670.800B |
| development and test | $38.600B |
| reserve vehicles | $89.250B |
| architecture R&D | $330.000B |
| production tooling | $178.000B |
| base capital expansion | $20.640B |
| base operating expansion | $21.755B |
| full-scale proving | $155.000B |
| certification and training | $78.000B |
| **`SAT-170R` architecture program** | **$1,582.045B** |

The correction adds $243.299B to the Pass 85 terrain program. With the unchanged $1,226.984B non-terrain remainder and $170.787B federated-receiver increment, `DCP-2` rises to $2,979.815B. The associated national boundary rises to $10,362.957B.

These are controlled design comparators, not forecasts or acquisition estimates. Their purpose is to show what honest system boundaries do to an equal-scale civil force. If the vehicle depends on new bridge materials, energy conversion, robotic placement, compound ranges, crews, depots and independent suppliers, those resources belong inside the proposition.

At thirty deployment groups, the fleet rises to 296 vehicles and the terrain program to about $1.881T; `DCP-2` reaches $3.412T and the national boundary $11.112T. The stress case exposes a production and workforce obligation rather than implying that more formations appear without new industrial capacity.

## 14. A $530 billion technology campaign

The selected architecture is not constrained to current commercial components. It becomes a mission-driven innovation portfolio with rival physical implementations and explicit failure transitions. The $530B portfolio is included within the R&D, proving and relevant receiver accounts; it is not added again to the program total.

The largest campaigns pursue cellular energy-citadel architecture, a high-temperature generator core, fuel containment and fire control, no-host-water heat rejection, fault-contained power electronics, `TAP-285` contact, dynamic load and stability control, terrain sensing, pod sealing and braking, an ultra-high-load modular bridge, autonomous bridge handling, articulated structure, bilateral payload access, occupied crew refuges, field module recovery and an offline configuration-and-physics compiler.

At least three rival lineages remain funded for decisive systems. The point is not procurement theater. Competing implementations prevent one favorable coefficient from becoming a hidden monopoly on the force concept. An alternative energy sector may be lighter but lose on casualty containment; a bridge material may reduce mass but fail inspectability; a pod may lower pressure but become impossible to clear of debris. Whole-system evidence must eliminate rivals.

The program’s industrial output is broader than a carrier. It creates new sectors in distributed mobile power, high-load civil bridging, adaptive ground systems, destructive civil-safety testing, autonomous infrastructure construction, field-removable plant modules and offline configuration authority. These are exportable capacities because other states face the same damaged-service problem, not because export volume is assumed to justify the domestic mission.

## 15. Proving campaign and admission logic

The evidence register contains 140 gates across packaging, mass and stability, energy and thermal systems, contact and route opening, crew and payload, and program delivery. Every gate identifies a claim, representative object, destructive challenge, failure rule and independent authority. All remain `OPEN`; strict credit is zero.

The proving sequence should advance through increasingly coupled objects:

1. instrumented joints, pod quadrants, bridge chords, tanks, converters, coolers, cradles and refuge barriers;
2. complete energy citadels, bilateral payload bays, pod pairs and bridge modules;
3. representative fore and aft bodies, one complete cargo body and a full jointed half-vehicle;
4. full-gross vehicles under measured mass, mud, grade, turn, bridge, fire, thermal and module-removal worlds;
5. four-vehicle receiver missions with one local compound casualty; and
6. complete terrain and atmospheric cells under independent release, one-mode denial and seven-day reset.

The sequence must include deliberately inconvenient cases: a full payload at the allowed center-of-gravity boundary; smoke and ash on the thermal surfaces; one pod disabled beside one tripped energy sector; a bridge leaf unavailable; one unload face blocked; a refuge denied; a joint locked; network denial; stale configuration data; and a supplier-lineage hold. The test article must be representative in mass, energy, geometry, materials, controls and crew exposure. A light demonstrator cannot validate a 717-tonne interaction.

Admission moves the architecture, not merely the score. If pod mechanics require more volume, the 46-metre envelope may reopen. If fire containment consumes a buffer, payload or energy volume must move. If the bridge coefficient rises, both bridge and energy mass rise. If the hour-166 reset cannot be repeated, fleet and depot quantities must change. If a decisive common supplier ancestor emerges between air and terrain, the `DCP-2` assurance claim must be revised even if both vehicles work.

## 16. What this pass makes authoritative

At research maturity `R2`, Pass 86 makes the following configuration grammar authoritative for subsequent work:

- `P4` is the sole internal behavior reference under the twenty registered hard gates;
- the vehicle contains four 11.5-metre rigid bodies and three active joints;
- the payload occupies two rigid cargo bodies but remains one governed service block;
- four independently bounded nine-megawatt energy citadels sit in mirrored fore and aft pairs;
- two occupied refuges lie in separate buffers and own distinct safe-state roles;
- the contact target is 285 square metres across twelve pods rated to 85 tonnes locally;
- six five-metre bridge modules are carried so one unavailable module still leaves twenty-five metres installed;
- energy and bridge mass are solved in one gross-mass fixed point;
- terrain reaches absolute public service at hour 49.57 and resets at hour 166;
- the program comparator is $1.582T and the revised `DCP-2` boundary is $2.980T; and
- 140 named evidence gates remain open with zero readiness credit.

It does not establish material allowables, pod life, bridge capacity, energy efficiency, thermal flux, fire stopping, toxic safety, crew survivability, route speed, autonomous placement, production rate, cost or readiness. Those remain hypotheses with owners and failure transitions.

## 17. Stocktake and next force-design move

This pass resolves the terrain carrier’s first internal contradiction and exposes a wider methodological one.

The resolved contradiction is physical: a twenty-three-metre rigid payload spine and five carried bridge modules cannot deliver the previously claimed turning and one-loss crossing behaviors. The four-body, six-module architecture restores those behaviors provisionally and propagates the consequence through mass, energy, contact, crew, receiver, reset, workforce, industry and cost.

The unresolved contradiction is comparative. `SAT-170R` now has a substantially deeper internal, thermal, contact, casualty and economic treatment than `GCH-340`. It would be misleading to optimize the terrain vehicle further or render the two-mode force while the atmospheric carrier’s energy, lift-control, landing surface, mooring, ballast transition, structure, heat rejection, crew refuge, module removal and casualty propagation remain at a shallower boundary.

The next force pass should therefore build a complete-system `GCH-340` closure under the same discipline:

- derive installed energy, stored energy, conversion and heat rejection from the full atmospheric mission;
- solve buoyancy, ballast and unloading as a coupled transient rather than separate steady states;
- distribute ground-coupled loads across a defined landing-contact system and damaged bearing surface;
- place lifting cells, structural paths, payload positions, propulsion, mooring, energy, crew and egress in one geometry;
- test local tears, cell loss, gust, mooring failure, hard landing, fire and partial unload as spatial casualties;
- close receiver clearances, authority, public release, reset and industrial lineages; and
- propagate any correction into the shared `DCP-2` clock, workforce and fiscal boundary.

Only after both carriers reach equal physical depth should the program compare whether two access modes still provide independent service under the same evidence rule. That comparison—not visual appeal—will define the first responsible requirements rendering.

The larger lesson for a Department of Resilience is direct. Ambition is not the multiplication of vehicle concepts. It is the willingness to let service guarantees drive new physical architectures, to let contradictions overturn attractive machines, and to fund the laboratories, industries, professions and trials required to discover capabilities that do not yet exist.
