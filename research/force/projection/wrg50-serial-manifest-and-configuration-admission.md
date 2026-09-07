# From tonnes to a deployable water force

## WRG-50 serial manifest and configuration admission

The Department of Resilience cannot project water service by moving an aggregate number of tonnes. It must move controlled configurations whose identity, geometry, safety, custody, route, receiving interface, crew and commissioning condition are known before dispatch. Pass 63 applies that rule to `WRG-50`, the project's first complete formation hypothesis for restoring 50,000 cubic metres of potable water per day. The result is the first attempt to compile one major mission formation from an engineering mass estimate into a serial movement and receiving problem.

The source model is useful and incomplete in a specific way. It balances treatment, conveyance, storage, distribution, wastewater, workforce and broad lift demand. Its sixteen preliminary equipment lines total 20,448.845 tonnes before a 15 percent contingency and 23,516.172 tonnes after it. Those quantities establish that water restoration is a major-force problem. They do not yet describe assets that a carrier, transfer node or receiver can admit.

Expanding each source quantity unit produces 690 planning objects. Under the inherited 40-tonne land and rail position screen, 560 objects fit by both mass and chargeable transport burden. A clean-sheet 120-tonne land and rail target raises mass fit to 689 objects, but chargeable fit reaches only 686 because three low-density break-tank packages consume more position capacity by volume than by weight. Even then, zero objects pass strict dispatch admission and zero pass receiver admission. The source provides no released configurations, measured packed dimensions, centres of gravity, restraint designs, hazard determinations, origins, carrier reservations, node slots, routes, receiving sites or commissioning acceptances.

This is not a verdict against `WRG-50`. It is a decision about what must be designed next. The force needs an acquisition system that treats packaging, external interfaces and receiver preparation as coequal with process performance. A 350-tonne treatment train that produces the right water quality but cannot be lifted, restrained, routed, discharged, connected or operated at a named site is not projected water service. A pipe mass allowance without a credible transport form is not a pipeline force. A percentage contingency without named reserve objects is not resilience.

The companion [serial manifest and admission model](../../../models/force/projection/wrg50-serial-manifest-and-admission-model.xlsx) preserves all 690 planning objects, the two rival carrier-position screens, six service-chain complements, four declared arrival waves, a twenty-eight-field release protocol, four transfer-node contracts, one receiver contract and twenty-six terminal integrity checks. It carries every failure rather than filling missing fields with optimistic assumptions. No rendering is authorized.

## Executive judgment

Five conclusions govern the next design stage.

First, **the current manifest is a mass estimate, not a configuration baseline**. Sixteen aggregate lines are sufficient for early force sizing and insufficient for movement scheduling or acquisition. The word `set` conceals the most extreme example: one 424.464-tonne allowance for fittings, valves, anchors and bypass reserve. Treating that line as one object produces an obvious position failure. Treating it as divisible without specifying functional sublots would be equally misleading. The correct next object is a controlled bill of material that preserves which valves, anchors, joints, tools, test equipment and spares must arrive together for a particular reach.

Second, **a larger carrier position solves only part of the problem**. Raising the land and rail screen from 40 to 120 tonnes changes the mass result from 560 to 689 fitting objects. It does not supply dimensions, axle loads, route clearances, handling devices, lift points or receiver surfaces. It also leaves four chargeable objects outside the position envelope: the fitting set and three break-tank packages. The fitting set binds on mass. Each break-tank package binds on cube. Clean-sheet mobility should therefore be competed together with modularity and transport-form design rather than sized around inherited aggregate packages.

Third, **the pipe line contains a physical contradiction that invalidates its cube claim**. The source calculates 53.058 tonnes of polyethylene per kilometre. At the declared material density of 0.95 tonnes per cubic metre, the pipe material alone occupies about 55.85 cubic metres per kilometre. The manifest assigns only 18 cubic metres per kilometre of transport cube. Packed cube cannot be smaller than material volume. The source value is therefore invalid before allowing for voids, curvature, reels, cradles, joint protection or handling clearances. The model retains the value to expose the contradiction, but no carrier or warehouse decision may use it as physical evidence.

Fourth, **the contingency line cannot be scheduled**. The difference between the source base and contingent totals is 3,067.327 tonnes. It has no item identities, cube, complement, mode, deadline, origin or receiver. It cannot replace a missing treatment train, repair a failed pipe reach or restore a contaminated intake merely because its mass equals 15 percent of the formation. A mature force would hold configuration reserves against named failure modes, with preservation, custody, transport and regeneration obligations.

Fifth, **receiver admission is the final unit of force projection**. All carrier-fit calculations remain planning screens. Water service still requires a source-water envelope, intake authority, concentrate and wastewater paths, power protection, pipeline corridor, sanitary storage, operating workforce, independent product-water release and civil acceptance. None is attached to a named site. The correct current service result is therefore zero, not a discounted fraction of 50,000 cubic metres per day.

## 1. What is being compiled

`WRG-50` is designed around a public effect: temporary potable-water service at 50,000 cubic metres per day, sufficient for a reference population of one million people at 50 litres per person per day. Its [configuration study](../../systems/water/configuration-model.md) works backward through treatment, intake, 50 kilometres of twin trunk conveyance, pressure management, storage, distribution access, quality surveillance, sanitation, energy, construction, sustainment and transfer. The source workbook assigns 110 kilometres of pipe including reserve, six treatment trains, six intake modules, four boosters, three break-tank packages, eight laboratories, eight storage-hardware sets, 111 district interfaces, nine wastewater trains, sixty route-work machines, 220 vehicles, three power modules, 120 support modules, twenty spare packages and one consumables lot.

Those quantities do not share a common ontology. A vehicle is plausibly one physical asset. A kilometre is work and material that may be divided among sticks, reels, coils, joining stations and support frames. A `set` is an accounting boundary. A `lot` is a supply allowance. A treatment `train` may be one integrated structure, several skids or dozens of interdependent positions. Serial expansion therefore produces **planning objects**, not an assertion that `WRG-50` consists of exactly 690 acquired assets.

That distinction matters for both undercounting and overcounting. One planning object may conceal many transport positions. Several planning objects may travel as one controlled unit. The serial register creates stable placeholders so every implied unit can carry evidence and cannot disappear inside a subtotal. It does not grant configuration maturity merely by assigning an identifier.

The compiler applies five successive boundaries:

1. preserve the source quantity, mass, cube, primary-lift and basis;
2. map the line provisionally to an external cargo class, service complement and latest-arrival wave;
3. calculate mass-only and chargeable-position fit against two rival carrier screens;
4. require a complete twenty-eight-field object release before dispatch; and
5. require compatible node and receiver contracts before public-effect credit.

Each boundary can reject the prior result. A configuration that fits a position can still fail safety. A safe configuration can still lack a carrier or route. A delivered object can still fail at the receiver. The sequence prevents analytical convenience from becoming operational credit.

## 2. The chargeable-position rule

Physical mass is necessary and not always binding. Aircraft, ships, rail consists, trailers, nodes and staging areas also consume space. Pass 61 introduced external position classes; Pass 62 carried mode-level density floors into rival carrier requirements. This pass applies the same principle at source-unit level.

For planning object `i` assigned to mode `m`, chargeable transport burden is:

```text
CCT(i) = max[ physical mass(i), packed cube(i) × density floor(m) ]
```

The declared floors are 0.25 tonnes per cubic metre for air, 0.15 for sealift and 0.20 for rail and road. They are comparison controls, not measured vehicle envelopes. A planning object fits rival `r` only when its unit mass or chargeable burden is less than or equal to the rival's position capacity:

```text
mass_fit(i,r) = 1[ mass(i) ≤ position_capacity(m,r) ]
CCT_fit(i,r)  = 1[ CCT(i)  ≤ position_capacity(m,r) ]
```

The standard rival retains the Pass 62 screens: 180 tonnes for air, 20,000 tonnes for sealift and 40 tonnes for rail and road. The heavy rival keeps the air and sealift screens but raises rail and road to 120 tonnes as a clean-sheet technology target. The number is not a truck or railcar specification. It asks whether a materially heavier continental carriage system would remove the formation's most obvious unit-level discontinuities.

Across the source manifest, physical mass totals 20,448.845 tonnes. The declared cubes total 66,098 cubic metres. Applying density floors raises chargeable burden to 20,775.445 tonnes. The 326.600-tonne difference comes from low-density break-tank hardware, storage hardware and district-interface packages. Because the pipe cube is invalid, even that chargeable total is a lower-quality planning value rather than a final demand.

### Standard screen

The standard rival fits all eight air planning objects and all 361 sealift objects. Rail fits sixty route-work machines and rejects 110 kilometre-units of pipe plus three power modules. Road fits 131 objects and rejects seventeen: one fittings set, four booster packages, three break-tank packages, eight storage-hardware sets and one consumables lot.

The result is 560 of 690 objects, or 81.2 percent by count. Those objects carry only 12,453 tonnes of physical mass, or 60.9 percent of the formation. On a chargeable basis they cover 12,519.600 of 20,775.445 tonnes, or 60.3 percent. Count therefore overstates closure because the rejected objects are unusually heavy and functionally central.

Only three of six chargeable service complements close: source works and quality, sanitation, and sustainment. Treatment fails because the consumables lot is oversized for its assigned road position. Conveyance fails on pipe, fittings, boosters, break tanks and power. Storage and distribution fails on storage hardware. A formation-level answer based on 81.2 percent object count would be wrong; the weakest-complement answer is zero complete `WRG-50` formations.

### Heavy target

The heavy rival changes the surface result sharply. Every rail planning object fits both mass and chargeable screens. On road, 147 of 148 objects fit by mass, with only the fitting set rejected. Chargeable fit falls to 144 because each 120-tonne break-tank package carries 900 cubic metres of declared volume and therefore consumes 180 chargeable tonnes.

The mass-only result is 689 of 690 objects, 20,024.381 tonnes, or 97.9 percent of source mass. The chargeable result is 686 objects carrying 19,664.381 tonnes of physical mass and 19,810.981 chargeable tonnes. That equals 99.4 percent of objects, 96.2 percent of physical mass and 95.4 percent of chargeable burden. Those are strong screening results and still do not close the formation.

Five complements close on chargeable fit. Conveyance remains open because its fittings and break tanks do not fit as declared. Under weakest-complement doctrine, the entire formation remains unavailable. This is exactly the kind of discontinuity a mass-only national model hides: more than 95 percent of burden can arrive while the system produces no admitted service because a small number of indispensable interfaces are absent.

### Divisibility is a design claim

The workbook also reports the theoretical minimum number of positions if each source unit could be divided perfectly. Under the standard screen, the 110 pipe kilometre-units require at least 220 positions, the fitting set eleven, booster packages twelve, break tanks fifteen, storage sets twenty-four, power modules six and the consumables lot three. Under the heavy target, the fitting set requires at least four positions and the three break-tank packages at least six.

These counts are lower bounds, not transport plans. They assume that mass and cube can be divided without duplicating frames, controls, pumps, tools, protection or crew. They also assume every sublot preserves a useful mission function. The acquisition authority must define legal cuts. A valve package for reach three cannot be credited merely because a different reach received an equal mass of fittings. A treatment train divided across four skids does not operate until all required skids, connections, controls and commissioning materials close at the same receiver.

## 3. Strict configuration admission

The central advance in this pass is a release protocol, not another capacity coefficient. Each object requires twenty-eight fields:

- stable identity, configuration revision and verified unit meaning;
- measured as-packed mass, length, width, height, cube and three-axis centre of gravity;
- rated lift and tie-down points, approved restraint and named handling equipment;
- hazard, temperature, external-power, contamination and decontamination conditions;
- released cargo class, complement membership and eligible or prohibited modes;
- origin, custody, carrier reservation, node slot and cleared route;
- named receiver, crew and current qualifications;
- configuration-ready time, mission-approved required-arrival time and independent inspection release; and
- regeneration disposition after use.

The protocol distinguishes `SOURCE_VALUE`, `DERIVED`, `DECLARED`, `UNKNOWN`, `INVALID` and `VERIFIED`. Only the final state satisfies strict release. A source value may be useful and remain unverified. A derived identifier creates traceability and remains outside configuration control. A declared deadline is a research allocation until the mission authority owns it. An invalid value cannot be repaired by optimistic formatting.

For object `i`, strict dispatch admission is:

```text
dispatch(i,r) = CCT_fit(i,r)
                × product over all required fields f of 1[state(i,f) = VERIFIED]
                × 1[carrier, node and route reservations are mutually consistent]
```

Receiver admission adds a compatible site contract and commissioning release:

```text
service(i,r,s) = dispatch(i,r)
                 × receiver_compatible(i,s)
                 × commissioned(i,s)
```

No field in the source reaches `VERIFIED` under this protocol. The serial register therefore denies all 690 dispatches under both rivals. This is not the assertion that every source claim is false. It is the narrower and more defensible assertion that none currently carries the evidence required to release a real load.

The distinction protects the program from two common acquisition failures. The first is designing a technically capable plant and discovering transport and site incompatibilities late. The second is buying mobility capacity against assumed loads that later change shape, weight, hazard or handling class. Configuration admission forces mission equipment and movement systems to co-evolve.

## 4. Complement preservation

`WRG-50` is divided into six service-chain complements:

| Complement | Required function |
|---|---|
| `C01` | source works, intake and independent quality release |
| `C02` | potable treatment and required consumables |
| `C03` | conveyance, fittings, pressure management, construction and power |
| `C04` | sanitary storage, public distribution interfaces and organic mobility |
| `C05` | wastewater treatment and lawful residual path |
| `C06` | camp, workshop, warehouse and repair sustainment |

Complement closure is binary at this stage. If a future trial demonstrates a lawful degraded effect, that effect must receive its own population, service level, duration, excluded functions and safety limits. The model does not infer partial potable-water service from delivered mass.

The heavy rival's five-of-six result illustrates why complement identity must survive every queue. A transfer node optimizing tonnes per hour might leave the fittings set behind because it is awkward and move several easy vehicles instead. Its throughput report would improve while the water formation became less complete. The carrier, node and receiving systems need priority logic based on weakest complement and required arrival, not just mass or utilization.

Configuration reserves must also belong to complements. The source's 3,067.327-tonne contingency cannot be credited to all six simultaneously. A valid reserve register would state, for example, which pipe damage modes it covers, which pumps or drives it replaces, whether chemical stocks match the chosen treatment process, where the reserve resides, what carrier position it consumes and how it is restored after issue.

## 5. Arrival waves without invented readiness

The source deployment plan describes first entry at 0–24 hours, critical service at 24–72 hours, network build during days three through ten, regional service during days seven through twenty-one, and transfer during weeks three through twenty-six. It does not assign specific source lines or serial objects to those phases.

Pass 63 makes a conservative research allocation using whole lines:

| Latest arrival | Research allocation | Objects | Physical t | Chargeable t |
|---:|---|---:|---:|---:|
| 24 h | laboratories | 8 | 200.000 | 200.000 |
| 72 h | treatment, intake, power and consumables | 16 | 2,895.000 | 2,895.000 |
| 240 h | pipe, fittings, boosters, break tanks and work machines | 178 | 8,880.845 | 9,060.845 |
| 504 h | storage, interfaces, wastewater, vehicles, support and spares | 488 | 8,473.000 | 8,619.600 |

The allocation exposes rather than solves the schedule. The 24-hour source narrative also names command, survey and liaison functions that are absent from the equipment manifest. The 72-hour wave includes treatment, but `WRG-50` cannot deliver regional service without a constructed conveyance and distribution chain. Some line quantities would almost certainly split across waves. The research allocation refuses to manufacture those fractions before a reach-level bill of material exists.

The next schedule must be generated backward from commissioning. Every receiver work package should identify its critical path: source authorization, site possession, earthworks, intake, power, treatment, product-water release, trunk segment, pressure control, storage, distribution access, wastewater, operating crew and public handoff. Object arrival times should then follow those dependencies. The force should not celebrate an early treatment-train arrival if its intake, electrical protection or discharge package remains in a later convoy.

## 6. Nodes and receivers as acquired systems

Pass 62 established that transfer nodes are coequal platforms in the strategic-mobility enterprise. This pass states what that means for `WRG-50`. Every air, sealift, rail and road node requires thirteen fields: location and authority, activation time, operating surface and geometry, lifting and handling, cold/hazard/outsize areas, external power, fluid containment, labor and qualifications, measured mixed-cargo throughput, onward route, manual fallback, safety release and a reserved queue slot. All fifty-two mode-field records are currently unknown.

The receiver contract is more demanding because it owns service rather than cargo release. It requires a named site and civil authority; possession for the operating duration; final-access and hardstand conditions; source-water quantity, chemistry and authority; concentrate and wastewater acceptance; power intertie and protection; surveyed pipeline corridor; sanitary storage site; independent laboratory release; credentialed operating shifts; integrated safety and environmental approval; commissioning acceptance; and demobilization, transfer and site restoration. All sixteen fields are unknown.

This should change how the Department organizes investment. A prepared receiver is not merely a local permitting exercise. It is a latent national-power asset. The Establishment should acquire and maintain receiver interfaces in threatened domestic regions and, by agreement, with partners. A water receiver might include surveyed and legally preserved utility corridors, protected intake and discharge points, heavy pads, standardized electrical and wet interfaces, sanitary storage footprints, laboratory space, pre-negotiated operating authorities and trained local cadres. The mobile force then projects scarce plant and labor into a site already able to absorb them.

Prepared receivers do not eliminate expeditionary capability. Disasters can invalidate planned sites, and international missions may begin with little preparation. They create rivals that can be tested: a highly prepared fixed anchor, an austere rapidly constructed receiver, and a maritime or inland-water interface that performs some functions afloat. The winning architecture may vary by geography. Every rival must still close the same public-service contract.

## 7. Industrial architecture implied by the failure

The configuration gap defines an industrial economy that does not exist at required scale. A defense-scale Department of Resilience would not ask each emergency team to improvise transport paperwork after a disaster. It would build permanent design, certification, production and test institutions.

### Mission-system configuration bureaus

Each generating service needs a bureau that owns the complete formation baseline. For water, it would control every plant, pipe, fitting, power, laboratory, sanitation, vehicle, tool, software and consumable configuration; the legal subdivisions of each package; and the interfaces required to recombine them. The bureau would maintain as-designed, as-built, as-packed, as-loaded, as-delivered and as-regenerated states. It would have authority to reject changes that improve a component while breaking mobility or receiver compatibility.

### Independent load-certification authorities

Carrier operators should not certify the cargo they are pressured to move. Independent authorities would measure mass and geometry, determine centre of gravity, approve lift points and restraint, control hazards, witness proof loads and certify eligible modes. Their data would feed a digital load library available to origin, carrier, node and receiver planners. Automated scanning can reduce friction, but the legal and engineering release remains institutional.

### Position and interface primes

The Department should create major acquisition programs around position families, not only end platforms. Companies at the scale imagined for clean-sheet ships and aircraft would compete modular plant frames, long-load systems, fluid modules, rolling machines, energy modules, cold and laboratory positions, and outsize structures. They would also produce common handling, connection, sensing and condition-monitoring systems. The prize is not a universal box. It is a governed family of external interfaces that lets different mission systems share carriers and nodes without sharing hidden failure modes.

### Receiver and node arsenals

Public shipyards, depots and private primes would build deployable transfer-node sets and receiver kits: rapid heavy surfaces, autonomous cranes and movers, fluid containment, temporary railheads, no-pier discharge, power islands, potable manifolds, laboratories, route-survey systems and manual fallbacks. The Department would keep enough public production and maintenance capacity to prevent a small supplier group from controlling readiness.

### Configuration reserve enterprises

Reserve production would be tied to failure distributions and regeneration time. Pipe plants, membrane lines, pump and drive factories, power-module lines, chemical suppliers and structural-system producers would maintain surge tooling and qualified labor. Some reserves would be physical stocks. Others would be protected production capacity with exercised lead times and allocated raw materials. Both require auditable claims; neither is created by adding 15 percent to a spreadsheet total.

## 8. Technology competitions pulled by `WRG-50`

The failure record supports ambitious technical programs. It does not yet select their form.

### 8.1 A rapid main-conveyance family

The largest line is 110 kilometres of nominal 0.5-metre internal-diameter pipe including reserve. The source geometry implies 5,836.381 tonnes. Its invalid cube prevents a carrier decision. The Department should compete at least four transport-and-installation architectures:

1. factory-produced sectional mains with automated joining, inspection and long-load carriers;
2. large-reel or segmented-coil systems that trade material and pressure limits against installation speed;
3. mobile field extrusion or continuous manufacture using transported resin and distributed quality control; and
4. foldable, lined or composite conduits designed for rapid low-to-moderate pressure service and later replacement.

The competition should score the complete reach: material supply, transport cube, carrier positions, route clearance, lay rate, joints, anchors, crossings, pressure and surge, contamination protection, repair, recovery and residual waste. A low-mass pipe that requires slow joining may lose. A bulky reel that enables continuous lay may win in one terrain and fail in another. The acquisition object is the source-to-receiver reach, not the pipe material alone.

### 8.2 Distributed pressure and tank modules

Booster and break-tank packages drive surface-position failures. Clean-sheet rivals should include self-deploying tank structures, modular pressure-control cells, integrated manifolds, autonomous level and quality control, and foundations that minimize site work. Their transport state must be part of performance. A 900-cubic-metre package that unfolds at the site is different from a 900-cubic-metre rigid transport volume; the current source does not distinguish them.

### 8.3 Treatment trains designed around movement

The six 350-tonne treatment trains fit the coarse 20,000-tonne sealift screen only because that screen is far larger than the object. They remain outsize plants without dimensions or handling. The Department should compete train architectures around a specified commissioning bundle: process skids, pretreatment, product-water protection, controls, chemicals, laboratory interfaces, maintenance access, black start, waste handling and crew. Critical early output may justify smaller replicated trains even if total plant mass rises, because smaller units improve air or land optionality and graceful degradation.

### 8.4 Power modules as a defined hazard class

The source names three five-megawatt modules and assigns them to rail. It does not specify whether they are combustion, storage, fuel-cell, reactor-coupled or mixed systems. Cargo class cannot be inferred from output alone. The power competition should bind technology to fuel or charging logistics, protection, black start, harmonics, thermal rejection, emissions, fire behavior, acoustic limits, maintenance and receiver intertie. The module's transport and operating safety cases should mature together.

### 8.5 Consumables without the `lot` abstraction

Thirty days of treatment consumables appear as one 105-tonne, 400-cubic-metre road lot. The chemical identities, hazard divisions, temperature limits, segregation rules and replenishment cadence are absent. Process competitions should report consumables by chemical and package configuration, including regeneration or substitution options. A lower-energy treatment process may be inferior if its reagent chain is fragile; a heavier process may be preferable if it uses widely available and safely handled inputs.

### 8.6 A live configuration and mission twin

The digital system should not be a visualization layer. It should hold object identity, configuration revision, measured envelope, condition, custody, complement, required arrival, carrier and node reservation, route, receiver interface and regeneration state. It should prevent the same carrier position or reserve package from being claimed by multiple campaigns. It should show when a late indispensable fitting reduces a nominally delivered formation to zero. Automated planning earns authority only after its data and release rules survive physical trials.

## 9. The next proof object

Attempting to validate all 690 planning objects at once would reproduce the aggregate problem at a larger scale. The next proof should be a complete **10-kilometre first-reach water system** capable of sustained, independently released public service. Ten kilometres sets a material transport problem large enough to expose pipe form, joining, crossings, construction support and pressure management while remaining suitable for repeated instrumented trials. The service rate, source chemistry, pressure profile and public-use points should be selected before the bill of material is frozen rather than obtained by mechanically scaling every `WRG-50` line.

The trial must include:

- one named source and one named receiver under civil authority;
- a source-to-use chain with intake, treatment, quality release, power, conveyance, pressure control, storage, accessible distribution and wastewater or residual handling;
- at least two rival pipe transport and installation forms;
- released serial configurations with measured mass, dimensions, cube, centre of gravity, lifting, restraint, hazards and handling;
- origin custody, no-notice readiness, carrier positions, node slots and cleared routes;
- assembly and commissioning under a timed service contract;
- seven days of degraded operation with seeded component, power, communications and route failures; and
- disassembly, decontamination, return, repair and restoration to readiness before a second activation.

The primary measures should be time to independently released water at public-use points; population and service level sustained; weakest-complement completeness; labour hours and qualification bottlenecks; chargeable carrier positions by class; node queue and release time; installation and repair rates; energy and consumables; water loss and quality; receiver work and footprint; safety events; and regeneration time. Cost belongs in the test record but cannot override a failed public-service or safety gate.

The proof should preserve at least three failure outcomes. First, every transport rival may fail the service time. Second, a technically superior pipe form may lose when receiver and repair burdens are included. Third, the current `WRG-50` architecture itself may be rejected in favour of smaller distributed formations, greater prepared infrastructure or a different allocation between mobile and fixed systems. The purpose of the trial is to discover the force, not validate a preferred illustration.

## 10. Decisions warranted now

This pass warrants six program decisions.

1. Establish serial configuration, external-interface and receiver admission as mandatory gates for every canonical formation.
2. Treat the 120-tonne land and rail position as a research target, not a selected vehicle, and compete it against finer modularity and prepared receivers.
3. Suspend use of the `WRG-50` pipe cube in carrier, node, warehouse and cost models until a physical transport form is measured.
4. Replace percentage contingency in future formation releases with named reserve configurations allocated to complements and failure modes.
5. Fund the 10-kilometre first-reach competition as the next representative water proof rather than drawing a mature `WRG-50` platform.
6. Keep all `WRG-50` rendering blocked until a complete configuration survives carrier, node, receiver, operation and regeneration evidence.

The pass does not warrant a procurement quantity, platform selection, validated deployment time, receiver inventory or public-service claim. Its carrier positions are comparison screens. Its cargo classes and arrival waves are provisional mappings. Its 690 identities are planning controls. Twenty-six integrity checks show that the workbook calculates what it says; they do not convert unknown evidence into proof.

## Conclusion

Defense-scale civil power requires the discipline to know what the force is before deciding what moves it. `WRG-50` began as a coherent service-chain hypothesis with a large but manageable aggregate mass. Serial compilation reveals a different object: a coupled industrial system whose performance depends on packaging, configuration control, position geometry, hazardous-material release, origin readiness, transfer nodes, receiving infrastructure, crew and civil commissioning.

The heavy carrier target is valuable because it exposes where capacity helps and where it does not. It moves the screen from 560 to 686 chargeable-fit objects and closes five of six complements. The remaining four objects still deny the formation, and none of the 690 can yet be dispatched under strict evidence. That is not excessive caution. It is the point at which a conceptual force begins to behave like a real one.

The next generation of disaster-response primes should therefore build more than large ships, aircraft and vehicles. They should build complete, certifiable mission configurations; the nodes that release them; the receivers that turn them into public service; and the production and regeneration system that keeps them ready for the next catastrophe. Once those requirements are measured, the exterior form will follow. Until then, the most honest rendering of `WRG-50` is its unresolved configuration.

## Internal authorities

- [WRG-50 configuration study](../../systems/water/configuration-model.md)
- [WRG-50 engineering workbook](../../../models/systems/water/water-restoration-engineering.xlsx)
- [Canonical cargo and transport closure](canonical-cargo-and-transport-closure.md)
- [Carrier-node requirements and industrial program](carrier-node-requirements-and-industrial-program.md)
- [Common technical architecture](../../systems/common-technical-architecture.md)
- [Department force architecture](../force-architecture.md)

