# F36 `CISA-40` `SA6` internal cell and source-boundary design constitution

## Executive judgment

The previous pass established a provisional two-tonne maximum credible release (`MCR`) for one `SA6` source compartment, but only after twenty-four propagation-denial claims were accepted. It also proposed one liquid sump, one pressure receiver and one gas holder for each operational lane. That arrangement could retain a one-compartment event. It could not prove that one compartment remained independent of its neighbors, because the receiving systems themselves were common paths.

This pass creates `SBD-1`, the internal cell and source-boundary design constitution. Its governing correction is:

> A source is not independent when its emergency destination is shared. Every admitted compartment must retain its own isolation, relief, drainage, receiving, disposition, safety-energy and evidence path through terminal source condition.

`SBD-1` therefore replaces the shared lane-level emergency systems with four complete source trains per operational lane. Each train begins at one source pod and ends in an independently identified terminal destination. Root A receives a dedicated 150 mm liquid route, 15 m³ source sump, 40 m³ firewater vault and recovery handoff for every pod. Root B receives a dedicated 500 mm reference-gas route, 5,344 kg pressure receiver, 2,000 m³ gas-holder chamber and last-resort disposition path for every pod. No pressurized manifold, drain, safety-power bus, final isolation element or native recorder may cross-connect the four trains.

That correction changes the planning capacity materially. Each lane now has 60 m³ of source-liquid retention against a 50 m³ full-rack requirement, 160 m³ of firewater retention against a 120 m³ requirement, 8,000 m³ of gas-holder volume against a 6,360 m³ thermally allowed reference-gas quantity and 21,376 kg of receiver capacity against 8,000 kg of installed source. The capacity arithmetic for the four-compartment `C2` state now closes. The authority does not. `C2` remains blocked until the physical propagation evidence, safe-state performance, source reconciliation and independent decision all close.

The two operational cells remain `MC-B1` at `PTC-B` and `MC-C1` at `PTC-C`. The destructive consequence cell remains `MC-A1` at `PTC-A`. Each operational lane receives four staggered source pods at longitudinal stations 2.5, 4.8, 7.2 and 9.5 m, alternating laterally at ±0.8 m. A 2.1 × 1.7 × 3.2 m planning bay envelope gives each pod its own boundary, support, route departure and sensor field while preserving the inherited 12.0 × 3.6 × 3.8 m article envelope. The geometry is an internal test configuration, not exterior form.

The design is governed by sixteen measurement planes, from the source interior (`P00`) to the evidence boundary (`P15`). Sixteen root–site–pod routes are each checked across eleven no-common-path domains, producing 176 path records. Thirty-two interface records preserve both root-native ancestry and public-test handoff. Sixty-four controlled drawing sheets divide the design into general arrangement, civil containment, source quartet, root-specific process, safety power and control, instrumentation, and rescue/robotics packages. None establishes exterior appearance.

The evidence design is similarly explicit. Eighteen measurement functions create 354 channels per operational lane and an uncompressed aggregate rate of about 50.808 MB/s. A ten-minute full-rate window, six-hour five-percent tail, two independent originals and 1.35 protocol overhead produce approximately 230.461 GB per event. The eighty inherited safety events plus forty-eight new paired propagation exposures create 128 registered events and about 38.349 TB including a thirty-percent reserve. The inherited 576 TB public vault remains ample. Capacity is not evidence integrity, so time, calibration, packet identity, local retention and two physically separate originals remain independently governed.

The paired propagation campaign contains twenty-four protocols: six functions, two roots and two sites. Each protocol has one challenged event and one clean control, giving forty-eight exposures. Four transfer functions use a provisional 0.5 kg protected-side upper bound. Thermal and fragment functions use a provisional 0.8 normalized protected-side utilization bound. These are declared falsifiable hypotheses, not accepted limits. Every exposure remains unexecuted.

The corrected architecture requires USD 420M of capital and USD 42M/year of annual support. Thirty-four months of support creates a USD 539M program exposure. Replacing the previous `MCR-1` allocation raises the reconciled `BRD-4R` boundary to USD 940M capital and USD 174M/year. That remains inside the USD 960M/260M annual `CISA-1` parent boundary, leaving USD 20M capital and USD 86M/year. The no-credit physical-use view is USD 1.068B capital and USD 215M/year. It exceeds the parent capital boundary by USD 108M. The two views answer different questions and remain visible: funding ownership reconciles; gross physical use does not.

The pass closes 158 planning gates. It leaves 188 physical gates open and seven downstream gates blocked. The planning model contains twenty-seven sheets, 781 terminal audits and thirty-nine sensitivity tests, all passing with no formula error. Accepted physical sources remain zero.

The decisive learning is institutional as much as technical. A national resilience force cannot inherit the defense-industrial habit of calling a shared emergency utility “redundant” because it has multiple valves. It needs a source-boundary discipline that follows mass, energy, command and evidence to their independent terminal states. That discipline will be essential for larger future systems: mobile reactors, high-rate desalination, ammonia or hydrogen logistics, wildfire energy stores, autonomous earthmoving fleets and rapidly deployed power systems all create source hazards whose safe destinations are part of the vehicle or formation design.

Exterior rendering remains blocked. The next decisive pass should resolve Root B two-phase relief and retention physics through a technology competition among direct low-pressure capture, staged pressure recovery and a hybrid measured-destruction architecture. The 500 mm route in this pass is a transparent reference-state screen, not a flashing-flow design.

## 1. Decision and inherited boundary

### 1.1 Decision

`SBD-1` answers:

> What internal source geometry, independent process topology, measurement system, safety logic, recovery chain, drawing package, physical campaign and fiscal boundary are required to test whether one two-tonne `SA6` source can remain independent of three neighbors?

The answer is not a larger test chamber. It is a cell composed around sixteen independent source routes: two roots, two sibling operational sites and four source pods. The route is the irreducible safety object. A lane, vessel, valve, sump or gas holder is useful only insofar as it preserves the route's independence.

This pass preserves the governing hierarchy from [`MCR-1`](f36-cisa40-sa6-maximum-credible-release-and-source-preserving-containment-constitution.md):

1. protect human life;
2. prevent recruitment of another source;
3. preserve direct evidence;
4. recover the source when safe;
5. protect public infrastructure; and
6. preserve schedule.

No evidence requirement delays a life-protecting action. No recovery objective justifies a common path. No schedule claim converts an open physical question into a planning pass.

### 1.2 Inherited objects

`SBD-1` inherits rather than reopens:

- the `CISA-40` 12.0 × 3.6 × 3.8 m common envelope, 32-tonne dry state and 40-tonne operating state;
- the four-compartment `SA6` source arrangement and two-tonne source mass per compartment;
- Root A liquid-fuel and Root B DME planning media;
- `C0`, `C1` and `C2` source states;
- `PTC-B/LN-11` and `PTC-C/LN-12` as sibling operational lanes;
- `PTC-A` as the destructive consequence location;
- the requirement for two locally complete native evidence originals;
- the USD 960M capital and USD 260M/year `CISA-1` parent boundary; and
- the prohibition on exterior rendering.

The immediate lineage includes the [coupled module specification](f36-coupled-utility-module-and-receiver-spine-physical-specification.md), [internal build-release constitution](f36-cisa40-internal-build-release-and-measurement-drawing-constitution.md), [root build package](f36-cisa40-root-build-package-and-tolerance-stack-constitution.md), [construction traveler](f36-cisa40-construction-release-and-evidence-traveler-constitution.md), [controlled-defect campaign](f36-cisa40-full-scale-subarticle-and-controlled-defect-execution-campaign.md), [public test complex](f36-cisa40-public-test-complex-and-phase-zero-commissioning-constitution.md), [reference-article package](f36-cisa40-reference-article-and-phase-zero-source-package-constitution.md) and `MCR-1` above.

### 1.3 Evidence classes

| Class | Meaning | Authority in this pass |
| --- | --- | --- |
| inherited requirement | controlled value or object from an accepted predecessor | retained unless explicitly corrected |
| declared hypothesis | geometry, time, flow, threshold, staffing or cost proposed for design | planning only |
| calculated screen | arithmetic result derived from inherited values and hypotheses | sizes the program; does not qualify physics |
| physical observation | measured result from a valid native event packet | zero |
| accepted physical source | observation admitted by the independent physical authority | zero |

The distinction prevents a common failure in ambitious technology programs: detailed arithmetic can create the appearance of maturity before the causal system exists. `SBD-1` is detailed because the eventual experiment must be reproducible, not because detail creates authority.

## 2. The common-path correction

### 2.1 Why the previous arrangement fails its own rule

`MCR-1` denied six propagation functions: source-boundary failure, a common fuel path, relief backflow, shared drainage, thermal escalation and fragment/support recruitment. It then gave each lane one 12.5 m³ sump, one 5,344 kg receiver and one 2,000 m³ gas holder. Those receiving systems created three additional ways for source compartments to interact.

A shared sump can collect liquid from several compartments, transmit fire or vapor into another bay, and erase the ancestry of recovered material. A shared pressure receiver can create return pressure, compete for volume or force two relief routes into one header. A shared gas holder can transmit pressure, flame or incompatible products across what had been separate source boundaries. Adding check valves reduces some normal-flow interactions but does not prove independence under heat, deformation, debris, partial blockage or loss of actuation.

The correct question is therefore not whether the installed emergency capacity exceeds the source quantity. It is whether any event in one train can change the safe state of another train through a common object.

### 2.2 Source train as the unit of independence

Each source pod receives a complete train:

```text
SOURCE POD
   │
   ├── primary vessel boundary
   ├── independent isolation
   ├── dedicated relief or liquid-transfer route
   ├── dedicated drain or knockout
   ├── dedicated receiver or sump
   ├── dedicated holder or recovery destination
   ├── dedicated last-resort disposition
   ├── independent thermal and fragment barrier
   ├── independent structural support
   ├── independent safety energy and final element
   └── locally retained native evidence
```

The train may exchange non-safety status data across the public evidence network after local capture. It may not depend on that network to isolate, route, retain or record the event. A maintenance connection can exist only if it is physically absent, blanked and independently observed during source admission. Administrative prohibition is not equivalent to physical separation.

### 2.3 The eleven-domain test

Every one of the sixteen root–site–pod routes is registered against eleven domains:

| Domain | No-common-path question |
| --- | --- |
| source boundary | can an initiating breach directly open or load a neighbor? |
| primary isolation | does another train share the actuator, stored energy or final element? |
| relief or transfer route | can backpressure, blockage or flame traverse a common header? |
| drain or knockout | can liquid, vapor or suppression water cross between bays? |
| receiver or sump | can capacity competition or inventory mixing recruit a neighbor? |
| gas holder or recovery | can pressure or composition propagate through the terminal destination? |
| last-resort disposition | does one train's protective action deprive or threaten another? |
| thermal and fragment barrier | does the barrier remain functional under the registered stimulus? |
| structural support | can one pod's deformation or release remove another's support? |
| safety energy and logic | can one fault disable multiple isolation paths? |
| native evidence | can one failure erase both the event and its neighbor reference? |

Sixteen routes multiplied by eleven domains create 176 records. A planning record passes when its object, drawing and protocol are assigned. Physical proof remains open until the relevant challenge event, control and disposition are accepted.

## 3. Source quartet and operational-cell geometry

### 3.1 Staggered quartet

The four source pods preserve the inherited longitudinal arrangement while alternating laterally:

| Pod | longitudinal station | lateral station | planning bay envelope | next clear gap |
| --- | ---: | ---: | --- | ---: |
| `SP-1` | 2.5 m | −0.8 m | 2.1 × 1.7 × 3.2 m | 0.20 m |
| `SP-2` | 4.8 m | +0.8 m | 2.1 × 1.7 × 3.2 m | 0.30 m |
| `SP-3` | 7.2 m | −0.8 m | 2.1 × 1.7 × 3.2 m | 0.20 m |
| `SP-4` | 9.5 m | +0.8 m | 2.1 × 1.7 × 3.2 m | 1.45 m to the envelope end |

The lateral staggering does three things. It prevents a straight line of sight among all four source centers. It gives alternate sides for route departure. It allows barriers and sensors to observe one pod without requiring a shared central chase. It does not by itself prove fragment or thermal separation; those remain physical questions.

The inherited source quantities are 2.500 m³ for Root A and 2.994 m³ of liquid for Root B per pod. Root B's planning vessel gross volume is 3.743 m³ at an eighty-percent liquid fill. Vessel geometry, head form, nozzle reinforcement, supports and thermal protection remain root-specific drawing objects.

### 3.2 Cell allocation

| Cell | Site | Role | provisional exclusion radius | remote-control distance |
| --- | --- | --- | ---: | ---: |
| `MC-B1` | `PTC-B` | source-preserving operational lane | 200 m | 250 m |
| `MC-C1` | `PTC-C` | source-preserving operational lane | 200 m | 250 m |
| `MC-A1` | `PTC-A` | destructive consequence cell | 250 m | 300 m |

Two operational cells preserve site diversity. Each must be capable of executing all Root A and Root B operational protocols without using its sibling's utilities, evidence vault or response force. The consequence cell accepts representative ignition, blast, fragment, roof-fire and support-collapse conditions that would be inappropriate for a source-preserving lane.

The three non-overlapping exclusion circles require approximately 44.768 hectares of controlled land. That figure excludes access corridors, terrain effects, security setbacks, ecological buffers and external infrastructure. It is a geometric lower-bound screen, not a siting decision.

### 3.3 Functional zoning

An operational cell contains six zones:

1. **source court** — four individually bounded pod bays and their near-field sensors;
2. **route gallery** — separated liquid or pressure corridors with no cross-train header;
3. **retention court** — four sumps and firewater vaults or four receiver/holder sets;
4. **safe-state field** — passive dispositions, isolation energy and terminal-source sensing;
5. **remote operating refuge** — protected command, event clock and independent evidence original; and
6. **recovery and rescue perimeter** — robotics, decontamination, casualty transfer and controlled re-entry.

The route gallery and retention court are not ordinary utilities. They are extensions of the source boundary. Their location, supports, drainage, thermal exposure and evidence channels belong on the source drawing.

## 4. Root A liquid train

### 4.1 Per-train flow screen

A two-tonne Root A source released over 120 seconds produces a planning mass flow of 16.667 kg/s. At 800 kg/m³, the volumetric flow is 0.020833 m³/s. A 150 mm internal diameter gives approximately 1.179 m/s, below the declared 2.0 m/s velocity ceiling. A 12 m route has a nominal transit time of 10.179 seconds.

This calculation establishes only that a 150 mm route is not obviously undersized on bulk velocity. It does not establish valve coefficient, head loss, gravity behavior, vapor formation, blockage tolerance, water interaction, fire resistance or source-vessel emptying. Those become controlled physical quantities.

### 4.2 Independent retention

Each Root A train receives:

- one 15 m³ source-liquid sump;
- one 40 m³ firewater vault;
- gas break between source and drainage systems;
- independent level and mass observation;
- no cross-train drain;
- a named recovery vessel; and
- a discrepancy ledger with a provisional 5 kg closure threshold.

Four sumps provide 60 m³ per lane. The full-rack source-liquid requirement under the inherited five-times-volume rule is 50 m³, leaving 10 m³ of margin and a 1.20 capacity ratio. Four firewater vaults provide 160 m³ against the 120 m³ lane requirement, leaving 40 m³ and a 1.333 ratio.

The 15 m³ sump is deliberately larger than the prior 12.5 m³ one-compartment capture volume. That margin absorbs instrument dead zones, foam, debris and recovery heel without treating the full-rack requirement as a shared pool. The firewater vault remains separate because water volume cannot also be claimed as recovered source volume.

### 4.3 Root A flow path

```text
P00 source interior
  → P01 vessel wall
  → P02 interstitial boundary
  → P03 source nozzle
  → P04 primary isolation
  → P06 dedicated liquid drain/transfer
  → P09 dedicated 15 m³ sump
  → named recovery vessel and custody ledger

P07 dedicated firewater drain
  → dedicated 40 m³ firewater vault
```

The two drainage paths remain separately measurable even when they terminate in the same recovery operation. A remotely operated pump may remove material only after terminal source condition, composition sampling and custody transfer. Pumping during the event would introduce a new energy source and a new failure path unless specifically qualified.

### 4.4 Technology agenda for liquid containment

The design should drive new capabilities rather than freeze current practice. Candidate programs include:

- fast passive diverters that direct a gross vessel release without external power;
- high-temperature transparent mass-balance sections using strain, pressure and distributed thermal sensing;
- self-sealing drain liners that preserve flow after fragment penetration;
- robotic skimming and phase separation that keeps humans outside the hot zone;
- chemically specific optical tomography of pool thickness and spread; and
- recoverable fire barriers whose thermal history is itself a native evidence object.

The force should buy these as families of interoperable safety articles, not one-off facility equipment. The same technologies would support mobile fuel farms, wildfire aviation bases, rapidly deployed generators and post-disaster hazardous-material recovery.

## 5. Root B pressure and gas train

### 5.1 Reference-state sizing

The Root B source is a two-tonne DME planning case. Releasing it over 120 seconds gives 16.667 kg/s. Using the declared reference-gas factor of 0.530 m³/kg gives 8.833 m³/s. A 500 mm internal diameter gives 44.988 m/s, below the declared 60 m/s velocity screen. An 80 m route has a nominal reference transit time of 1.778 seconds.

That arithmetic is not a pressure-relief design. A real DME event may involve flashing liquid, choked flow, aerosol carryover, refrigeration, ice formation, heat input, vessel depressurization, line inventory, pressure-wave interaction and receiver backpressure. The reference-state route is useful because it makes the architectural scale visible. It must not be used to select wall thickness, valve capacity or physical operating limits.

### 5.2 Independent retention array

Each Root B train receives:

- a dedicated relief route;
- a 5,344 kg pressure receiver;
- a 2,000 m³ gas-holder chamber;
- a measured last-resort disposition path;
- independent pressure, temperature, flow, gas and oxygen observation;
- no common pressurized or return header; and
- a local evidence original.

Four holders provide 8,000 m³ per lane. Against the 6,360 m³ thermally allowed `C2` reference quantity, the margin is 1,640 m³ and the ratio is 1.258. Four receivers provide 21,376 kg of nominal capacity against 8,000 kg of installed source, a ratio of 2.672. This does not imply that the receivers can accept the transient. It means that static nominal capacity no longer forces one source to compete with another.

### 5.3 Three candidate terminal architectures

The next technology competition should carry three genuinely different architectures rather than small variations of one header.

**Architecture B1 — direct segmented low-pressure capture.** Each source flashes through a short, protected route into a dedicated low-pressure expansion chamber and then a segmented membrane holder. Its virtues are passive capacity, visible source ancestry and low terminal pressure. Its risks are enormous deployed volume, cold embrittlement, membrane compatibility, wind loading, vapor stratification and difficulty controlling two-phase inlet momentum.

**Architecture B2 — staged pressure recovery and condensation.** Each route enters a high-rate knockdown receiver followed by staged accumulators and active or stored-cold condensation. Its virtues are smaller final volume, potentially higher source recovery and easier transport of retained product. Its risks are complex transient control, heat rejection, refrigeration dependence, receiver backpressure and the possibility that active equipment becomes necessary for safe state.

**Architecture B3 — hybrid recovery with measured last-resort destruction.** The first stage captures liquid-rich flow and recoverable vapor; overflow enters a dedicated outdoor holder; a final isolated oxidizer destroys only the fraction that cannot be safely retained. Its virtues are tolerance of uncertain phase behavior and a clear life-safety escape. Its risks are ignition control, combustion stability, emissions measurement, public acceptability and the temptation to call destruction “recovery.”

The competition should be settled by mass and energy closure, not narrative preference. Each architecture must survive representative source temperature, heat input, obstruction, wrong-side pressure, sensor loss, power loss, partial receiver fill and site-network denial. A hybrid may win, but common equipment cannot be credited as independent merely because each train has a separate inlet.

### 5.4 Root B flow path

```text
P00 source interior
  → P01 vessel wall
  → P02 interstitial boundary
  → P03 source nozzle
  → P04 primary isolation
  → P08 dedicated two-phase relief route
  → P09 dedicated pressure receiver
  → P10 dedicated holder inlet
  → P11 dedicated holder volume
  → P12 dedicated last-resort disposition
```

No stage may rely on the public network for safe actuation or native recording. If the source reaches the last-resort route, the packet must still conserve initial mass, captured liquid, retained vapor, estimated unretained inventory and measured destruction products within declared uncertainty.

## 6. Safety energy, control and terminal source condition

### 6.1 Three unlike paths

Each root–site case receives three independent safety paths:

| Path | Energy | Hold-up | Detection | Controller | final action |
| --- | --- | ---: | --- | --- | --- |
| analog hardwire | dedicated 125 VDC battery A | 4 h | pressure and flow | relay logic | spring isolation |
| diverse digital | dedicated 48 VDC battery B | 8 h | unlike gas and thermal sensors | isolated safety controller | accumulator isolation |
| passive | stored mechanical energy | not time-dependent | thermal or pressure element | none | rupture route or passive diversion |

There are twelve registered paths: three for each root at each sibling site. They may share an observed event clock only after locally complete recording. They do not share a final element, safety bus, controller or actuator reservoir.

The passive path matters because batteries, wires and logic can all become correlated under heat, water or fragment exposure. The analog path matters because a diverse digital system can still fail by common environmental cause. The digital path matters because it can fuse unlike sensors and create a more discriminating response. Diversity is not ornamental; it is a hypothesis that must be challenged under common-cause conditions.

### 6.2 Safe-state clocks

Command, observation and terminal source condition remain separate times:

- trip command: 0.100 s planning target;
- decisive vote: 0.250 s;
- primary isolation: 2.000 s for Root A and 5.000 s for Root B;
- passive route opening: 10.000 s;
- Root A route transit: 10.179 s reference;
- Root B route transit: 1.778 s reference;
- terminal source condition: 30 s for Root A and 120 s for Root B;
- native evidence seal: 30 s after the defined evidence window; and
- minimum human entry: 1,800 s for Root A and 3,600 s for Root B.

The clock does not stop when software reports “closed.” Root A terminal state requires measured cessation or bounded recovery flow, stable sump and firewater inventory, no growing pool and no neighbor recruitment. Root B requires measured isolation, bounded receiver and holder state, no growth of an unretained cloud and a closed mass ledger within uncertainty.

### 6.3 Automatic stop conditions

The cell returns to `C0`, invalidates the event for physical credit and holds the affected route when any of the following occurs:

- a cross-train pressure, liquid, gas, heat or evidence path is observed;
- both active safety paths lose credible energy or timing;
- the passive route fails to reach its registered state;
- native time uncertainty prevents causal ordering;
- source mass discrepancy exceeds the registered limit without disposition;
- a protected-side metric exceeds its declared bound;
- one evidence original is not locally complete;
- a sensor used for admission is out of calibration or saturated without an unlike reference;
- human entry occurs before the registered authority and atmospheric conditions permit it; or
- any emergency action uses an unregistered route.

An event stopped for safety can still be scientifically valuable. It cannot be silently recoded as a successful qualification.

## 7. Measurement constitution

### 7.1 Sixteen planes

The measurement system follows the source rather than the facility organization:

| Plane | Location | Governing quantities |
| --- | --- | --- |
| `P00` | source interior | mass, pressure, temperature |
| `P01` | primary vessel wall | strain, temperature, leakage |
| `P02` | interstitial boundary | pressure, concentration, liquid |
| `P03` | source nozzle | mass flow, pressure, command |
| `P04` | primary isolation | travel, differential pressure, leakage |
| `P05` | bay atmosphere | gas, oxygen, flame, heat |
| `P06` | source-liquid drain | flow, identity, mass |
| `P07` | firewater drain | flow, identity, temperature |
| `P08` | relief riser | two-phase flow, pressure, temperature |
| `P09` | receiver or sump | mass, pressure, composition |
| `P10` | gas-holder inlet | flow, pressure, direction |
| `P11` | gas-holder volume | volume, pressure, temperature |
| `P12` | last-resort disposition | flow, ignition, destruction |
| `P13` | adjacent source face | heat, pressure, fragment, strain |
| `P14` | exclusion field | gas, pressure, heat, weather |
| `P15` | evidence boundary | time, packet, power, custody |

Every controlled drawing must identify the planes it exposes. Every event protocol must say where stimulus is applied and where protected state is observed. “Cell pressure” or “gas detected” is not specific enough to decide propagation.

### 7.2 Channel architecture

The planning lane contains 354 channels across eighteen functions:

| Function | channels | rate |
| --- | ---: | ---: |
| compartment mass | 8 | 100 Hz |
| liquid mass flow | 8 | 1 kHz |
| gas mass flow | 8 | 1 kHz |
| vessel pressure | 12 | 10 kHz |
| vessel temperature | 24 | 100 Hz |
| interstitial state | 16 | 1 kHz |
| high-range gas concentration | 16 | 100 Hz |
| low-range gas concentration | 16 | 100 Hz |
| oxygen displacement | 12 | 10 Hz |
| thermal radiation | 48 | 1 kHz |
| flame onset | 24 | 10 kHz |
| dynamic pressure | 48 | 100 kHz |
| structure and support | 48 | 10 kHz |
| sump inventory | 8 | 10 Hz |
| gas-holder state | 16 | 10 Hz |
| weather field | 12 | 10 Hz |
| safety energy | 24 | 1 kHz |
| event and evidence time | 6 | 100 kHz |

At eight bytes per sample, the aggregate uncompressed rate is about 50.808 MB/s. The high-rate dynamic pressure and timing channels dominate. This is intentional: propagation is a transient causal question, and aggressive down-sampling before the event has been understood destroys information that cannot be recreated.

### 7.3 Native evidence volume

The evidence schedule retains:

- 600 seconds at full rate;
- 21,600 seconds at five percent of full rate;
- two independent originals; and
- a 1.35 multiplier for headers, calibration, indexing and custody.

The result is approximately 230.461 GB per event. The 128-event safety register produces about 29.508 TB before reserve and 38.349 TB with thirty percent reserve. The inherited 576 TB vault gives a planning capacity ratio of about 15.0.

That headroom should not invite indiscriminate compression or a larger campaign. It allows failed attempts, replays and preservation of raw native channels. Summary products may be generated, but they never replace the originals.

## 8. Propagation-denial campaign

### 8.1 Protocol matrix

The campaign crosses six functions with two roots and two sites:

1. independent source boundary;
2. no common fuel manifold;
3. directional relief;
4. segregated drainage or knockout;
5. thermal-escalation barrier; and
6. fragment shadow and independent support.

This produces twenty-four protocols. Every protocol has a challenged exposure and a clean control, yielding forty-eight physical events. Clean controls use the same article class, configuration discipline, measurement planes and decision rule but omit the registered challenge stimulus. They protect the program against attributing ordinary variation to the inserted failure.

### 8.2 Protected-state metrics

Four functions—source boundary, common manifold, directional relief and segregated drainage—use transferred mass to the protected train as the governing metric. The provisional upper bound is 0.5 kg. Thermal and fragment/support functions use normalized protected-side utilization with a provisional upper bound of 0.8.

The bounds are research hypotheses. They must be accompanied by measurement uncertainty, predeclared treatment of censoring and an invalid-event rule. An observed value under the bound cannot pass if the measurement system was saturated, missing or causally ambiguous. An observed value over the bound cannot be averaged away with the clean control.

### 8.3 Event validity

A propagation event is valid only when:

- the source state and neighboring inert states were independently admitted;
- the challenge stimulus matches its registered envelope;
- all governing measurement planes are native and time-aligned;
- both originals survive and reconcile;
- the safe-state sequence is complete;
- source disposition closes within uncertainty;
- no unregistered intervention changes the outcome; and
- the independent physical authority issues a disposition.

Invalid events remain in the public register. They consume time, media and hardware, and their cause becomes part of the design record. Replacement events receive new identities.

### 8.4 Why forty-eight is a floor

Forty-eight paired events provide one challenge and one control for each root–site function. They establish coverage, not statistical generality. Boundary temperatures, source conditions, barrier aging, manufacturing variation and compound faults may require additional events. The program should add those only through a predeclared decision rule, not because an inconvenient result needs dilution.

## 9. Recovery, custody, rescue and human entry

### 9.1 Per-train recovery ledger

Every source route receives a ledger containing:

- initial source mass and uncertainty;
- receiver, sump and holder starting states;
- time history of transferred material;
- recovered material identity;
- measured destroyed or released fraction;
- residual vessel and line inventory;
- two evidence-original identifiers;
- an eighteen-field terminal packet;
- independent custody authority; and
- discrepancy disposition.

Root A closes through measured liquid capture and a named recovery vessel. Root B closes through receiver inventory, holder state and any last-resort disposition. A successful emergency action with an unclosed ledger protects life but does not qualify source preservation.

### 9.2 Remote rescue force

The cell treats rescue as a designed formation, not an emergency-service assumption. Each site package includes:

- protected refuge outside the provisional exclusion domain;
- remote casualty location and thermal/gas observation;
- robotic isolation and inspection capability;
- decontamination for liquid, vapor and suppression products;
- burn and inhalation stabilization;
- controlled medical transfer; and
- independent authority for human entry.

The first response is remote. Human entry begins only after the relevant 30- or 60-minute minimum, atmospheric and structural criteria, route condition and medical posture are independently confirmed. The consequence cell requires its own rescue package because it cannot borrow readiness from an operational lane while both are active.

### 9.3 Innovation agenda for rescue

The cell should mature technologies with direct force-wide value:

- heat- and vapor-tolerant inspection robots with intrinsically safe power;
- rapidly deployed optical gas and thermal fields that operate without a national network;
- robotic patient location and low-trauma extraction;
- autonomous decontamination and contaminated-water segregation;
- wearable exposure dosimetry whose record joins the native event packet; and
- remote medical telemetry designed for communications-denied disaster zones.

These capabilities are precisely the kind of public industrial technology that an equal Department of Resilience would create: expensive, hard, rarely justified by one locality, but transformative when standardized and procured at national scale.

## 10. Drawing and interface constitution

### 10.1 Sixty-four internal sheets

The controlled drawing register contains:

| Discipline | sheets | Required content |
| --- | ---: | --- |
| general arrangement | 8 | coordinate system, cells, zones, routes and exclusion interfaces |
| civil and containment | 8 | foundations, barriers, vaults, drainage and recovery courts |
| source quartet | 8 | pod geometry, supports, separations and route departures |
| Root A process | 8 | liquid isolation, drains, sumps, firewater and recovery |
| Root B process | 12 | relief, receivers, holders, pressure boundaries and disposition |
| safety power and control | 8 | three unlike paths, one-lines, final elements and hold-up |
| instruments and evidence | 8 | planes, channels, time, retention and custody |
| rescue and robotics | 4 | refuge, remote access, decontamination and medical transfer |

Every sheet carries a hazard-boundary identifier, measurement-plane range, stimulus or conserved quantity, root, site and authority record. A drawing is planning-complete when those fields and its controlled content are present. It remains physically unproven.

No sheet may establish exterior bodywork, styling, silhouette, cabin treatment or deployment appearance. Internal sections are allowed because they expose testable safety boundaries. Exterior form remains downstream of accepted source physics and complete-article authority.

### 10.2 Thirty-two interface records

Each of the sixteen source routes receives two records:

- a **root-native record** from the serialized source pod to its root-specific boundary; and
- a **public-handoff record** from that boundary to the public receiver or recovery object.

The separation prevents a public cell from erasing supplier or root ancestry. It also prevents a root from declaring the public receiving system outside the safety case. Each record requires twenty-four fields covering identity, configuration, materials, quantities, calibration, route state, authority, time and custody.

## 11. Workforce and sovereign institutional design

`SBD-1` requires 248 mission positions within the inherited 448-position `SA6` program envelope. The positions are not an added national total. They refine the institution required to operate the cells:

- source and root engineering;
- pressure, relief and multiphase analysis;
- civil containment and structural response;
- instrumentation, calibration and time assurance;
- independent safety-energy and control engineering;
- cell operations and maintenance;
- source recovery, hazardous-material custody and disposition;
- robotics, rescue, decontamination and medicine;
- evidence operations, reconstruction and physical acceptance; and
- program integration, finance and public data stewardship.

The important design choice is separation of authority. The operating team configures and conducts the event. The source authority admits the hazardous state. The rescue authority can stop work and controls human entry. The evidence authority judges packet validity. The physical acceptance board disposes the claim. None reports to the schedule owner for the decision it controls.

This is the germ of a resilience-industrial profession comparable to military test and evaluation, nuclear operations or flight safety. It creates a career system for proving high-consequence public-service technology instead of asking temporary contractors to certify the equipment they were hired to deliver.

## 12. Thirty-four-month execution sequence

| Months | Phase | Exit object |
| --- | --- | --- |
| 0–4 | source, limits and authority freeze | accepted source and authority constitution |
| 2–10 | internal drawing and interface release | sixty-four sheets and thirty-two records |
| 4–18 | civil courts and segregated vaults | two operational cells and one consequence cell ready for cold work |
| 8–20 | receiver and gas-holder arrays | eight receiver/holder trains accepted for commissioning |
| 12–22 | `C0` commissioning and denial trials | known-truth cold evidence and safe-state paths |
| 18–26 | limited live-source calibration | `C1` source and measurement envelopes |
| 22–30 | paired propagation exposures | forty-eight challenge/control dispositions |
| 28–33 | recovery, replay and site-loss closure | accepted custody and evidence-survival packages |
| 32–34 | independent acceptance board | source-state and downstream decisions |

The four-month increase over the previous thirty-month horizon is driven by the independent retention arrays. It is not a generic contingency. Building eight gas-holder chambers, eight pressure-receiver trains, eight liquid sumps and eight firewater vaults creates more civil work, more commissioning and more interfaces than the shared-lane design.

The overlaps are conditional. Live-source calibration cannot begin merely because the calendar reaches month 18. It requires the relevant `C0` cell, route, instruments, safety paths, recovery package and authority record. Paired propagation events cannot begin until the named protocol and challenge apparatus are accepted. The board cannot accept missing events on the promise that they will be performed later.

## 13. Fiscal correction

### 13.1 `SBD-1` allocation

| Capital use | Quantity × unit | Total |
| --- | ---: | ---: |
| operational lane courts and civil containment | 2 × USD 75M | USD 150M |
| destructive consequence cell | 1 × USD 60M | USD 60M |
| four-train gas-holder arrays | 2 × USD 36M | USD 72M |
| pressure-receiver arrays | 2 × USD 20M | USD 40M |
| segregated sump and firewater systems | 2 × USD 12M | USD 24M |
| instrumentation and native evidence | program | USD 28M |
| safety energy, remote operation and rescue | program | USD 22M |
| qualification articles and controlled media | program | USD 24M |
| **corrected capital** |  | **USD 420M** |

| Annual function | Total/year |
| --- | ---: |
| two operational lane teams | USD 14M |
| consequence-cell readiness | USD 5M |
| retention and source recovery | USD 8M |
| instrumentation and native evidence | USD 5M |
| safety, rescue and medical | USD 4M |
| controlled media and maintenance | USD 6M |
| **corrected annual support** | **USD 42M/year** |

Thirty-four months of support is USD 119M. Capital plus support creates a USD 539M program exposure. These are design allocations, not bids, appropriations or construction authority.

### 13.2 Portfolio reconciliation

`SBD-1` replaces the USD 260M capital and USD 25M/year `MCR-1` allocation. The net increase is USD 160M capital and USD 17M/year. Applied to the inherited `BRD-3R` boundary of USD 780M/157M per year, the reconciled `BRD-4R` becomes USD 940M/174M per year. Against the `CISA-1` parent boundary, it leaves USD 20M capital and USD 86M/year.

The no-credit physical-use view adds the USD 128M/41M annual shared-estate reservation. `BRD-4U` is therefore USD 1.068B capital and USD 215M/year. It leaves USD 45M/year but exceeds the parent capital boundary by USD 108M.

The overrun is a finding. It should not be repaired by quietly shrinking gas retention, pooling safety systems or crediting shared assets twice. The program has three legitimate choices in a later capital decision: enlarge the parent boundary, remove or redesign a physical requirement through accepted evidence, or assign part of the shared estate to a different controlled parent with explicit availability terms. `SBD-1` has no authority to choose among them.

### 13.3 What the correction teaches about resilience acquisition

Early civil-resilience concepts routinely underprice independence because common utilities look efficient. At small scale, one sump, one compressor or one communications node may be reasonable. At national force scale, correlated loss can destroy both service and evidence. The acquisition system therefore needs two economic views from the beginning:

- **funding ownership**, which prevents double appropriation; and
- **gross physical use**, which prevents a shared asset from being counted as simultaneously available to incompatible missions.

An equal Department of Resilience should make both mandatory for every formation and proving program. Otherwise the institution will accumulate cheap-looking plans whose common dependencies fail together during national emergencies.

## 14. Release logic and falsification

### 14.1 Gate populations

`SBD-1` closes 158 planning gates:

- 64 controlled drawing assignments;
- 16 route-train designs;
- 24 propagation protocols;
- 32 interface records;
- 3 cell packages;
- 4 drainage packages;
- 4 safety-power packages;
- 4 recovery packages;
- 3 rescue packages;
- 2 finance and schedule decisions; and
- 2 authority and custody decisions.

It leaves 188 physical gates open:

- 3 accepted cells;
- 16 accepted route trains;
- 48 executed propagation exposures;
- 24 accepted propagation dispositions;
- 72 inherited safety events;
- 8 evidence replays;
- 4 safe-state cases;
- 4 instrument packages;
- 4 recovery packages;
- 3 rescue packages; and
- 2 evidence-original survival cases.

Seven downstream gates remain blocked: `C2`, `SDEC-1`, complete-article admission, `CISA-RB1`, `CRC-E01`, production and exterior rendering.

### 14.2 What would falsify the design

The architecture fails as a source-independence design if any representative event demonstrates:

- reverse mass transfer above the accepted bound;
- protected-side thermal or fragment demand above accepted utilization;
- pressure, flame, liquid or gas passage through a common destination;
- shared safety-energy or final-element loss;
- failure to reach terminal source condition within the accepted envelope;
- inability to close source mass and disposition within uncertainty;
- loss of both independent evidence originals;
- rescue or human-entry dependence on the sibling site; or
- a gross physical-use requirement that cannot be financed without removing an accepted safety function.

The appropriate response is redesign and repeat, not relaxation by committee. Thresholds may change only through a new controlled safety argument that preserves life and propagation priorities.

## 15. Model and verification

The companion [twenty-seven-sheet planning model](../../../models/force/generation/f36-cisa40-sa6-internal-cell-and-source-boundary-design-constitution.xlsx) contains the source quartet, geometry, route screens, root-specific trains, retention arrays, no-common-path register, safety logic, sensors, evidence volume, planes, drawing and interface registers, protocols, exposures, safe state, recovery, rescue, schedule, capital, annual support, release gates and terminal audit.

Saved-workbook verification establishes:

- 27 worksheets;
- zero formula errors;
- 781 passing terminal audits and zero failures;
- 39 passing sensitivity tests and zero failures;
- exact restoration of all perturbed controls;
- 158 planning passes, 188 physical opens and 7 downstream blocks; and
- zero accepted physical sources.

The sensitivities challenge route count, flow velocities, retention margin, event volume, total event population, capital, annual support and release-gate counts. They verify the model's dependency structure. They do not validate DME thermodynamics, fluid transients, barrier physics, human response or cost estimates.

## 16. Research stocktake

### 16.1 What this pass resolves

The project now has a coherent internal source-boundary grammar. It knows the irreducible route object, pod geometry, receiving capacity, eleven independence domains, sixteen measurement planes, eighteen sensor functions, three unlike safety paths, paired propagation structure, recovery ledger, rescue boundary, controlled drawings, interface records, workforce, schedule and corrected cost.

It also resolves a conceptual error that would recur across the future force: emergency containment cannot be a shared afterthought when source independence is the claim. Receiving systems are part of the source topology.

### 16.2 What remains genuinely unknown

The largest technical unknown is Root B. The 500 mm route and 8,000 m³ lane holder array show scale but do not answer:

- transient flashing and choking;
- phase distribution and aerosol carryover;
- receiver pressure and temperature history;
- refrigeration and ice formation;
- heat input from fire or environment;
- backpressure and route stability;
- gas-holder deployment and material compatibility;
- ignition and measured destruction performance; or
- full mass and energy reconciliation.

Root A also retains open questions in passive diversion, drain survivability, pool control, firewater interaction and recovery. Barrier response, fragment fields, support collapse and compound failures remain open for both roots. No physical source, cell or event has been accepted.

### 16.3 What this means for the larger Department of Resilience thesis

The broader project is becoming more ambitious in the right way. The force is not merely a catalog of specialized vehicles. It is a sovereign capability system that can invent, prove, manufacture, operate and regenerate unfamiliar public-service technology under extreme conditions.

This pass illustrates the institutional depth required. A future nuclear desalination carrier, megawatt mobile cooling plant or wildfire energy aircraft would need more than a platform program. It would need controlled source states, unlike build roots, public destructive facilities, independent evidence, physical acceptance, source recovery, trained rescue formations, protected data rights and industrial regeneration. Military innovation succeeds partly because it builds the institutions that make difficult technology testable. A Department of Resilience must do the same for hazards whose purpose is rescue rather than coercion.

The economic implication is equally important. Independent safety systems are capital intensive, but they create reusable industrial products: high-rate multiphase capture, autonomous hazardous recovery, distributed safety power, high-temperature sensing, evidence-grade time systems and remote rescue robotics. A USD 1T/25-year national program could create supplier sectors around these capabilities, then export standards, equipment and trained service packages to partners facing the same hostile climate and infrastructure environment.

## 17. Next decisive pass

The next pass should create `RHT-1`, the Root B two-phase relief and deployable retention technology program. It should:

1. define the source vessel pressure–temperature envelope and representative heat inputs;
2. construct flashing, choking, pressure-loss and receiver-fill models with declared uncertainty;
3. compare direct segmented low-pressure capture, staged recovery/condensation and hybrid measured-destruction architectures;
4. specify replaceable subscale and full-scale route articles rather than committing immediately to a facility;
5. design challenge cases for obstruction, wrong-side pressure, cold soak, hot soak, partial receiver fill, energy loss and site-network loss;
6. close mass and energy at every measurement plane;
7. quantify gas-holder deployment volume, anchoring, compatible materials and regeneration;
8. establish technology down-select and stop rules before testing; and
9. return a corrected schedule and cost without borrowing authority from `SBD-1`.

Internal process diagrams, vessel sections, route sections and sensor layouts may proceed. Exterior platform form should remain blocked until `RHT-1` resolves the governing Root B physics and the Root A drainage/fire campaign has an executable physical protocol.

## Conclusion

`SBD-1` turns the two-tonne maximum credible release from a statement about compartment size into a testable architecture. Four source pods require four complete emergency destinies. Two roots at two sites create sixteen source trains. Eleven independence domains create 176 records. Six functions create twenty-four paired protocols and forty-eight propagation exposures. Sixteen measurement planes and 354 channels make the causal path observable. Three unlike safety paths preserve action when one technology fails. Recovery, rescue, evidence and finance are part of the design rather than annotations around it.

The result is more expensive than the prior concept and more honest. Reconciled funding remains inside the parent program; gross physical use exceeds its capital boundary. Static capacity closes for `C2`; physical authority remains blocked. The drawing package is complete enough to begin internal engineering; exterior form remains unavailable.

That is the standard an equal Department of Resilience requires. It should not inherit mature-looking platforms and improvise safety afterward. It should create the public institutions, industrial technologies and evidence systems that allow unprecedented rescue capability to be ambitious without becoming opaque.
