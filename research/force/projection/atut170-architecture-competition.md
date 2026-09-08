# `ATUT-170` architecture competition

## Purpose and decision

This study asks a narrower and harder question than “what should a very large disaster-response truck look like?” It asks which complete physical architecture could move one independently governed 158.75-tonne service load across 800 kilometres of damaged land, arrive through weak soil and broken infrastructure, make that payload usable by relative hour 45, recover itself after representative damage, and return to certified service inside seven days.

The answer is not a scaled road transporter. Three familiar extrapolations each dominate one part of the problem and fail the whole mission:

- a distributed tracked carrier is fast and tractive but too concentrated for the weak-soil case and cannot close the route clock after its obstacle work;
- a load-walking carrier is exceptionally gentle on soil but cannot cover strategic inland distance or bridge the governing gap;
- an amphibious cushion carrier crosses floodwater quickly but cannot generate the required grade traction, fit the route envelope or climb debris;
- a segmented adaptive terrain carrier, `T4 SAT-170`, is the only rival that closes every declared behavior screen.

`T4` is therefore retained as the provisional universal behavior reference. It is not an admitted vehicle and its exterior form is not stable. Its decisive features are a twelve-pod distributed traction system, active articulation and load leveling, variable contact area, sealed wading, a self-laid 25-metre bridge-and-mat kit, route-sensing robots, offline convoy control and cooperative recovery. These are not support accessories. They are inside the vehicle’s mass, energy, crew, industrial, reset and cost boundaries.

The companion [architecture workbook](../../../models/force/projection/atut170-architecture-competition.xlsx) contains the executable mass, pressure, traction, power, route, obstacle, recovery, receiver, resilience, reset, workforce, production and cost argument. All one hundred independent checks pass. All one hundred representative evidence gates remain open, strict readiness credit is zero and rendering remains blocked.

## 1. The object being designed

### 1.1 A carrier is a temporary infrastructure system

The inherited `DCP-2` formation contains two separately governed 635-tonne service cells. The atmospheric cell divides across two `HBL-340` carriers. The terrain cell divides across four `ATUT-170` carriers. Each terrain carrier receives one 145-tonne dry block and one 13.75-tonne wet pack, for 158.75 tonnes assigned. The design rating is 170 tonnes so that the carrier does not begin life at an exact-fit limit.

The payload is not generic cargo. It is a serial part of a public-service machine. The carrier therefore has to preserve:

1. payload identity and custody;
2. load restraint and environmental protection;
3. access to the payload in its required unload order;
4. arrival at a receiver that can bear the carrier;
5. route opening when roads, bridges and surveys have failed;
6. power, sensing and control while national communications are unavailable;
7. recovery without assuming another heavy civil fleet already exists;
8. a reset path that restores the carrier, route kit, crew and receiver together.

The design object is thus closer to a mobile infrastructure battalion embodied in one vehicle than to a tractor and trailer.

### 1.2 Registered mission boundary

The competition holds the following requirements constant.

| Requirement | Registered value | Design consequence |
|---|---:|---|
| Design payload | 170 t | minimum rated payload |
| Assigned payload | 158.75 t | mission load used for receiver calculations |
| Largest assigned cube | 772 m³ | governing stowed-volume demand |
| Largest assigned deck demand | 176 m² | governing load and access surface |
| Usable cube | 800 m³ | 3.6 percent reserve over assigned cube |
| Usable deck | 184 m² | 4.5 percent reserve over assigned deck |
| Damaged-land route | 800 km | strategic inland movement, not local last-mile work |
| Route composition | 500 km degraded hard / 220 km broken or saturated / 80 km off-road and obstacle | three mobility regimes in one mission |
| Origin release and load | 8 h | part of the public-service clock |
| Receiver service build | 8 h | payload must become usable, not merely arrive |
| Relative service ceiling | 45 h | maximum from regional activation |
| Saturated-ground pressure | ≤35 kPa | rated-gross weak-soil admission |
| Receiver bearing floor | 60 kPa | mission-gross receiving surface |
| Route width / turn | ≤12 m / ≤25 m | broken-network maneuver envelope |
| Grade / side slope | ≥20% / ≥12% | longitudinal traction and lateral control |
| Step / gap / water | ≥1.5 m / ≥20 m / ≥2 m | debris, bridge loss and flood approach |
| Unload | ≤4 h | cargo accessible without a separate heavy-crane assumption |
| Recovery pull ratio | ≥1.2 | damaged self- and cooperative recovery |
| Reset | ≤168 h | certified reuse boundary |

These values are research assumptions inherited from or declared within the repository. They are not observations of an existing system.

## 2. Method: eliminate attractive partial answers

The competition uses disqualifying screens rather than weighted scores. A carrier that is excellent in floodwater cannot trade that advantage against an inability to climb the registered grade. A carrier that arrives on time cannot compensate for destroying its weak-soil receiver. A carrier that works only when a separate bridge fleet, survey fleet or recovery fleet arrives first has not closed the universal carrier requirement.

Seven compound screens govern the decision:

1. mass, cube, deck and geometry;
2. weak-soil ground pressure;
3. traction, installed power and mission energy;
4. route time and public-service time;
5. grade, cross-slope, step, gap, water, width and turn;
6. recovery and damaged route-kit residual;
7. receiver entry and unload.

This is deliberately conservative about substitution. A failed gate changes the assurance class rather than merely lowering a score.

## 3. Four clean-sheet rivals

### 3.1 `T1 DTC-170`: distributed tracked carrier

`T1` uses two long articulated tracked hulls under a common load deck. Its intuition is familiar: add track area, electric drive and articulation to the lineage of heavy tracked transporters.

It is the least expensive rival at a declared $712.58 billion for the national architecture program. It carries the required payload and has ample tractive and energy reserve. Its failure is systemic. At 485 tonnes rated gross on 110 square metres of contact, it develops 43.25 kPa, above the 35-kPa saturated-ground limit. Its 32-metre turn radius exceeds the broken-network requirement. The short bridge kit, 1.2-metre step and 1.8-metre wading depth do not close the compound obstacle. Its route takes 41.29 hours before load and receiver build, putting public service at 57.29 hours.

`T1` remains valuable as a prepared-corridor or firmer-ground carrier. It is not universal under the registered case.

### 3.2 `T2 LWS-170`: load-walking transporter

`T2` distributes weight across many independently controlled pads and legs. It is the best static weak-soil and side-slope architecture in the competition. Its 555-tonne rated mass over 190 square metres produces only 28.66 kPa. It steps over 2.5 metres, turns inside 14 metres and develops a 1.5 recovery pull ratio.

Those advantages do not overcome its strategic-mobility failure. At 18, 10 and 6 kilometres per hour across the three route classes, the declared terrain path takes 67.11 hours. Public service occurs at 83.11 hours. Its twelve-metre gap kit and 1.5-metre water depth also fail the universal route. `T2` could be a high-value local works machine or a receiver construction system; it is not the 800-kilometre carrier.

### 3.3 `T3 ACC-170`: amphibious cushion crawler

`T3` uses a segmented air cushion with edge drives. Its 300-square-metre effective contact area produces only 17.00 kPa, and it crosses five metres of water. It is the only non-selected rival to preserve the clock, reaching public service at 44.90 hours.

The same physical logic that produces flotation weakens terrestrial control. With a 0.14 effective traction coefficient applied through only thirty percent of the footprint, the model provides 214 kN of force against 1,428 kN demanded by the grade and soft-ground case. The architecture also declares only an eight-percent grade, six-percent cross-slope and half-metre step. Its sixteen-metre width and forty-metre turn radius are incompatible with the route. `T3` is an amphibious regional carrier, not a universal inland terrain system.

### 3.4 `T4 SAT-170`: segmented adaptive terrain carrier

`T4` accepts that no single contact geometry can dominate the entire route. A central articulated spine carries the payload. Twelve independently powered and steerable terrain pods change their effective contact geometry, shed debris, level the load and isolate damage. A 36-tonne route kit contains a modular bridge-and-mat system and route robots. Control remains local and offline-capable. Recovery hardpoints and cooperative tow are primary structure, not field improvisation.

The declared mass statement is:

| Element | Mass |
|---|---:|
| Primary structure and articulated spine | 68 t |
| Propulsion | 58 t |
| Energy system | 60 t |
| Mobility pods | 72 t |
| Payload handling | 24 t |
| Bridge, mat and route kit | 36 t |
| Control, crew and mission systems | 14 t |
| **Tare** | **332 t** |
| Rated payload | 170 t |
| **Rated gross** | **502 t** |
| Assigned payload | 158.75 t |
| **Assigned mission gross** | **490.75 t** |

The provisional envelope is 42 metres long, 8.6 metres wide and 8.8 metres high. A 23-by-8-metre deck supplies 184 square metres. Cargo clearance of 6.2 metres creates a 1,140.8-cubic-metre geometric envelope around the 800-cubic-metre usable requirement. These are packaging controls, not exterior render geometry.

## 4. The first-principles physics

### 4.1 Ground pressure

Rated-gross nominal pressure is calculated as

\[
p = \frac{m g}{A}
\]

where mass is in tonnes, gravitational acceleration is 9.81 m/s² and effective contact area is in square metres, yielding kilopascals.

For `T4`:

\[
p = \frac{502 \times 9.81}{155} = 31.77\ \text{kPa}
\]

That leaves only 3.23 kPa of declared margin to the saturated-ground boundary. This is not generous. It makes effective contact area, load sharing, sinkage, repeated-pass damage and dynamic pressure primary evidence questions. A static arithmetic pass does not prove mobility in deformable soil.

### 4.2 Traction

The competition separates ground pressure from usable traction. Low pressure alone does not move a vehicle up a grade. Demand is approximated as

\[
F_d = m g (s + c_r)
\]

where \(s\) is the required grade fraction and \(c_r\) is the declared soft-ground rolling coefficient. Available force is

\[
F_a = m g \mu f_d
\]

where \(\mu\) is the effective traction coefficient and \(f_d\) is the driven fraction of the contact system.

For `T4`, the model declares \(\mu=0.62\), \(f_d=1.0\), and \(c_r=0.08\). Demand is 1,378.89 kN and nominal available force is 3,053.26 kN, a 121.4-percent reserve. This large arithmetic margin should not be misread as proof: the coefficient combines soil mechanics, contact control and debris shedding that do not yet exist as representative evidence.

At 35 kilometres per hour on the broken-route segment and 82-percent driveline efficiency, the governing tractive-plus-hotel demand is 18.85 MW. Twelve modules provide 32 MW. Removing one leaves 29.33 MW, above the declared maximum demand.

### 4.3 Energy is the leading feasibility risk

The route-energy model uses a declared 0.85 kWh per tonne-kilometre across 800 kilometres, rated gross mass, and an 80-MWh route-work allowance:

\[
E_m = 0.85 \times 502 \times 800 / 1000 + 80 = 421.36\ \text{MWh}
\]

The architecture declares 600 MWh onboard, producing 42.4-percent arithmetic reserve. But the energy-system mass allocation is only sixty tonnes—ten kWh/kg at the system boundary if the 600 MWh is interpreted as deliverable energy.

That is not a conventional battery assumption. It is not automatically closed by attaching a familiar generator, either: fuel, tanks, conversion equipment, thermal rejection, safety separation and reserve all consume the same mass and volume. The model therefore treats the energy line as a technology target rather than an available component. A liquid-fuel, hydrogen, metal-air, compact nuclear or other architecture must be competed at complete-system level. If the target is missed, additional energy mass raises gross mass, ground pressure, traction demand, structure and cost together. The apparent vehicle pass can be invalidated by this one coupled term.

This is precisely why a Department of Resilience needs military-like technology campaigns: it can specify a civil mission coefficient, fund multiple lineages, build representative ranges and refuse to count projected performance as readiness.

## 5. Route and service clock

The route is not modeled at one average speed. Each architecture traverses three distance classes and carries an explicit route-work allowance:

\[
t_r = \frac{500}{v_h} + \frac{220}{v_b} + \frac{80}{v_o} + t_w
\]

For `T4`, declared speeds of 55, 35 and 20 km/h plus four hours of route work produce:

\[
t_r = 9.09 + 6.29 + 4.00 + 4.00 = 23.38\ \text{h}
\]

Eight hours of origin release and eight hours of receiver service build place public service at relative hour 39.38, leaving 5.62 hours to the hour-45 limit. With the six-hour regional activation offset, absolute service occurs at hour 45.38, inside the hour-54 calendar boundary.

The clock is an integrated requirement. It can fail through slow driving, excessive survey, bridge deployment, payload release or receiver assembly. Future evidence must measure the complete service chain rather than demonstrate maximum speed on a prepared course.

## 6. Obstacles, route ownership and receiver

`T4` passes the declared behavior screen with a 25-percent grade, sixteen-percent side slope, 1.8-metre step, 25-metre organic gap, 2.5-metre water depth, 8.6-metre width and 18-metre turn radius.

The important architectural choice is not any one number. It is ownership of the route problem:

- route robots classify bearing, obstacles and bypasses ahead of the carrier;
- the mobility pods alter contact and articulation rather than asking a separate earthmoving formation to prepare every metre;
- the bridge-and-mat kit crosses the governing small gap and preserves 20 metres after loss of one five-metre panel;
- sealed mobility modules accept a bounded flooded approach;
- the carrier can pull at 1.4 times its own weight and use another `ATUT` as a cooperative recovery anchor;
- receiver ground pressure, width, turn and a 3.25-hour unload remain inside the registered limits.

This does not eliminate specialized route-opening formations. It prevents the strategic terrain carrier from becoming useless whenever the first failed bridge or saturated approach appears before those formations arrive.

## 7. Resilience and lawful limits

Twenty-two behavior worlds test the provisional reference. They include loss of one drive module, energy sector, mobility pod or control lane; loss of route drones; denied network and GNSS; smoke and dust; loss of one bridge panel; saturated soil; grade, side slope, step, gap and water cases; crew casualty; loss of a vehicle; receiver denial; whole-mode denial; simultaneous terrain and atmospheric denial; and withholding representative evidence.

The declared architecture or the independent `HBL-340` path preserves the `DCP-2` public effect in twenty-one worlds. Simultaneous denial of both carriage modes fails by design. The evidence-withheld world is especially important: behavior still calculates as a pass, but current credit remains a fail. Every one of the twenty-two worlds has zero strict evidence credit.

This preserves three different statements:

1. the architecture is internally coherent under declared assumptions;
2. the formation retains a second physics family when the terrain path fails;
3. neither statement is a measured readiness claim.

## 8. Reset and force composition

Six reset paths operate concurrently. The mobility-pod, track and brake path governs at 148 hours. Energy and thermal work closes at 124 hours; structure and deck at 118; route kit at 136; crew and mission-state reconstruction at 44; base, receiver and route handback at 96. The critical path leaves twenty hours to the 168-hour ceiling.

The architecture adds permanent specialties to the `DCP-2` boundary:

| Specialty | Deployed | Affiliated | Minimum watch |
|---|---:|---:|---:|
| Mobility-pod operation and maintenance | 16 | 36 | 6 |
| Route robotics and bridge crew | 20 | 44 | 6 |
| Terrain release and soil mechanics | 8 | 18 | 2 |
| Energy and traction systems | 8 | 18 | 2 |
| Heavy recovery and cooperative tow | 12 | 28 | 4 |
| **Addition** | **64** | **144** | **20** |

The revised configured detachment reaches 592 deployed people, 1,301 affiliated positions and a 194-person minimum watch after the prior `HBL-340` correction. This is an institutional result. A terrain carrier creates professions, release authorities, schools, depots, ranges and technical commands; it cannot be bought as equipment alone.

## 9. Industrial program

Forty-three ready packages require 172 operational vehicles. A twenty-percent reserve adds 35, and the test enterprise adds 12, for 219 total production articles.

The baseline ramp produces no operational articles in years one through four, builds twenty during engineering and manufacturing development in years five through eight, sustains sixteen per year for ten years, and completes reserve production through year 24. Peak output is sixteen vehicles per year.

The industrial system declares:

- three final integration lines;
- three qualified mobility-pod lineages;
- three traction-motor suppliers;
- two energy-system lineages;
- two bridge-and-route-kit lineages;
- four compound test ranges;
- 28,000 peak direct workers;
- 80,000 workers across the wider industrial ecosystem.

This is the kind of demand signal the project means by coequal civil power. The state is not purchasing unusual trucks. It is creating a durable heavy-civil mobility sector with independent design teams, competing energy lineages, manufacturing learning, depot depth, technical education and partner-market potential.

## 10. Cost and fiscal reconciliation

The selected architecture is not the cheapest. `T1` costs less but fails the mission. `T2` costs more and also fails. `T4` is selected because it alone closes the universal behavior boundary.

| Program line | `T4` 25-year value |
|---|---:|
| Ready-set lifecycle | $421.40000B |
| Development and test articles | $23.40000B |
| Reserve vehicles | $50.75000B |
| Architecture research and development | $150.00000B |
| Production tooling | $105.00000B |
| Base capital expansion | $12.04000B |
| Base operating expansion | $12.23694B |
| Full-scale proving | $70.00000B |
| Certification and training | $38.00000B |
| **`ATUT-170` architecture program** | **$882.82694B** |

The Pass 83 `DCP-2` boundary contained a $290.25B generic `ATUT` lifecycle account. Removing that placeholder leaves $1.22698385T of non-`ATUT` program. Adding the full `T4` architecture account produces:

| Boundary | Value |
|---|---:|
| Revised `DCP-2` | $2.10981079T |
| Dynamic one-region `F1-C1` base | $7.38314155T |
| Revised national boundary | $9.49295234T |
| Increase over Pass 83 | $592.57694B |

These are declared research comparators, not forecasts or appropriations estimates. Their value is structural: they prevent a physically rich vehicle from inheriting the cost of a much shallower placeholder.

### 10.1 Concurrency sensitivity

Raising assigned hard-access groups from 22 to 30 increases ready packages from 43 to 59, operational vehicles from 172 to 236, reserve vehicles from 35 to 48 and total articles from 219 to 296. The selected architecture program rises to $1.06751022T, revised `DCP-2` to $2.40960847T and the national boundary to $10.11030522T.

The fixed production schedule still contains 219 articles. The stress case therefore exposes a 77-vehicle capacity gap. The model does not silently assume more lines or a higher rate. A later force-generation decision must choose between a longer build, additional integration capacity, a readiness reduction or a narrower concurrency claim.

## 11. Technology portfolio

Thirteen campaigns receive $260B over twenty-five years:

| Campaign | $B | Decisive coefficient |
|---|---:|---|
| Variable-footprint mobility and low-pressure contact | 28 | ≤35 kPa at 502 t |
| High-torque distributed traction | 22 | grade reserve under weak-soil conditions |
| Active articulation and load leveling | 18 | side-slope and step behavior |
| Soft-soil state sensing | 16 | authoritative route release |
| Modular bridge and mat deployment | 24 | 25 m capacity and 20 m damaged residual |
| Route robotics and scout drones | 18 | four-hour route-work allowance |
| Amphibious wading and sealing | 12 | 2.5 m flooded approach |
| High-specific-energy power plant | 20 | 600 MWh inside the declared mass boundary |
| Self-recovery and cooperative tow | 18 | 1.4 pull ratio |
| Offline convoy autonomy | 12 | four-vehicle movement under network denial |
| Payload deck variants and restraint | 14 | common dry-block and wet-pack handling |
| Production and digital certification | 26 | sixteen vehicles per year across three lines |
| Compound terrain-to-service proving | 32 | complete 800 km mission, unload and reset |

The portfolio illustrates how the Department of Resilience should drive innovation. It does not promise a technological miracle and then hide it in a vehicle line. It isolates the coefficient, funds rival ways to change it, requires representative proof, preserves supplier plurality and carries failure back into force design.

## 12. Evidence program and rendering boundary

The workbook registers one hundred evidence gates:

- forty-eight common gates apply twelve tests to each of the four candidates;
- thirty-two gates open the selected `T4` structure, pods, buses, articulation, sensing, bridge, recovery, convoy, unload, reset and service-chain claims;
- twenty program gates cover integration lines, supplier ancestry, production rate, bases, proving, public release, workforce, fleet and lifecycle recovery.

All are open. The selected reference has behavior-level coherence, not empirical admission.

Rendering remains blocked for a substantive reason. An image would force choices about pod geometry, track or foot form, articulation joints, bridge stowage, energy-plant volume, cooling surfaces, crew station, maintenance access and payload doors. Those choices are precisely the coupled terms still under competition. A rendering now would turn unproved packaging into an apparent design and exert path dependence on later research.

## 13. Implications for the mature Resilience Force

This competition changes the force concept in six ways.

First, inland access becomes a strategic mobility domain. The `ATUT` is not subordinate earthmoving equipment. It carries a complete service cell across a continent-scale damaged route and therefore belongs beside maritime and atmospheric projection in allocation, readiness and industrial policy.

Second, route engineering moves inside the carrier boundary. The force still needs major civil works, but small-gap bridging, bearing assessment, route sensing and recovery must be organic when the carrier’s purpose is to arrive before intact infrastructure can be assumed.

Third, low ground pressure and traction are competing physical demands. A successful system requires controlled contact, not simply more track area or flotation.

Fourth, public-service time governs vehicle design. Load release, route work, unload and receiver build are as important as cruise speed.

Fifth, energy is likely to determine the mature architecture. The current high-specific-energy target may force a different plant, a larger carrier, staged energy exchange, or a two-vehicle propulsion-and-payload pairing. That choice must be made before exterior geometry stabilizes.

Sixth, the industrial base is part of force projection. Three integration lines, plural mobility and energy lineages, national proving ranges, schools, depots and an 80,000-person ecosystem are not implementation details. They are the enduring capacity through which the Department converts repeated environmental failure into technological and economic power.

## 14. Stocktake and next boundary

This pass makes the following authoritative at research maturity `R2`:

- the seven-screen competition method;
- the failure of three single-regime extrapolations under the universal case;
- `T4 SAT-170` as the sole provisional behavior reference;
- the 332-tonne tare, 502-tonne rated-gross and 490.75-tonne mission-gross mass statements;
- the 31.77-kPa pressure, 23.38-hour route, hour-39.38 service and 148-hour reset calculations;
- the 219-article industrial object and $882.82694B architecture account;
- the revised $2.10981079T `DCP-2` and $9.49295234T national boundaries;
- the $260B technology portfolio and one-hundred-gate evidence register.

It does not admit a vehicle, prove deformable-soil mobility, validate the energy system, authorize production, establish safety or stabilize exterior geometry.

The next physical pass should reconcile `GCH-340` and `SAT-170` at their common terrain–air interface. It should allocate receiver zones, payload transfer states, energy exchange, route handoff, maintenance, shared and separated ancestry, and two-mode mission schedules without weakening the custody and loss logic already established. Within that pass, the `SAT-170` energy plant and contact system should be competed one level deeper. Controlled requirements renderings should be reconsidered only if those two terms stop moving.
