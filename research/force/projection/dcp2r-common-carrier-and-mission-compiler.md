# `DCP-2R`: common carrier and mission compiler

## A compound-assurance behavior reference for projected civilian service

## Executive judgment

The present two-mode deployment concept is necessary but not sufficient for a mature Resilience Force. The existing `DCP-2` architecture establishes an important single-cut guarantee: one 635-tonne public-service cell may arrive through the atmosphere and another over damaged terrain, and loss of either access physics family does not eliminate the other. That is a legitimate lower bound. It does not, however, guarantee that the surviving mode can absorb a further carrier or payload casualty while still producing the complete civilian effect.

This pass therefore asks a harder question: what formation, payload and receiver architecture can lose an entire carriage mode, then lose one vehicle and one functional payload element within the surviving mode, and still create the same independently assayed public service by absolute hour 54?

The answer is not simply “buy more carriers.” Additional vehicles create reserve mass, but exact specialized payload blocks can still leave the surviving formation without water treatment, black start, heat rejection, distribution, assay or another irreplaceable function. Functional reserve requires the service effect itself to be distributed across the carriers.

The selected behavior reference is `DCP-2R`, a deliberately ambitious successor architecture built around an **Adaptive Service Kernel**, or `ESK-40`. One complete service effect is represented by forty 15.875-tonne physical tiles divided equally among five functional families:

- `E`: energy, conversion, storage and protection;
- `W`: safe water, wastewater and residual custody;
- `T`: useful thermal service and final heat rejection;
- `D`: electrical, fluid and building distribution; and
- `C`: civil control, communications, assay, medical access and repair.

Eight tiles from every family produce the canonical 635-tonne kernel. Each tile is assigned a provisional coefficient of 14.285714 service units, so seven surviving tiles retain the 100-unit family floor. The atmospheric formation carries three `GCH-340R` vehicles, each with four tiles from every family. Any two vehicles therefore retain forty tiles and eight from every family. The terrain formation carries five `SAT-170R` vehicles, each with two tiles from every family. Any four likewise retain the same forty-tile kernel. After the vehicle casualty, one further tile may be rejected while its family still meets the service floor.

This is physical functional coding, not digital parity and not a claim that unlike machines are interchangeable. It is a technology hypothesis about multi-effect modules, fluid and energy custody, contained failure, rapid connection and receiver-side recomposition. Air and terrain tiles share service semantics and civil interfaces, but they must use separate physical designs, suppliers, control kernels, energy lineages and certifying authorities. Otherwise the apparently diverse force inherits a common decisive cause.

Under the declared boundary, `DCP-2R` requires three air and five terrain carriers per ready formation; 439 total carrier articles; 906 deployed personnel, 2,031 affiliated positions and a minimum watch of 284; a 25-year `DCP-2R` program envelope of **$4.94079719 trillion**; and a resulting national program boundary of **$12.32393874 trillion**. It costs $1.16349609 trillion more than the Pass 87 `DCP-2` boundary but $1.06307905 trillion less than duplicating two complete exact-block formations. The saving is conditional on the `ESK-40` premise. It disappears if multifunction coefficients, independence or field recomposition do not prove real.

The workbook tests six architectures through 24 non-substitutable gates. Only `DCP-2R` and full exact-cell duplication pass all 24. The selected architecture then passes 28 deterministic mission worlds inside the proposed compound guarantee. Four deliberately harder probes remain labeled `BOUND`; they receive no assurance credit. Seventy model controls and 160 evidence-state controls pass, while all 160 physical evidence gates remain open. The arithmetic reconciles. The technology does not yet exist at the claimed standard.

The next decisive research object is therefore not an exterior carrier rendering. It is a representative five-family tile set in two independent physical lineages, followed by a ten-tile terrain load, a twenty-tile air load, and a destructive receiver trial that removes one carrier and one additional tile. Vehicle imagery remains blocked until that burden is physically intelligible.

## 1. From access redundancy to compound service assurance

The force-projection chain has progressively replaced movement abstractions with public-service obligations. The [public-service pod](service-entry-pod-configuration.md) rejected fractional cargo credit. The [canonical cargo closure](canonical-cargo-and-transport-closure.md) made carriers answer to complete deployable positions. The [`DCP-2` physical configuration](tafg1-dcp2-physical-configuration.md) required two independent 635-tonne service cells. The [`SAT-170R` closure](sat170r-internal-architecture-and-coupled-closure.md) and [`GCH-340R` closure](gch340-complete-system-and-transient-closure.md) then made each carriage mode pay for its own mass, energy, ground interaction, crew, receiver and reset.

Those steps established two physically different ways to bring the same nominal payload to public service. The remaining ambiguity concerned the guarantee itself.

Let one complete public-service effect be `S`, with mass `M_S = 635 t`. Let the air and terrain paths be `A` and `T`. The single-cut `DCP-2` requirement can be written:

```text
loss(A) => T delivers S
loss(T) => A delivers S
```

This is valuable. It prevents weather, airspace, terrain, bridge, route or receiver conditions associated with one physical mode from becoming a universal stop. But a mature national force must also distinguish a mode cut from a carrier cut. A mode may survive while one of its vehicles is rejected at origin, lost en route, quarantined at the receiver or unable to unload. A payload element may then fail assay or become unavailable after that vehicle loss.

The proposed compound guarantee is:

```text
loss(A) + loss(one terrain carrier) + loss(one surviving terrain tile)
    => T still delivers S by hour 54

loss(T) + loss(one air carrier) + loss(one surviving air tile)
    => A still delivers S by hour 54
```

The requirement does not claim survival after any number of losses. It makes the admitted casualty set explicit. A two-air-carrier loss after the terrain mode has disappeared, a two-terrain-carrier loss after the air mode has disappeared, simultaneous loss of both modes, or two additional family-tile losses are outside the present guarantee. The challenge lattice labels those cases `BOUND` instead of quietly treating them as successful or statistically unlikely.

That distinction matters institutionally. A force that calls every conceivable case “required” becomes unaffordable and untestable. A force that leaves the casualty set implicit can claim resilience without owning any particular failure. `DCP-2R` defines a severe but finite constitutional promise and exposes what the promise costs.

## 2. Equal depth does not mean identical machines

The two carriers now meet at comparable analytical depth. The atmospheric `GCH-340R` reference has a rated gross mass of 1,461.415 tonnes, an assigned 317.5-tonne service payload per carrier, 2,185.075 megawatt-hours of deliverable onboard energy, twenty-four lift cells, six conversion trains, twelve propulsion pods and sixteen contact feet. Its governing transition is a cold-dense unload: lift hydrogen must be converted into contained water to preserve ground reaction while payload leaves the vehicle.

The terrain `SAT-170R` reference has 705.935 tonnes assigned gross per carrier, a 158.75-tonne service payload, 667.031 megawatt-hours onboard, four rigid bodies, mirrored energy citadels, dual crew refuges, split-keel bridge stowage and 285 square metres of ground contact. Its governing problems are complete-system energy mass, deformable-soil contact, route opening and bridge-cycle reset.

The air vehicle therefore carries twice the service payload of the terrain vehicle, and the reinforced formation uses three air carriers versus five terrain carriers. This is not a preference for aviation. It follows the carrier payload quanta already closed in Passes 86 and 87:

| Quantity | Atmospheric path | Terrain path |
| --- | ---: | ---: |
| Assigned payload per vehicle | 317.5 t | 158.75 t |
| Tiles per vehicle | 20 | 10 |
| Reinforced formation | 3 vehicles | 5 vehicles |
| Surviving quorum | 2 vehicles | 4 vehicles |
| Payload in surviving quorum | 635 t | 635 t |
| Relative public service | 41.917 h | 43.569 h |
| Absolute public service | 47.917 h | 49.569 h |
| Declared reset | 162 h | 166 h |

Equal depth means that both paths answer the same questions: complete departure state, energy custody, route or flight state, survivor selection, unloading, receiver admission, service assembly, assay, civil release, crew, reset and evidence. It does not force the same machinery or a cosmetic family resemblance. The force wants common service meaning across different physical failure families.

## 3. Why another vehicle is not enough

Suppose the current exact 635-tonne service cell contains specialized blocks for power, water, thermal control, distribution and civil control. Splitting those blocks over two air carriers or four terrain carriers can create a complete nominal formation. Adding a third air carrier or fifth terrain carrier creates extra payload capacity after one vehicle is lost: 635 tonnes remain in either mode. But retained mass alone says nothing about the distribution of irreplaceable functions.

If the added carrier holds general spares, the lost carrier may still contain the only treatment train or final heat sink. If it holds duplicates of one or two dominant blocks, another carrier loss may expose a different family. If the exact blocks are divided more finely, the force has already begun to move toward a new payload grammar. There is no allocation of indivisible, single-function blocks that guarantees every two-of-three air subset and every four-of-five terrain subset contains the full service vector unless every decisive block is duplicated broadly enough to approach full-cell duplication.

The architecture competition makes this visible:

| Candidate | Formation | Payload grammar | 24-gate result | Judgment |
| --- | --- | --- | ---: | --- |
| `P1` | 2 air / 4 terrain | current exact blocks | 13 | valid single-cut lower bound; not compound assured |
| `P2` | 3 air / 5 terrain | exact blocks unchanged | 15 | reserve mass without functional reserve |
| `P3` | 2 air / 4 terrain | `ESK-40` | 15 | adaptive payload but inadequate mass after vehicle loss |
| `P4` | 3 air / 5 terrain | `ESK-40` | 24 | selected compound-assurance reference |
| `P5` | 4 air / 8 terrain | duplicated exact cells | 24 | complete but materially larger and costlier control |
| `P6` | 2 air / 4 terrain | exact blocks plus utility bridge | 13 | bridge depends on an independently qualified local source |

`P2` is the critical negative case. It proves why fleet expansion cannot be credited as resilience by itself. `P3` proves the converse: payload adaptability cannot overcome a simple shortage of surviving mass. `P6` clarifies the role of local infrastructure. A prepared utility bridge can be useful, but it is conditional on a source, route, authority and receiver that remain available. It cannot close a universal source-independent guarantee.

`P5` is not absurd. Full duplication is the conservative engineering control and may ultimately win if multifunction tiles fail. Its purpose is to price the alternative honestly. `P4` is preferred because it seeks the same deterministic behavior with 439 total carrier articles rather than 646 and a program boundary $1.063 trillion lower. That preference is an option on successful research, not evidence that the option will succeed.

## 4. `ESK-40` as physical functional coding

The adaptive service kernel treats every family as a population of repeated physical contributors rather than a single exquisite plant. Forty tiles form one service effect: eight `E`, eight `W`, eight `T`, eight `D` and eight `C`. Each tile has an assigned integrated mass of 15.875 tonnes, including its share of structure, connectors, working fluids, reagents, controls, safety, tools and custody loads.

The provisional capacity algebra is simple:

```text
8 tiles/family × 14.285714 service units/tile = 114.285712 units
7 surviving tiles × 14.285714 service units/tile = 100 units
5 families × 8 tiles × 15.875 t = 635 t
```

The arithmetic creates an explicit margin for one tile loss. It does not establish that a 15.875-tonne module can perform the assigned work. “Service unit” is a normalized family coefficient used to keep the architecture honest until physical metrics are decomposed. The energy family must eventually be expressed in black-start megawatts, firm energy, fault current, ride-through and protected connections. Water must be expressed in feed envelope, safe flow, storage, residual custody and assay. Thermal must include useful cooling, pumping and final heat rejection. Distribution must include actual route length, voltage, flow, building interfaces and protection. Civil control must include offline command, laboratory throughput, medical and access functions, communications, robotics and repair.

The families are not five boxes placed beside one another. The innovation burden lies in giving each tile a primary function while also supplying limited cross-support. An energy tile may contain protected conversion and black start while contributing thermal support. A water tile may own treatment and residuals while providing fire-water or thermal fluid. A thermal tile may support medical temperature control and water processing. A distribution tile may carry robotic corridor equipment and bypass hardware. A civil-control tile may host assay, communications, field repair and access systems.

This multifunctionality cannot become an excuse for universal common mode. Every tile needs contained failure boundaries, protected interfaces, replaceability and a declared primary coefficient. No signature may substitute for another. A control display saying “water available” cannot replace a passed water assay. Spare electrical capacity cannot compensate for absent distribution. General cargo mass cannot compensate for a missing final heat sink.

Wet integration is especially important. Water, fuel, reagents, lubricants and process liquids cannot sit in a separate formation-wide pack whose loss defeats every otherwise redundant tile. Each family must own and meter its custody burden, or several protected stores must be independently routable to every surviving quorum. The same rule applies to software, assay instruments, connector tooling and calibration authority.

## 5. Carrier quorums and the held reserve

Every air carrier carries four tiles from each family: twenty tiles and 317.5 tonnes. The possible surviving pairs are `A1+A2`, `A1+A3` and `A2+A3`. Each pair retains eight tiles per family, forty total tiles and 635 tonnes. After a further tile rejection, the affected family retains seven contributors and the provisional 100-unit floor.

Every terrain carrier carries two tiles from each family: ten tiles and 158.75 tonnes. Each of the five possible four-carrier subsets retains eight tiles per family and the same 635-tonne kernel. The formation does not depend on choosing a particular sacrificial vehicle.

At the receiver, the non-selected carrier is a **controlled reserve**. It remains loaded, isolated and under technical custody. It is not counted as delivered service. Its crew, fluids, tiles and parts cannot be cannibalized casually. If one of the nominal survivors fails admission, the receiver may formally recompile the quorum and substitute the held carrier. Until then, the reserve cannot share a pre-release utility spine that would turn isolation into fiction.

The quorum compiler is therefore partly computational and partly constitutional. It consumes the signed measured state of carriers, tiles, connectors, working fluids, crews and receiver zones. It enumerates valid subsets under an offline rule set. An independent checker reproduces the selection. Mode-specific configuration authorities admit the vehicles; family authorities admit the service functions; the civil authority alone authorizes public reliance.

Automation is useful because the configuration space is too consequential for improvised human arithmetic under stress. But the compiler cannot manufacture evidence or assume authority. Its two implementations must be independently developed for air and terrain. Its outputs are recommendations and signed state records, not self-executing permission to connect a population to an unassayed system.

## 6. One mission grammar, different physics

Both modes now follow a common mission state machine:

1. technical and configuration release at origin;
2. mode-specific movement;
3. receiver admission and survivor-state measurement;
4. quorum selection and controlled unload;
5. service-family assembly and assay;
6. independent civil release; and
7. post-release federation only after both effects are safe.

The atmospheric reference spends 16 hours in origin release and parallel load, 16.667 hours on the 4,000-kilometre route, 1.25 hours in arrest and quorum transfer, and 8 hours in service assembly and civil release. Relative service is 41.917 hours; the six-hour regional activation offset produces absolute hour 47.917.

The terrain reference spends 8.75 hours in measured configuration release, 10 hours on 500 kilometres of degraded hard route, 6.875 hours on 220 kilometres of broken or saturated route, 4.444 hours on 80 kilometres off road, 4.75 hours in contact, survey, bridge and route work, and 8.75 hours in unload, assay and civil release. Relative service is 43.569 hours and absolute service hour 49.569.

The model assigns deterministic stress allowances of 4.5 hours to air and 3.5 hours to terrain. These are design budgets, not measured percentiles, probabilities or confidence claims. With both delays imposed, the first service appears by hour 52.417. With the air mode removed, the terrain path including its full allowance releases by hour 53.069. With the terrain mode removed, the stressed air path releases by hour 52.417. The residual margins are small enough to make queues, weather tails, assay throughput and receiver operations decisive evidence questions.

The 28-world lattice tests nominal operation; each mode cut; one carrier loss in either or both modes; tile losses; carrier-plus-tile losses; mode-plus-surviving-carrier-plus-tile casualties; origin and receiver cuts; network and GNSS denial; energy-lineage cuts; and the declared delay budgets. Every inside world passes under the assumptions. Four harder cases are explicitly outside: air lost plus two terrain vehicles, terrain lost plus two air vehicles, both modes lost, and one vehicle in each mode plus two family-tile losses.

No frequency is assigned. Probability requires observed failure processes, correlation, route and weather distributions, maintenance state, crew performance, and receiver queues. Those belong in later empirical campaigns. The present lattice determines what must be physically true whenever an admitted world occurs.

## 7. Receiver geometry is part of the weapon system equivalent

A projected civil force fails if its carrier can arrive but the receiver cannot safely accept, isolate, unload, connect and release it. `DCP-2R` increases receiver burden because it brings larger quorums and controlled reserves.

The atmospheric boundary is a 520-by-460-metre, 239,200-square-metre controlled complex with three parallel zones. Each zone must support arrest, ground reaction, exclusion, lift-gas and water custody, payload transfer, emergency egress and fire protection. The terrain boundary remains 220 by 140 metres, or 30,800 square metres, with five vehicle positions arranged within a notional three-by-two grid. The unused grid cell is not empty convenience; it provides space for survey, crane work, casualty bypass, quarantine or a rejected vehicle.

The air and terrain complexes retain five kilometres of pre-release separation. They use independent ingress, utilities and technical authorities. Only after each has created an independently assayed public effect may the joint receiver command open a cross-tie. This prevents a common loader, power plant, assay chain or control network from silently defeating the two-mode claim.

These dimensions are planning envelopes, not solved sites. Plume, heat, rotor or propulsor effects, soil bearing, drainage, contamination, crowd protection, noise, medical access and public distribution may enlarge them. Nor does geometric room prove parallel throughput. Loader counts, labor paths, inspection stations, laboratories, cranes, hose and cable corridors, and reset bays need queue evidence.

## 8. The industrial ancestry firewall

Mode diversity is useful only if the causes that disable one path do not disable the other. The model therefore creates a twelve-domain ancestry firewall covering primary energy; power conversion; electrical protection; water membranes and chemistry; thermal machines; final heat rejection; distribution hardware; control kernels; communications bearers; navigation; structural connectors; and assay instruments.

Air and terrain may share four things: the definition of the service state, the units in which it is measured, the semantic intent of an interface, and the record used for civil handoff. They may not receive independence credit merely because two products have different names or come from different prime contractors.

True independence must be traced through sub-tier suppliers, fabrication processes, firmware libraries, model-training dependencies, calibration laboratories, feedstocks, test authorities and configuration tools. Two nominal suppliers using the same power module, membrane chemistry, satellite service or safety compiler may still create one decisive cause. No program office should certify both implementations of the same family. An Independent Ancestry Authority should own bills of material, causal maps, destructive common-cause trials and change surveillance.

This rule deliberately sacrifices some economies of commonality. The Resilience Force should standardize the civil language and connection contract while maintaining rival physical lineages beneath it. That resembles a public utility constitution more than a commercial platform family: interoperability at the released boundary, diversity before it.

## 9. Workforce and authority

The selected boundary grows the `DCP-2` workforce from 758 deployed, 1,699 affiliated and 244 minimum watch to 906 deployed, 2,031 affiliated and 284 watch. The increments are:

| Element | Deployed | Affiliated | Watch |
| --- | ---: | ---: | ---: |
| Air reinforcement | 44 | 96 | 14 |
| Terrain reinforcement | 32 | 72 | 8 |
| `ESK` and assurance | 48 | 110 | 12 |
| Receiver expansion | 24 | 54 | 6 |
| **Total increment** | **148** | **332** | **40** |

These figures are staffing hypotheses. Their purpose is to expose professions that an equipment-only account would omit: configuration custody, quorum compilation, independent checking, ancestry surveillance, water and residual assay, energy release, thermal safety, distribution protection, receiver exclusion, civil release, controlled reserve, reset and technical schools.

Carrier commanders may release a vehicle to move. They may not release water, electricity, occupied cooling or medical service to the public. Each decisive technical role needs a named casualty substitute who does not violate the independence rule. Limited dual qualification is appropriate for liaison and other non-decisive work, but it cannot collapse two certifying lineages into the same exhausted individual.

The affiliated count includes relief pools, depots, laboratories, instructors, independent authorities and configuration staffs. It excludes the broader contractor industrial workforce. Later trials must measure task durations, handoffs, fatigue, school throughput and simultaneous-duty peaks. Until then, automation may reduce enumeration and documentation time but should not be credited with reducing accountable release positions.

## 10. Reset, fleet and production

Forty-three ready formations drive the fleet boundary. The selected air fleet rises from 86 operational vehicles to 129—three per formation—with 26 reserve and 14 development articles, for 169 total. The selected terrain fleet rises from 172 operational to 215—five per formation—with 43 reserve and 12 development articles, for 270 total. Together `DCP-2R` contains 439 carrier articles, 102 more than the present 337-article baseline.

The full-duplication control would require 221 air and 425 terrain articles, or 646 total. The selected architecture therefore avoids 207 articles relative to that control. The result is economically meaningful but not dispositive: one failed payload premise can erase it.

Reset remains governed by the slowest certified path. The air reference is 162 hours and the terrain reference 166 hours against a 168-hour ceiling. Vehicle inspection, tile replenishment, working-fluid custody, receiver restoration, crew recovery, evidence review and reconfiguration are separate queues. The formation is not ready because the carrier returned to base. It is ready when a complete, independently certified load and crew can repeat the mission.

Development articles stay outside operational and reserve counts because destructive proof is a continuous function, not a one-time preproduction event. The force needs permanent rival pilot lines, instrumented receiver ranges, casualty insertion, environmental chambers, route and soil ranges, offline control laboratories, and whole-mission reset exercises.

## 11. Fiscal boundary and technology portfolio

The selected 25-year `DCP-2R` program begins with the Pass 87 `DCP-2` boundary of $3.7773011 trillion and adds:

| Increment | 25-year boundary |
| --- | ---: |
| Atmospheric reinforcement | $551.14745B |
| Terrain reinforcement | $292.34864B |
| Receiver expansion | $80.00000B |
| `ESK` and independence | $240.00000B |
| **Selected `DCP-2R`** | **$4.94079719T** |

Adding the $7.38314155 trillion national base outside `DCP-2` produces a $12.32393874 trillion national boundary. Full exact-cell duplication produces $6.00387624 trillion for the two-mode program and $13.38701779 trillion nationally.

These are acquisition envelopes, not appropriations forecasts, vendor estimates or discounted cash flows. They receive no learning-curve, export, avoided-loss or economic-multiplier credit. The comparison is useful because it reveals the scale of the assurance choice, not because the last digits are predictive.

A $775 billion technology and proving portfolio is nested within the selected program rather than added to it. Twenty campaigns cover the five tile families; air and terrain reinforcement; offline quorum compilation; semantic connectors; independent energy and process lineages; both receivers; cross-mode civil release; network and navigation denial; destructive compound trials; reset; workforce schools; industrial pilot lines; and an evidence commons with independent red teams.

The portfolio should be managed as competing capability campaigns rather than a linear development plan. Each campaign has a failure allocation. If the energy tile misses its coefficient, the force adds tiles, carriers or a different energy architecture. If receiver heat rejection fails, the site grows or the service output falls. If ancestry analysis finds a shared decisive supplier, compound credit is withdrawn. If reset exceeds the ceiling, fleet and industrial capacity grow. Failure changes the design; it does not disappear inside contingency.

## 12. Evidence constitution and falsification

The workbook registers 160 evidence gates: eight gates for each of twenty campaigns. The common gate classes are coefficient; mass and custody; interface; contained failure; independence; mission clock; reset; and authority. Every gate begins `OPEN` and receives zero maturity credit.

An accepted gate needs a representative article, raw records, a preregistered threshold, an accountable independent owner and an explicit failure allocation. A green spreadsheet reconciliation means only that the declared model is internally consistent. It does not turn a normalized service unit into measured megawatts or safe water.

The proving sequence should proceed from the smallest objects with the greatest architectural leverage:

1. build one representative tile from each family in separate air and terrain lineages;
2. close dry mass, wet mass, fluid custody, power, heat, connectors, contained failure, field replacement and assay;
3. assemble one ten-tile terrain load and one twenty-tile air load;
4. demonstrate carrier-level configuration measurement and independent compiler agreement;
5. assemble full three-air and five-terrain formations at separate receivers;
6. quarantine one carrier, reject one further tile and reconstruct the service vector;
7. run the absolute mission and 168-hour reset clocks under network and GNSS denial; and
8. repeat with independent red teams changing casualty timing and sub-tier causes.

The strongest early falsification is the tile coefficient. If one 15.875-tonne module cannot carry its assigned primary function, cross-support, containment, connectors and custody burden, `ESK-40` loses authority. The correct response would be to reopen tile mass, family count, carrier number and the full-duplication control—not to preserve the label by redefining “service unit.”

## 13. Institutional and economic meaning

`DCP-2R` illustrates why a Department of Resilience cannot be a grant office surrounding a fleet. It requires institutions capable of writing public-service guarantees, sustaining rival technical lineages, owning receivers, certifying professions, maintaining deep fleets, operating permanent proving grounds and withdrawing assurance credit when causal independence disappears.

The industrial system would resemble a civil counterpart to the defense base without copying its purpose. Prime integrators would compete complete service architectures. Specialist firms would produce power conversion, membranes, thermal machines, deployable distribution, robotics, laboratories, connectors and offline controls. Public arsenals and private yards would preserve surge and repair. Technical colleges and academies would train configuration, assay, receiver and release professions. Government would maintain test articles and evidence infrastructure even when no disaster is active.

Export opportunity would follow from verified service effects. Allies and partner cities could acquire compatible receivers, tile families, control semantics, training and industrial licenses without purchasing the entire United States formation. But exportability should not drive premature commonality. The most valuable standard is the civil service and interface contract. Partner nations should be able to implement independent physical lineages underneath it.

Strategically, the force changes what American power can promise. It can arrive with power, water, cooling, communications, medical continuity and access that do not depend on the damaged society donating its last working port, grid, road or technical staff. It can demonstrate competence without coercion and stabilize partners by invitation. The same industrial system strengthens domestic continuity because its assets, schools, receivers and suppliers exist before catastrophe.

## 14. Stocktake and next decision

This pass does not supersede `DCP-2` by declaring it wrong. It clarifies its assurance class. The two-air/four-terrain exact-block formation remains the current single-mode-cut lower bound. It is smaller and may be appropriate where the public guarantee does not include a second casualty within the surviving mode.

`DCP-2R` is a higher compound-assurance behavior reference. It adds one concurrent spare carrier per formation in each mode and changes the payload grammar so surviving mass retains every function. Full exact-cell duplication is the conservative control. The current preference for `DCP-2R` is provisional and conditional on proving physical multifunctionality and independence.

The burden has moved decisively into the payload. Carrier exteriors are no longer the next unknown with the greatest power to change the force. The priority object is a complete representative five-family tile set and its receiver connectors. The next research pass should decompose each normalized family coefficient into physical performance, mass, energy, heat, fluid, containment, crew and assay requirements; compete tile architectures within both lineages; and determine whether the 15.875-tonne boundary survives.

Only after a representative tile grammar, carrier load and destructive receiver mission stabilize should rendering begin. At that point imagery can communicate an evidence-led architecture: access panels, fluid segregation, protection distances, lifting and handling points, connector fields, maintenance envelopes, crew paths, quarantine markings and receiver choreography. Until then, exterior art would create confidence in a shape whose most decisive internal object has not yet been designed.

## Model companion

The companion workbook, [`dcp2r-common-carrier-and-mission-compiler.xlsx`](../../../models/force/projection/dcp2r-common-carrier-and-mission-compiler.xlsx), contains the service constitution, tile grammar, complete air and terrain quorum enumeration, six-way architecture competition, common state machine, delay budgets, 28-world challenge lattice, receiver geometry, ancestry firewall, crew and authority map, fleet and workforce boundary, program costs, twenty technology campaigns, 160 evidence gates and 230 terminal audit controls.

