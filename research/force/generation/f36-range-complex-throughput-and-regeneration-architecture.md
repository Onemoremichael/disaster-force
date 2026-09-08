# F36 range-complex throughput and regeneration architecture

## Executive judgment

The F36 proving campaign cannot be scheduled by counting two damage cells and dividing twenty-six runs between them. Each credit-bearing event occupies a chain of scarce physical services: article preparation, fixture configuration, pre- and post-event metrology, controlled stimulus, quarantine, cleaning, water assay, forensic opening, evidence replay, blind-truth custody and return to a known state. If any one service is sized at average demand, it becomes the hidden clock for the entire program.

This architecture treats the proving range as a deployable production system for trustworthy decisions. It sizes the complex from the ninety-eight credit-bearing events established in Pass 103—seventy-two closure articles and twenty-six full-bore damage runs—then adds stochastic invalid events, one bounded repeat policy, physical reset and the loss of a complete campus. A negative-binomial planning approximation converts prospective invalid-event rates of fifteen percent for closure work and twenty percent for damage work into P90 campaign loads of ninety closure attempts and thirty-seven damage attempts. These rates are research assumptions, not observed performance.

The arithmetic produces three distinct answers:

- three closure bays and three damage cells are the mathematical minimum with no asset loss and no queue margin;
- four of each can finish after losing one cell, but leave concentrated queue risk; and
- six closure bays and six damage cells, distributed two per campus across three unlike campuses, preserve the campaign after losing an entire campus while keeping residual P90 utilization near 62.1 percent and 54.5 percent respectively.

The six-cell architecture is the mature requirement. It deliberately rejects the idea that a national proving institution should be built to the mathematical minimum. Each campus is a complete truth-producing island with two closure bays, two 120 m damage cells, two water laboratories, two metrology detachments, two evidence-replay cells, one forensic line, one blind-configuration shop, independent source and receiver loops, grid-forming power, clocks, custody, waste handling and safe shutdown. No campus owns the only instance of a decisive service.

Supporting services are sized against their own work rather than copied from the fixture count. The P90 campaign creates 365 forensic line-days, approximately 6,600 water-assay panels, 254 pre/post metrology brackets, 2,392 independent replay hours and thirty blind events. The mature estate therefore carries three forensic lines, six water laboratories, six metrology detachments, six replay cells and three blind shops. A complete campus loss leaves every service above its required throughput and retains unlike authorities.

The range uses regenerative inventory rather than one-time project stock. Twenty-four closure-article positions, eighteen instrument packs, twelve root-adapter sets, sixty registered injury cassettes, eighteen damage-cell sensor/actuator packs, twelve contamination modules, twelve traveling calibration packages and protected challenge lots keep reset work outside the critical path. A cell does not become ready because the article was removed. It becomes ready only after waste custody, cleaning, inspection, reference checks, configuration sealing and evidence closure return it to a registered state.

The architecture requires approximately 1,230 direct public personnel and a 1,850-person qualified industrial affiliate pool. It is an operational command, not a facility-management contract. Five-team shift systems, cross-campus augmentation, independent authorities and a protected training reserve permit continuous events without borrowing the people whose absence the campaign is meant to expose.

The capital boundary is USD 4.480B and annual support is USD 0.398B. Both are cross-classified inside the Pass 101 first-article boundaries of USD 8.120B and USD 0.446B/year. They include the Pass 102 protocol and its nested Pass 103 truth infrastructure; they are not additive appropriations. The range complex consumes 55.2 percent of the first-article capital boundary and 89.2 percent of annual support, revealing that trustworthy tempo is predominantly a standing-workforce and regeneration obligation rather than a one-time construction problem.

Twenty-two planning and physical gates preserve the distinction between a capacity design, constructed assets, commissioned service lanes and an admitted campaign. The planning package may advance. Site acquisition, construction, staffing, cell commissioning, loss rehearsal, first-wave execution, root credit, production and rendering remain held or blocked. No concept rendering is authorized.

## 1. The decision this architecture owns

Pass 102 defined the experiment. Pass 103 defined how the range proves its own measurement chain. Neither established how much public capacity is required to execute those decisions without forcing root order, erasing independence or making invalid events politically unaffordable.

This architecture owns seven decisions:

1. the planning attempt load after prospective invalid events;
2. the complete cycle time for each station, including reset and evidence closure;
3. the minimum, one-cell-loss and mature site-loss capacity for each service lane;
4. the physical distribution of those lanes across independent campuses;
5. the reset inventory and workforce required to sustain continuous operation;
6. the schedule that preserves root balance, blind integrity and forensic closure; and
7. the capital and annual boundaries of the resulting public institution.

It does not accept a site, award construction, commission a fixture, validate an invalid-event probability, admit a technical root or select a production form.

## 2. The throughput unit is an admitted decision

The range output is not a test start, a completed pressure cycle or an emptied cell. Its output is one terminal event packet admitted as `ADMITTED`, `FAILED` or `INVALID` by the evidence board. Until the packet reaches a terminal state, the event continues to occupy institutional capacity even if the physical article has left the fixture.

```text
ARTICLE READY
      │
      ▼
CONFIGURATION + PRE-BRACKET
      │
      ▼
PHYSICAL EVENT
      │
      ▼
SAFE RECOVERY + QUARANTINE
      │
      ├──────────► WATER / SAMPLE CHAIN
      ├──────────► FORENSIC OPENING
      └──────────► DUAL EVIDENCE REPLAY
                         │
                         ▼
                 FINAL ADMISSION
                         │
                         ▼
                 CELL KNOWN-READY
```

The station clock and the decision clock overlap but do not substitute for each other. A cell may begin reset while independent evidence work continues only when the causal boundary is sealed and the reset cannot change the event's retained truth. Conversely, a clean packet cannot release a fixture whose physical state remains unknown.

### 2.1 Five capacity states

Every station occupies exactly one of five states:

| State | Meaning | Capacity credit |
| --- | --- | ---: |
| `READY` | configuration, references, blanks, people and reset stock are valid | 1.0 |
| `OCCUPIED` | registered event or mandatory hold is underway | 0.0 |
| `RESETTING` | cleaning, repair, calibration or evidence sealing is incomplete | 0.0 |
| `RESERVE_READY` | commissioned and protected from routine scheduling | 1.0 only after declared activation |
| `OUT` | unsafe, uncalibrated, unstaffed or configuration-unknown | 0.0 |

An asset count without state is not capacity. The national scheduler may consume only `READY` tokens and may not plan routine work against `RESERVE_READY` capacity.

## 3. Demand and stochastic attempt load

### 3.1 Planning approximation

For `n` required credit-bearing events and prospective invalid probability `p`, the expected attempt count is:

`E[A] = n / (1 − p)`

The negative-binomial variance is approximated as:

`Var[A] = n p / (1 − p)^2`

The planning P90 count uses a normal approximation with `z = 1.2816`, rounded upward:

`A90 = ceil(E[A] + 1.2816 × sqrt(Var[A]))`

| Lane | Required credits | Invalid assumption | Expected attempts | P90 attempts |
| --- | ---: | ---: | ---: | ---: |
| closure | 72 | 15% | 84.71 | 90 |
| damage | 26 | 20% | 32.50 | 37 |

The approximation is intentionally simple and inspectable. Once commissioning generates mounted data, the Department must replace the assumed rates and normal approximation with empirical cause-specific distributions and a preregistered discrete-event simulation. Until then, P90 is a design load, not a probability claim about the finished range.

### 3.2 Bounded repeat policy

Invalid work cannot create an unlimited retry entitlement.

- A first invalid event caused by an independently verified range fault may return the same matrix position to the queue once if blind truth remains protected.
- A second invalid event on the same service lane freezes the lane and opens a common-cause review before any replacement event.
- A valid article failure receives no automatic repeat. A later event must be a separately authorized causal experiment and does not erase the failure.
- An `INDETERMINATE` result may receive one repeat only when the evidence board identifies the uncertainty to be retired and freezes the changed method before execution.
- Root teams receive equal retry law; schedule pressure cannot create a waiver.

The P90 load carries planning room for invalidity. It does not override these stop rules.

## 4. Complete station cycles

Cycle time includes every physical predecessor to the next `READY` state.

### 4.1 Closure bay: eight calendar days

| Segment | Calendar days | Exit condition |
| --- | ---: | --- |
| receive and configuration survey | 0.75 | article and root adapter accepted into custody |
| install, instrument and pre-bracket | 1.25 | mounted reference and independent load path close |
| process and proof program | 4.17 | 100 instrumented hours complete |
| safe removal and quarantine | 0.50 | article transferred without losing evidence |
| fixture reset and post-bracket | 0.75 | cleaning, inspection and reference checks pass |
| schedule/weather allowance | 0.58 | controlled local variation absorbed |
| **Total** | **8.00** | **bay returns to `READY`** |

The 100 instrumented hours remain the Pass 103 planning target. Continuous unattended operation is prohibited unless the safety and evidence authorities have commissioned that specific mode.

### 4.2 Damage cell: fourteen calendar days

| Segment | Calendar days | Exit condition |
| --- | ---: | --- |
| cassette/article installation | 2.0 | active 120 m article and injury system sealed |
| pre-bracket, blanks and custody | 1.0 | metrology and sanitary entry close |
| injury and six-hour restoration event | 1.0 | safe terminal service state recorded |
| quarantine and sample recovery | 2.0 | water, waste and article custody separate |
| article removal and forensic transfer | 2.0 | damage truth preserved outside cell |
| decontamination and utility recovery | 3.0 | blanks, drains and source/receiver loops clean |
| cassette, actuator and sensor reset | 2.0 | mechanical and configuration references pass |
| schedule/weather allowance | 1.0 | controlled local variation absorbed |
| **Total** | **14.0** | **cell returns to `READY`** |

The cell reset is a measured regeneration event. A visibly clean cell with a failed blank, missing waste ledger or changed actuator baseline remains `RESETTING`.

## 5. Fixture capacity result

Productive capacity discounts calendar time by a prospective availability factor that includes planned maintenance, reference work, staff training, local weather and ordinary corrective work. Closure bays use 68 percent over a fourteen-month campaign window; damage cells use 65 percent over twelve months.

### 5.1 Closure bays

The P90 closure load is 720 bay-days: ninety attempts at eight days. One bay supplies approximately 289.765 productive bay-days over fourteen months.

| Architecture | Bays available | Productive bay-days | P90 utilization | Judgment |
| --- | ---: | ---: | ---: | --- |
| mathematical minimum | 3 | 869.295 | 82.8% | completes only with all bays; concentrated queue risk |
| one-bay-loss minimum | 4 total / 3 residual | 869.295 residual | 82.8% | finishes after one loss but exceeds mature utilization target |
| mature three-campus force | 6 total / 4 after campus loss | 1,159.060 residual | 62.1% | preserves schedule after loss of two co-located bays |

### 5.2 Damage cells

The P90 damage load is 518 cell-days: thirty-seven attempts at fourteen days. One cell supplies approximately 237.413 productive cell-days over twelve months.

| Architecture | Cells available | Productive cell-days | P90 utilization | Judgment |
| --- | ---: | ---: | ---: | --- |
| mathematical minimum | 3 | 712.238 | 72.7% | all cells must survive; no independent reserve |
| one-cell-loss minimum | 4 total / 3 residual | 712.238 residual | 72.7% | finishes after one loss but remains above target |
| mature three-campus force | 6 total / 4 after campus loss | 949.650 residual | 54.5% | preserves schedule after loss of a two-cell campus |

The Pass 102 pair of damage cells remains the first commissioning unit, not the mature national capacity. Pass 104 adds a second pair and a protected third pair. This is not duplication for its own sake: it prevents the first site's design, water loop, software, staff or utility island from defining the only path to evidence.

## 6. Three unlike campuses

The National Resilience Proving Complex contains three campuses separated by electrical control region, source-water system, watershed, transport corridor, network provider, waste-disposal chain and primary staffing pool.

| Campus | Mission posture | Closure bays | Damage cells | Water labs | Metrology teams | Replay cells | Forensic lines | Blind shops |
| --- | --- | ---: | ---: | ---: | ---: | ---: | ---: | ---: |
| `NRC-A` | high-tempo hydraulic and cold-region campus | 2 | 2 | 2 | 2 | 2 | 1 | 1 |
| `NRC-B` | hot/contaminated and dense-civil-interface campus | 2 | 2 | 2 | 2 | 2 | 1 | 1 |
| `NRC-C` | protected reserve, transfer and independent reproduction campus | 2 | 2 | 2 | 2 | 2 | 1 | 1 |
| **National estate** |  | **6** | **6** | **6** | **6** | **6** | **3** | **3** |

`NRC-C` is not a warehouse. One closure bay and one damage cell remain `RESERVE_READY`; the second pair executes commissioning, reference work, cold reproduction and surge. Its staff and utilities exercise continuously so activation is a state transition, not a mobilization promise.

### 6.1 Campus-island boundary

Each campus owns a complete local chain:

- source, receiver, buffer and high-rate hydraulic loops;
- grid-forming electric power with black-start capability and non-electric safe shutdown;
- local water treatment, challenge isolation, quarantine and waste accountability;
- independent time, edge capture and original evidence storage;
- lifting, access, drainage and containment sized for the 120 m cell;
- local metrology, blanks and reference custody;
- root-neutral article handling and protected blind-truth paths; and
- food, shelter, communications and shift support for isolated continuous operation.

A shared national network, vendor portal, crane fleet, assay reagent lot, signing root or central scheduling service may improve efficiency. None may be required to reach safe state, preserve originals or continue the residual campaign.

## 7. Closure-bay architecture

Each closure bay is a reconfigurable full-bore production and measurement station rather than a fixed joint tester. It provides public containment, hydraulic stimulus and independent observation while preserving the article-owned closure kernel.

The mature bay requires:

- removable source and receiver manifolds outside the active article boundary;
- independent axial-load towers and full-section geometry metrology;
- root-neutral floor, overhead handling and exclusion volumes;
- swappable environmental shrouds for cold, hot, wet and contaminated preparation;
- isolated article power and process-data interfaces;
- dual original evidence capture and witness-clock distribution;
- robotic leak capture and cleanable sanitary boundaries;
- rapid root-adapter exchange verified by reference spools; and
- a protected maintenance position that does not consume a test bay.

### 7.1 Bay technology campaign

The Department should drive a **software-defined full-bore fixture**: modular load frames, distributed fiber and acoustic metrology, machine-surveyed adapters and physically enforced configuration envelopes that can accept unlike root geometries without using custom range tooling to finish the article. The objective is a bay whose public measurement configuration changes in hours while its independent truth remains stable.

## 8. Damage-cell architecture

Each damage cell is a contained civil-infrastructure battlefield. It must impose registered injury, soil, water, debris, exclusion, settlement and receiver states while allowing the article to detect, isolate, access, repair, prove, flush and release service using only deployed capability.

### 8.1 Cassette cell

The 120 m active article runs through replaceable injury, soil and contamination cassettes. Sacrificial cell liners, modular drains, removable source/receiver interfaces and robotic survey reduce reset time without simplifying the service problem. Injury actuators remain public and independently measured; repair machines remain article-owned.

The cassette system is designed for:

- clean transection, crush, puncture/tear, closure pullout and settlement families;
- sealed combined injuries whose delivered geometry is not disclosed before disposition;
- inward-gradient contamination challenges with mass-balance recovery;
- root-specific article supports charged to the article rather than the range;
- rapid safe removal without changing the opened damage truth;
- independent post-event scanning before destructive transfer; and
- replacement of damaged cell structure without replacing the whole facility.

### 8.2 Technology campaign

The Department should fund self-characterizing injury cassettes, autonomous contamination recovery, high-rate cleanable receiver loops, robotic liner exchange, embedded load-path tomography and remote forensic transfer. The goal is not theatrical destruction. It is repeatable, registered harm followed by a measured return to a known cell state.

## 9. Supporting-lane sizing

### 9.1 Forensic lines

Planning assigns two line-days to each P90 closure attempt and five to each damage attempt:

`90 × 2 + 37 × 5 = 365 line-days`

One line provides approximately 298.288 productive days over fourteen months at 70 percent availability. Three lines, one per campus, leave two after campus loss and 596.575 productive line-days. Residual utilization is 61.2 percent.

Each line combines nondestructive scanning, registered sectioning, microscopy, water/material recovery and evidence packaging. It may not be organizationally subordinate to the builder or initial acceptance team.

### 9.2 Water laboratories

Planning assigns twenty-four assay panels to each closure attempt and 120 to each damage attempt:

`90 × 24 + 37 × 120 = 6,600 panels`

One laboratory provides approximately 3,323.775 panels over twelve months at fourteen panels per day and 65 percent availability. Six laboratories leave four after campus loss, supporting 13,295.1 panels at 49.6 percent residual utilization. The estate preserves primary, split-sample, blank/recovery and surge functions without making one laboratory both sole operator and sole judge.

### 9.3 Metrology detachments

Two full pre/post brackets for each P90 attempt create 254 bracket events. One detachment provides approximately 212.905 brackets over fourteen months at five per week and 70 percent availability. Six detachments leave four after campus loss and operate at 29.8 percent residual utilization. The apparent spare capacity is intentional: detachments also maintain reference artifacts, travel between campuses and conduct unlike-primary comparisons.

### 9.4 Evidence replay

Planning assigns ten replay hours to each closure packet and eight to each damage packet, then duplicates the work across two independent authorities:

`2 × (90 × 10 + 37 × 8) = 2,392 replay-cell hours`

One replay cell provides approximately 3,798.6 hours over twelve months at sixteen hours per day and 65 percent availability. Six cells are justified by independence and campus survival rather than raw compute. After campus loss, four cells operate at only 15.7 percent utilization, leaving capacity for forensic replays, software diversity, migration tests and older campaign reproduction.

### 9.5 Blind-configuration shops

The campaign plans thirty blinded closure and damage states. One shop could manufacture them at the assumed rate, but one shop would make a single custody chain decisive. Three shops—one per campus—leave two after loss and operate below twenty percent of nominal event capacity. The unused time belongs to challenge development, clean-control manufacture, truth verification and rekeying, not unregistered production work.

## 10. Common-cause constitution

Redundancy is false when nominally separate assets inherit one failure root. The range registry therefore records independence at the subsystem level.

| Common-cause family | Required separation |
| --- | --- |
| electric power | unlike grid regions, local grid-forming islands and non-electric safe shutdown |
| source/receiver water | separate source systems, treatment trains, buffers and quarantine paths |
| controls | independently buildable baselines and at least two implementation roots |
| time | local holdover, separate witness sources and no sole network dependency |
| evidence | two original authorities, local stores and delayed reconciliation |
| lifting/access | campus-owned cranes and alternate manual/robotic recovery paths |
| sanitary assay | unlike reagent lots, methods and split laboratories |
| waste/discharge | separate holding capacity and more than one disposition route |
| workforce | separate shift pools plus cross-campus qualification and protected reserve |
| transport | more than one heavy route and campus-resident reset stock |
| cyber/signing | separate trust roots, offline operation and revocable local credentials |
| weather/hazard | geographic separation sufficient to avoid one declared regional event |

### 10.1 Required loss rehearsals

Before full campaign admission, the complex rehearses:

1. complete loss of `NRC-A` during active work;
2. national network and external-time denial;
3. revocation of one controls/signing root;
4. contaminated source-water discovery;
5. grounding of one actuator or crane family;
6. invalidation of an assay reagent lot;
7. closure of one waste-disposition path;
8. quarantine of one shift pool;
9. regional hazard denial of one campus; and
10. disagreement between original evidence authorities.

The rehearsal succeeds only when active events reach safe states, original evidence survives, blinded truth remains controlled and the residual estate produces a new schedule inside the frozen campaign deadline.

## 11. Regeneration and reset inventory

### 11.1 Ready-stock floors

| Stock | National floor | Logic |
| --- | ---: | --- |
| closure article positions | 24 | four ready positions per bay; root-balanced queue |
| closure instrument packs | 18 | three packs per bay permit calibration rotation |
| root-adapter sets | 12 | two per bay; adapter change does not await repair |
| registered injury cassettes | 60 | P90 damage load plus challenge diversity and damaged-stock reserve |
| damage sensor/actuator packs | 18 | three per cell for installed, calibration and reserve states |
| contamination modules | 12 | two per cell; clean and challenged states separate |
| traveling calibration packages | 12 | two per metrology detachment |
| protected challenge lots | 24 | separate lots across analyte and particle families |
| evidence media sets | 18 | three independent field-replaceable sets per replay cell |

Stock below a floor does not automatically stop a safe active event. It blocks release of the next token that depends on that stock.

### 11.2 Regeneration clocks

| Object | Return-to-known-state target | Terminal evidence |
| --- | ---: | --- |
| closure bay after ordinary event | 72 hours after article removal | cleaning, inspection, post-bracket and configuration seal |
| damage cell after contaminated event | 240 hours after article removal | waste close, blanks, actuator survey and reference acceptance |
| water laboratory after high challenge | 24 hours | carryover blank and method-control recovery |
| forensic line after opened article | 48 hours | tool/material custody and blank work surface |
| replay cell after software fault | 4 hours | unlike implementation reproduces frozen control packet |
| blind shop after integrity event | 8 hours | credentials rekeyed and truth inventory reconciled |
| lost modular station | 30 days | one replacement lane commissioned |
| lost campus | 180 days | complete local chain independently recommissioned |

The thirty- and 180-day clocks require modular reserve structures, prequalified utilities, stored controls, trained teams and public technical data. Insurance or a future construction contract is not regeneration capacity.

## 12. Workforce and command

The range requires a permanent technical force because event tempo, evidence separation and safe regeneration cannot be assembled from occasional contractors.

| Community | Direct personnel | Function |
| --- | ---: | --- |
| closure-bay operations | 240 | six bays, five-team shift system and maintenance reserve |
| damage-cell operations | 330 | six cells, injury systems, containment and reset |
| sanitary laboratories | 120 | six laboratories, splits, controls and mobile assay |
| forensic lines | 90 | scanning, sectioning, microscopy and custody |
| metrology detachments | 96 | six teams, reference estate and traveling transfer |
| evidence replay and time | 72 | six cells, two implementations, clocks and migration |
| blind/configuration shops | 45 | truth manufacture, custody, clean controls and rekeying |
| campus utilities and safety | 120 | grid islands, water loops, waste, fire and safe shutdown |
| command and evidence boards | 42 | requirements, schedule, admission, cost and dissent records |
| mobile reserve and training | 75 | augmentation, qualification, casualty replacement and exercise control |
| **Direct public force** | **1,230** |  |

A qualified 1,850-person industrial affiliate pool supplies heavy fabrication, specialized maintenance, reference renewal, software reproduction and modular-station replacement. Affiliates do not replace public decision authorities or the core shift force.

### 12.1 Five-team shift system

Each continuously operating station family uses four rotating teams and one team in training, maintenance support or reserve. The fifth team is not excess labor. It prevents qualification, illness, investigation and leave from becoming unrecorded overtime or contractor substitution.

## 13. Campaign flow

The range architecture fits inside the Pass 102 thirty-month protocol:

| Wave | Months | Principal output |
| --- | --- | --- |
| `RC01` final site and modular-station design | 1–5 | three-campuses baseline and interfaces |
| `RC02` site islands and long-lead plant | 3–10 | power, hydraulic, water, waste and evidence islands |
| `RC03` closure bays and support lanes | 6–13 | six closure bays plus metrology, laboratories and replay |
| `RC04` damage cells and cassette estate | 7–15 | six cells and registered injury inventory |
| `RC05` station and campus commissioning | 10–18 | all known-state and common-cause gates closed |
| `RC06` closure campaign | 15–28 | seventy-two credit-bearing positions and bounded repeats |
| `RC07` damage campaign | 18–29 | twenty-six credit-bearing positions and bounded repeats |
| `RC08` forensic, replay and final admission | 16–30 | all packets terminal; residual dissent preserved |

The schedule uses rolling admission. It does not wait for every closure event before beginning eligible damage work, and it does not allow a damage event to outrun its root-specific closure prerequisite.

### 13.1 Queue discipline

The National Range Scheduling Authority allocates tokens rather than appointments. A token names the root, matrix position, fixture configuration, required support lanes, blind state, predecessor packet and latest admissible start. It becomes executable only when every named service holds a compatible `READY` state.

Queue rules include:

- root balance across campus, calendar period, team and environmental condition;
- no more than two consecutive credit-bearing events from one root;
- work-in-process caps of twelve closure positions and four damage positions per campus;
- no scheduling against protected reserve capacity;
- no support-lane double booking across physical and evidence work;
- no silent acceleration by dropping post-brackets, blanks, sections or replays; and
- automatic rescheduling after a common-cause declaration using the same frozen priorities.

## 14. Range command as force structure

The complex belongs to a **National Resilience Proving Command** with three campus commands and five national functional authorities:

1. Range Operations Authority controls safe physical execution and reset.
2. Metrology and Reference Authority owns traceability and mounted-state brackets.
3. Evidence and Time Authority owns original records, clocks and replay.
4. Sanitary and Environmental Authority owns water, waste, blanks and release interfaces.
5. Truth and Forensic Authority owns blind states, opening and causal reconciliation.

The National Range Scheduling Authority sits outside campus operations. The Evidence Admission Board sits outside scheduling. The Acquisition and Industrial Mobilization Command funds and learns from the estate but cannot direct a result.

This is the same institutional ambition that a military department applies to test ranges, arsenals and operational evaluation. The Department of Resilience requires permanent sovereign places where complex civil systems can fail at full scale without making evidence, safety or environmental custody subordinate to program momentum.

## 15. Technology portfolio created by throughput

Throughput is not merely an argument for more concrete. It creates a focused technology program.

### 15.1 Modular destructive infrastructure

Develop factory-built 120 m cell segments, replaceable injury cassettes, sacrificial contamination liners, self-surveying load frames and standardized source/receiver islands. The goal is to regenerate a destroyed test lane in thirty days rather than reconstruct a bespoke range.

### 15.2 Autonomous reset

Develop robots for confined cleaning, liner exchange, geometry survey, contamination recovery, sensor replacement and registered tool custody. Automation earns credit only when it shortens a measured reset segment while preserving blanks, human stop authority and evidence.

### 15.3 Traveling primary-quality metrology

Develop rugged pressure, flow, geometry, force, time and water-transfer systems that carry primary-quality traceability between campuses. This technology later travels with deployed water, power, hospital and thermal formations so field commissioning does not depend on a surviving local laboratory.

### 15.4 Evidence-native industrial controls

Develop controllers that separate command, observation, quality flag, uncertainty, operator authority and clock state at the source. Deterministic replay and offline signing become public interfaces. A supplier dashboard remains optional.

### 15.5 High-rate sanitary truth

Develop closed challenge-water ecosystems, rapid multi-method field assays, automated mass-balance recovery and reusable quarantine modules. These capabilities directly support desalination carriers, mobile hospitals and emergency distribution systems.

### 15.6 Forensic production lines

Develop robotic large-section tomography, water-compatible sectioning, automated plane registration and material-history correlation. The output is a reproducible causal package, not a collection of photographs.

### 15.7 Range logistics compiler

Develop a scheduling and inventory compiler that conserves fixture, people, reference, sample, waste, evidence and reset states together. The compiler may propose a schedule. It cannot create readiness, waive a gate or modify blind truth.

## 16. Nested capital and annual support

### 16.1 Capital: USD 4.480B

| Use | USD B | Physical object |
| --- | ---: | --- |
| six closure bays | 0.780 | root-neutral full-bore stations and maintenance positions |
| six damage cells | 1.440 | 120 m cells, cassettes, containment and injury systems |
| campus hydraulic and utility islands | 0.540 | source, receiver, power, water, waste and black start |
| six sanitary laboratories | 0.300 | primary, split, control and mobile laboratory capacity |
| three forensic lines | 0.270 | scanning, sectioning, microscopy and custody |
| metrology estate | 0.210 | six detachments, traveling packages and primary comparisons |
| evidence and replay estate | 0.150 | six replay cells, clocks and local stores |
| three blind/configuration shops | 0.090 | truth manufacture, vaults and clean controls |
| site separation and custody | 0.240 | protected transport, storage, security and independent networks |
| reset stock and modular reserve | 0.250 | adapters, instrument packs, cassettes and replacement modules |
| controlled program reserve | 0.210 | uncertainty retirement and failed-asset replacement |
| **Total** | **4.480** | **inside Pass 101 USD 8.120B** |

The range-complex boundary includes the Pass 102 USD 1.480B protocol estate and its nested Pass 103 USD 0.420B commissioning slice. Those figures are views of the same first-article capital, not layers to add together.

### 16.2 Annual support: USD 0.398B/year

| Use | USD B/year | Persistent service |
| --- | ---: | --- |
| public workforce and training | 0.140 | 1,230 direct personnel and qualification cycles |
| utilities, water and waste | 0.060 | isolated operation, challenges and accountable disposition |
| maintenance and reset | 0.065 | return-to-known-state work and modular repair |
| metrology and reference renewal | 0.030 | traveling transfer and artifact replacement |
| sanitary laboratories | 0.028 | assays, blanks, splits and challenge lots |
| forensic operations | 0.020 | scanning, sectioning and causal packages |
| evidence, time and cyber | 0.018 | two originals, replay, clocks and signing roots |
| blind truth and custody | 0.012 | sealed manufacture, vaults and rekeying |
| campus transport and protection | 0.015 | heavy routes, security and cross-campus movement |
| readiness and exercise reserve | 0.010 | loss rehearsals and surge activation |
| **Total** | **0.398** | **inside Pass 101 USD 0.446B/year** |

Annual support consumes 89.2 percent of the parent boundary. This is an important correction: a full-scale proving force is labor-, maintenance- and custody-intensive. If the parent annual boundary cannot sustain it, the correct response is to revisit the parent allocation, not to disguise permanent work as capital or contractor contingency.

## 17. Release ladder

The range-complex model uses twenty-two gates:

1. credit demand and stochastic attempt load complete;
2. closure and damage cycle clocks complete;
3. closure-bay capacity closes after campus loss;
4. damage-cell capacity closes after campus loss;
5. forensic capacity closes after campus loss;
6. sanitary-laboratory capacity closes after campus loss;
7. metrology capacity closes after campus loss;
8. evidence-replay capacity closes after campus loss;
9. blind-shop capacity and separation close;
10. three-campus architecture is complete;
11. common-cause separation is specified;
12. reset stocks and regeneration clocks are complete;
13. workforce and shift system reconcile;
14. campaign schedule closes inside month thirty;
15. capital remains inside Pass 101;
16. annual support remains inside Pass 101;
17. planning package is complete;
18. constituted authorities approve sites and construction;
19. all three campus islands are commissioned;
20. all service lanes are commissioned and staffed;
21. complete-campus loss rehearsal passes; and
22. first campaign wave is admitted.

The first seventeen gates close in planning. Construction, physical commissioning, loss rehearsal and campaign execution remain held. Root acceptance, production, internal form and exterior rendering remain governed by the parent F36 chain and are blocked.

## 18. What this pass changes

### Established in planning

- an admitted decision packet, not a fixture event, is the range output;
- prospective invalidity expands the campaign to ninety closure and thirty-seven damage attempts at P90;
- mathematical minimum, one-cell-loss minimum and mature campus-loss capacity are different decisions;
- the mature force requires six closure bays and six damage cells across three complete campuses;
- supporting laboratories, forensics, metrology, replay and truth shops are independently sized;
- regenerative stock and return-to-known-state clocks are force structure;
- 1,230 public personnel and 1,850 qualified affiliates form the operating base; and
- range throughput consumes USD 4.480B capital and USD 0.398B/year inside the first-article boundary.

### Falsified

Seven shortcuts no longer survive:

- two damage cells are sufficient because only twenty-six runs are planned;
- fixture availability determines campaign throughput;
- a removed article makes a station ready;
- compute capacity determines evidence independence;
- co-located duplicates protect against a site-level common cause;
- invalid events can be repeated until a preferred result appears; or
- public proving infrastructure is mainly a one-time capital expense.

### Still provisional

Invalid-event rates, cycle times, availability factors, panel and replay burdens, workforce, stock floors, site distributions, schedules and costs are prospective design requirements. No site, bay, damage cell, laboratory, shift force or modular reserve has been built. The P90 calculation is an approximation pending observed commissioning data and a preregistered discrete-event model.

### Burden created by success

The next uncertainty is operational rather than architectural. A six-cell, three-campus estate needs one exact first campaign wave that proves its token system, work-in-process limits, cross-campus custody, blinded scheduling, station reset and lost-campus rescheduling without using planning arithmetic as evidence.

### Next experiment

The next pass should define the **F36 first campaign wave and lost-campus rehearsal constitution**. It should freeze the first ninety days of closure, damage, reference, blank, forensic and replay tokens; assign shift and authority rosters; inject the loss of one campus during an active event; conserve article, sample, waste, evidence and blind truth through transfer; and specify the decision that permits the remaining campaign to continue.

## Model verification

The companion workbook contains twenty-two sheets and fifty-nine independent terminal controls. The saved-workbook formula scan and terminal audit contain zero failures. Ten disposable perturbations behave causally and are restored: higher closure or damage invalidity and lower productive availability breach the residual-utilization ceiling; an incomplete campus record, capital mismatch or annual-support mismatch revokes planning authorization; construction approval releases no later physical state; downstream physical counts cannot bypass an absent predecessor; and rendering authority alone remains blocked. Every sheet is rendered and visually inspected after export.

The final workbook is 58,901 bytes with SHA-256 `69222352eb299fe4759464786ab85c215972829bcb479883c40a5ebb3bef1ea3`.

## Authority and limitations

This is a clean-sheet force-design architecture under the project's full-authorization assumption. It deliberately does not analyze current site ownership, statutes, procurement custom or political feasibility. It uses internal program lineage and no external sites. It is not a construction estimate, staffing authorization, safety case, environmental permit or observed queue model.

The companion workbook owns the stochastic attempt approximation, station cycles, service-lane capacity, campus distribution, common-cause rules, reset stocks, workforce, schedule, nested finances and release logic. The paper owns their institutional interpretation. Neither contains physical evidence.

All planning inputs remain prospective. Capacity gates can authorize only further design. Site, construction, commissioning, campaign, production, form and rendering decisions require their own constituted authorities and physical records.

## Related work

- [F36 fixture commissioning and first-run data constitution](f36-fixture-commissioning-and-first-run-data-constitution.md)
- [F36 closure-kernel and full-bore damage-cell protocol](f36-closure-kernel-and-full-bore-damage-cell-protocol.md)
- [F36 supplier-neutral sector and rupture-article build-release standard](f36-supplier-neutral-sector-and-rupture-article-build-release-standard.md)
- [F36 rapid water trunkline range and first-article constitution](f36-rapid-water-trunkline-range-and-article-constitution.md)
- [Workbook: F36 range-complex throughput and regeneration architecture](../../../models/force/generation/f36-range-complex-throughput-and-regeneration-architecture.xlsx)
