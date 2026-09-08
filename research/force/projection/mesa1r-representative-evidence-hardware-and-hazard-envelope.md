# MESA-1R: representative evidence hardware and hazard envelope

## Executive judgment

The measurement force described in [MESA-1](mesa1-measurement-and-destructive-evidence-architecture.md) cannot remain a diagram of authorities, channels and custody rules. Its equipment has mass. Its batteries occupy volume. Its clocks reject heat. Its storage must survive isolation. Its terrain sensors alter the contact system whose pressure they are supposed to prove. A serious proving enterprise must therefore design the evidence formation as physical hardware before it can claim that a representative vehicle or service system has been tested.

`MESA-1R` makes that correction. It selects five supplier-neutral planning articles: a `110 kg` atmospheric-tile evidence cassette, a `135 kg` terrain-tile cassette, a `1.2 t` atmospheric-carrier truth node, a `2.6 t` terrain-carrier truth node and a `2.8 t` civil-effect receiver station. Each carries its own sensing, acquisition, computation, clock, storage, energy, isolation and environmental protection. Each is allocated for a complete `168 h` evidence interval with no mission power and no network required for local survival. The selections are representative burdens for prototyping, not production designs.

The result overturns two placeholders inherited from MESA-1. The generic `75 kg` article kit is too small once seven-day energy is included. The generic `350 kg` carrier kit is much too small, especially on terrain. The article corrections remain inside the smallest `550 kg` certified tile-family allowance established in [ESK-40V](esk40v-physical-tile-and-carrier-interface-closure.md), so the service-tile mass ratings do not need to reopen. The carrier corrections do change the tested machines. The atmospheric carrier rises from `1,468.322 t` to about `1,469.301 t` in its instrumented configuration. The terrain carrier rises from `720.957 t` to about `723.786 t` after its mass-feedback term.

That terrain correction exposes the central finding of this pass: **measurement hardware consumes the margin it is intended to prove**. Instrumented ground pressure rises from `34.2492 kPa` to approximately `34.3836 kPa`. The remaining separation to the `34.75 kPa` evidence threshold falls to `0.3664 kPa`; the rule permitting expanded uncertainty to consume at most half the physical margin therefore limits `U95` to about `0.1832 kPa`. The earlier MESA-1 design allocation of `0.2209 kPa` would no longer be admissible. MESA-1R responds with a denser `4,560`-cell, `18,240`-channel pressure-and-geometry system and a revised planning allocation of `0.1292 kPa`. This passes the arithmetic screen but remains entirely unproved.

The evidence system is consequently a separate industrial formation, not an electronics option. It requires its own battery packs, pressure-skin production, replaceable wear layers, calibration platens, denied-time clock ensembles, immutable media, thermal enclosures, depots, mobile laboratories and independent maintenance workforce. A USD `6.8B` eight-campaign prototype subportfolio is nested inside the existing USD `24B` `F01` sovereign metrology family. The reallocation changes the unit assumptions for atmospheric and terrain hardware without changing the family total or the USD `1.050T` proving portfolio.

All `342` deterministic workbook controls pass. That statement means the selected allocations reconcile with the model. It does not mean the hardware works. All ten physical gates remain `OPEN`, production remains on `HOLD`, and exterior and internal renderings remain `BLOCKED` until a frozen representative full-mission campaign closes the measured mass, volume, access, heat and hazard envelopes.

## 1. The instrument paradox

A weak test architecture assumes that instruments observe a machine without changing it. That assumption may be tolerable for a bench component with generous margin. It is unacceptable for a compound service carrier already governed by narrow mass, energy, timing and ground-contact boundaries.

The instrument changes at least six things.

1. **Mass and inertia.** Batteries, enclosures, pressure skins and harnesses change gross weight, load transfer, braking, articulation and unload state.
2. **Volume and access.** Evidence hardware occupies protected internal volume and changes inspection, escape, maintenance and cooling paths.
3. **Heat.** Independent electronics and energy storage reject heat into or through the article. That heat may help a cold system, injure a hot system or change thermal signatures and materials.
4. **Power quality.** Even a nominally passive tap can change impedance, grounding, isolation and fault propagation. Independent power eliminates one class of mission dependency but creates its own fire and protection burden.
5. **Surface mechanics.** A pressure skin changes compliance, friction, hysteresis, wear and effective contact. The terrain carrier is therefore not representative merely because its sensor reads accurately.
6. **Human and software behavior.** Visible instrumentation can alter operator decisions, maintenance intensity and builder tuning. A network path intended for export can become a hidden diagnostic advantage.

The appropriate response is not to make the equipment disappear conceptually. It is to register the instrumented configuration as a distinct test article and pair it with controlled removal trials.

For every decisive mission, MESA-1R requires three physical states:

| State | Evidence configuration | Purpose |
| --- | --- | --- |
| Instrumented | complete evidence hardware installed and active | measures mechanism, boundary physics and civil effect |
| Emulated | evidence hardware removed; matched inert mass, center of gravity, impedance and heat substituted | separates sensing and software effects from physical burden |
| Bare | production-intent article without temporary evidence package | detects residual configuration effect and establishes final representativeness |

No pair is automatically equivalent. Instrumented-to-emulated comparison tests whether measurement signals or operation change the mission. Emulated-to-bare comparison tests whether the imposed test burden changes the mission. A favorable instrumented result cannot be transferred to production unless both comparisons remain inside registered bounds.

This is a more demanding doctrine than ordinary telemetry qualification, but it is proportional to the claim. The force is trying to certify that a very large machine can create safe public service in a damaged place, under compound loss, without hidden prepared support. The configuration used to observe that claim must be part of the claim.

## 2. Physical constitution of the evidence formation

MESA-1 established three logical planes: embedded control (`P0`), independent mechanism evidence (`P1`) and civil-effect witness (`P2`). MESA-1R converts the latter two into five physical nodes. They are not universal boxes. Atmospheric tiles, terrain tiles, carriers and civil receivers face different observability and survival problems.

### 2.1 Atmospheric tile cassette

The atmospheric cassette is allocated `110 kg`, `0.22 m³`, `55 W` average power, `180 W` peak power and `8 TB` of local write-once storage. Its dominant burden is the `52.5 kg` battery needed to carry `11.55 kWh`: `168 h × 55 W × 1.25` nameplate reserve. The remaining mass provides passive isolation, structural and load witnesses, electrical and fluid probes, acquisition, evidence compute, a diverse clock ensemble, enclosure and outward thermal rejection.

The cassette is a sealed article-level witness. It receives one-way signals and cannot command the tile. It must remain with the tile through handling, carriage, deployment, operation and reset so the evidence record does not begin only after favorable installation. Its enclosure must make a battery failure non-propagating without borrowing the tile's fire protection.

The increase from `75 kg` is material for test logistics but not for certified tile-family rating. The smallest family retains `550 kg` of planning allowance for evidence hardware. The cassette uses one fifth of that amount, leaving space for measured mounting and configuration corrections without altering the service payload.

### 2.2 Terrain tile cassette

The terrain cassette is allocated `135 kg`, `0.28 m³`, `65 W` average, `220 W` peak and `8 TB`. It carries separate structural, fluid, thermal, motion and geometry channels because a terrain tile experiences shock, soil, debris, water ingress, articulation and repeated field handling that are not atmospheric analogues. The `62.05 kg` battery allocation covers `13.65 kWh` with the same reserve rule.

Its enclosure is not merely a rugged version of the atmospheric box. It needs a replaceable contamination boundary, inspectable passive signal paths and a custody scheme that survives mud, decontamination and removal from a damaged carrier. The cassette's motion record must remain independent of the carrier navigation solution so loss of navigation does not erase article pose or contact history.

### 2.3 Atmospheric carrier truth node

The atmospheric carrier node is allocated `1.2 t`, `2.8 m³`, `0.8 kW` average, `2.2 kW` peak and `24 TB`. It witnesses the governing carrier phenomena: twenty-four lift cells, six conversion trains, six energy buses, twelve propulsion pods, sixteen contact feet, atmospheric state, unloading geometry and variable-buoyancy exchange. Its `763.64 kg` battery allocation is deliberately large because seven days at `0.8 kW` with reserve requires `168 kWh` of independent energy at the assumed pack-level `0.22 kWh/kg`.

The node is not expected to sample every high-rate sensor continuously at its nameplate peak. The average is a registered duty-managed evidence load; peak power protects coincident capture, clocking and local computation. Duty control may defer derived computation but may not suppress raw records around registered physical events or delete invalid-state evidence.

The atmospheric node adds `850 kg` above the prior placeholder. Applying the inherited `1.1512 t` gross response per tonne of fixed added mass produces about `0.9795 t` of carrier-gross increase. The instrumented atmospheric carrier is therefore its own configuration at approximately `1,469.301 t`. A qualification result at that mass is conservative for some loads but not automatically representative for unloading, buoyancy conversion, contact reaction or control behavior.

### 2.4 Terrain carrier truth node

The terrain node is allocated `2.6 t`, `8.5 m³`, `0.6 kW` mission-average power, `3.5 kW` peak and `24 TB`. Its defining element is not the computer or battery. It is a `1.14 t` replaceable sensing skin over the carrier's `285 m²` deployed contact system.

The remaining allocation includes independent optical and subsurface geometry, a traveling-platen calibration interface, isolated acquisition, evidence compute, immutable storage, denied-time clocks, `572.73 kg` of battery, passive harnesses and an environmental enclosure. This tight allocation is a design challenge in its own right. If representative vendors cannot meet it, the carrier requirement must reopen; the model may not hide the excess in generic structure.

The node adds `2.25 t` above the earlier `350 kg` placeholder. With the terrain gross-feedback coefficient, the instrumented carrier rises by about `2.829 t` to `723.786 t`. The increase appears small beside the vehicle, but the decisive pressure margin is already small. This is why instrumentation cannot be treated as percentage noise.

### 2.5 Civil-effect receiver station

The receiver station is allocated `2.8 t`, up to `12 m³`, `1.2 kW` average, `3.2 kW` peak and `64 TB`. It is separately powered and controlled by the civil-effect authority. Its instruments observe water assay and custody, electrical waveform and protection, flow and pressure, occupied thermal conditions, accessibility and lawful public release. A civil release ledger binds the physical service boundary to the authority that admits use.

The receiver is deliberately not installed as a carrier subsystem. A machine can report excellent outlet conditions while the public boundary fails because of a contaminated connection, unsafe grounding, an inaccessible distribution point or a withheld civil release. Separate physical custody prevents the service provider from defining the receiver's success condition.

The station's energy allocation requires approximately `1,145.46 kg` of batteries under the planning specific-energy assumption. Its enclosure must prevent that independent energy store from becoming an unregistered source for the mission. No jumper, shared inverter, heat loop or emergency export is allowed during a credited run.

## 3. Seven-day autonomy is a constitutional constraint

Independent evidence is not independent if it dies when the tested machine loses power. MESA-1R therefore sizes the five nodes for the full `168 h` interval plus `25%` nameplate reserve.

| Node | Average load | Required energy | Battery allocation |
| --- | ---: | ---: | ---: |
| Atmospheric tile cassette | `0.055 kW` | `11.55 kWh` | `52.50 kg` |
| Terrain tile cassette | `0.065 kW` | `13.65 kWh` | `62.05 kg` |
| Atmospheric carrier node | `0.800 kW` | `168.00 kWh` | `763.64 kg` |
| Terrain carrier node | `0.600 kW` | `126.00 kWh` | `572.73 kg` |
| Civil receiver station | `1.200 kW` | `252.00 kWh` | `1,145.46 kg` |

These masses use a `0.22 kWh/kg` pack-level planning value. The assumption is not a technology forecast and does not earn a procurement claim. It is a transparent design point. Lower specific energy increases test burden; higher specific energy creates mass margin. The prototype program must qualify cells, packs, containment, cold and hot endurance, fire propagation, state estimation and post-mission custody as one system.

The same constitutional logic governs data. Local storage is sized so loss of every external network changes delivery latency, not evidence survival. After a `25%` filesystem and custody reserve, all registered nodes retain their full raw interval. The terrain pressure field adds `3.648 MB/s`; total terrain carrier allocation is `20 MB/s`, requiring `16.128 TB` and leaving `7.872 TB` within the installed `24 TB`. The receiver requires `32.256 TB` and carries `64 TB`.

One local copy is not the final archive. It is the original survival boundary. Following a mission, originals transfer first to the independent evidence authority; builder analytic copies follow custody closure. Media faults, invalid sensors, dropped packets and time discontinuities remain explicit records. A later national archive cannot reconstruct a missing local original and cannot convert a broken mission into a complete one.

## 4. Denied time and physical event order

Clock precision matters because compound claims are ordered: arrival precedes unload; custody precedes energization; stable production precedes assay; assay precedes civil release. Yet satellite discipline cannot be assumed in the very failure worlds the force is built to enter.

The representative ensemble combines two independent atomic holdover roots with thermal characterization, traveling-reference calibration, hardware event distribution and registered readout. The provisional standard components are `0.0015`, `0.0018`, `0.0016`, `0.0020`, `0.0022` and `0.0010 s`. A root-sum-square allocation yields approximately `0.00423 s`; the coverage factor of two yields `0.00846 s`, inside the inherited `0.01 s` clock limit.

This is an architecture screen, not a claim that an oscillator will retain universal absolute time to that level in every environment. The trial must demonstrate holdover across temperature, shock, power cycling, root substitution and deliberate loss of external discipline. It must also test ancestry: two clocks built from one firmware, one calibration path or one environmental compensation model are not diverse merely because they occupy separate boxes.

Most importantly, clock closure does not solve event definition. A precisely timed controller state is not necessarily the physical instant of ground security, water stability or civil release. The evidence formation must connect clock edges to independent physical witnesses and a frozen event grammar. Better clocks protect order; they do not authorize the program to redefine success.

## 5. The soil-pressure truth system

The terrain carrier's contact claim is distributed in space and time. Twelve articulated pods traverse nonuniform damaged soil. Average force divided by nominal area can conceal local peaks, loss of contact, sinkage and shear. MESA-1R therefore makes the contact surface itself part of the metrology system.

At a `0.25 m` planning pitch across `285 m²`, the skin contains `4,560` cells. Four channels per cell register normal load, shear, temperature and health, producing `18,240` channels. At `200 Hz`, four bytes per sample and `4×` registered lossless compression, the effective stream is `3.648 MB/s`. The `4 kg/m²` replaceable-layer target produces the `1.14 t` skin allocation.

The skin cannot stand alone. It is paired with optical contact-boundary reconstruction, subsurface geometry, a geotechnical witness grid and calibration before and after the run. These paths answer different questions:

- the skin observes distributed surface load and local state;
- optical geometry observes actual contact boundary and deformation;
- subsurface witnesses observe sinkage and displaced soil;
- the geotechnical grid observes moisture, density and spatial variation; and
- the traveling platen ties local cells back to a physical load reference.

The revised planning uncertainty allocation is:

| Component | Standard uncertainty |
| --- | ---: |
| Load measurement | `0.020 kPa` |
| Contact-area reconstruction | `0.025 kPa` |
| Sinkage boundary | `0.020 kPa` |
| Peak capture | `0.030 kPa` |
| Spatial interpolation | `0.025 kPa` |
| Temperature effect | `0.010 kPa` |
| Calibration transfer | `0.015 kPa` |
| Terrain nonuniformity | `0.030 kPa` |
| **Combined standard allocation** | **`0.0646 kPa`** |
| **Expanded allocation, `U95`** | **`0.1292 kPa`** |

The instrumented carrier's modeled pressure is `34.3836 kPa`; the upper planning claim is therefore about `34.5128 kPa`, below the `34.75 kPa` threshold. The remaining separation is useful but not comfortable. Correlation, hysteresis, damage, missing cells or an optimistic contact reconstruction could consume it.

The skin also creates the very disturbance it observes. P04 therefore includes bare, emulated and instrumented runs over registered spatial blocks; layer replacement and recalibration; saturated and debris-contaminated conditions; missing-cell patterns; peak-load insertion; and post-run sectioning. If the skin changes traction or contact beyond the registered equivalence bound, the system fails even when its numerical uncertainty looks excellent.

## 6. Heat rejection and the no-crutch boundary

Seven-day batteries and evidence compute create a nontrivial thermal system. Heat must leave the evidence enclosure without aiding the tested mission. On a cold atmospheric carrier, instrument heat could reduce conditioning load. On a hot receiver, it could increase the civil burden. On terrain, enclosure heating could change pressure-skin compliance or clear moisture that a production surface would retain.

Every node therefore needs a measured outward heat path and a matched emulator. Calorimetry establishes average and transient rejection. The instrumented state, inert thermal emulator and bare state are compared under the same environment. The evidence system may use dedicated heat spreaders, phase buffers and external radiators, but it may not export useful heat to mission fluids, occupied spaces, lift gas, traction surfaces or receiver utilities.

The no-crutch rule extends beyond heat. Evidence hardware cannot:

- supply mission power;
- provide a control or diagnostic return path;
- improve navigation or communications;
- serve as ballast, structural reinforcement or environmental protection without an equivalent production element;
- provide a clean utility connection at the receiver;
- become the only surviving clock, network or compute path; or
- expose privileged live analytics to builder or operator teams during a blinded run.

The prohibition is enforced through physical interfaces, failure insertion and removal trials. Policy alone is insufficient because operational pressure will otherwise turn the proving range into an invisible service provider.

## 7. Prototype program

MESA-1R creates eight linked campaigns with `68` trials and `64` evidence gates. The USD `6.8B` program is an explicit subportfolio of `F01`; it receives no additive funding and no maturity credit before execution.

| Campaign | Object | Trials | Planning cost | Decisive falsifier |
| --- | --- | ---: | ---: | --- |
| `P01` | power and storage endurance | 8 | USD `1.0B` | any node loses the interval or borrows mission energy |
| `P02` | atmospheric and terrain tile cassettes | 10 | USD `0.7B` | mass, heat, isolation or handling fails |
| `P03` | atmospheric carrier node | 6 | USD `0.6B` | node changes unload, lift or gust behavior |
| `P04` | terrain carrier and soil skin | 12 | USD `1.5B` | uncertainty or test-mass pressure fails |
| `P05` | civil receiver station | 8 | USD `0.8B` | assay, release or rights custody fails |
| `P06` | clock custody and denial | 8 | USD `0.5B` | holdover, diversity or ancestry breaks |
| `P07` | removal and no-crutch trials | 8 | USD `0.6B` | measurement changes mission behavior |
| `P08` | frozen complete mission | 8 | USD `1.1B` | any evidence plane fails or public effect misses |

The sequence matters. P01 removes the temptation to depend on vehicle power or network service. P02 freezes representative article cassettes before they are integrated into carriers. P03 and P04 test carrier-specific effects. P05 proves that civil effect is separately observed. P06 protects event order. P07 performs the equivalence comparisons that most test programs would be tempted to waive. Only then may P08 freeze a complete formation and mission.

Each campaign has eight co-governing evidence gates. A campaign with seven favorable gates and one failed independence gate does not receive partial admission. The operational article may remain safe and useful; the design claim remains unearned.

## 8. Industrial and institutional consequence

Representative measurement equipment at this scale creates a strategic civil-metrology industry. It is not a niche instrumentation market attached to carrier prime contractors.

The Department of Resilience needs at least five durable supplier fields:

1. **Evidence cassettes and passive interfaces** for article-level structural, fluid, electrical, thermal and configuration capture.
2. **Large-area hazard skins** combining load, shear, temperature and health sensing with replaceable field protection.
3. **Independent energy and thermal containment** optimized for long-duration measurement rather than propulsion.
4. **Denied-time and immutable custody systems** with diverse hardware, calibration and software ancestries.
5. **Mobile primary references and receiver laboratories** capable of field calibration, assay, civil release and adversarial reproduction.

Carrier primes may compete to integrate these systems but should not control their original evidence, calibration chain or conformance authority. The Service Systems Proving Command needs evidence engineers, metrologists, calibration technicians, soil scientists, assay personnel, forensic maintainers, civil-release officers, time authorities, data custodians and independent trial directors as standing professions.

The `F01` capital total remains USD `24B`, but its internal equipment assumptions change. Atmospheric article cassettes receive USD `1.806B`; terrain cassettes USD `2.142B`; article integration USD `0.020B`; atmospheric carrier nodes USD `0.630B`; terrain carrier nodes USD `0.930B`; and eight receiver stations USD `1.600B`. The primary campus, distributed and mobile laboratories, paired-range arrays, offline fabric, archive, adversarial laboratory and reserve retain the balance. The prototype campaigns consume USD `6.8B` of this family, or `28.3%`.

The reallocation is intentionally budget-neutral at this stage. It is not evidence that the numbers are affordable or quoted. It says that an honest `F01` architecture can absorb mode-specific hardware by giving up generic allowances. Awarded work that exceeds any line reopens the family and then the USD `350B` facility portfolio above it.

This investment also drives technology beyond present commercial demand. The strategic opportunities include self-identifying pressure skins, mechanically transparent sensor layers, battery systems certified for long isolated custody, verifiable one-way physical interfaces, clocks with inspectable ancestry, immutable high-rate storage, automated calibration transfer and portable civil-effect laboratories. As with defense technology, the Department creates demand for capabilities that become commercially valuable after the state bears early integration and reliability risk.

## 9. Decision gates and rendering boundary

The current selection is narrow. It authorizes prototype allocations and nothing more.

| Gate | Required closure | Current state |
| --- | --- | --- |
| `H1` | weighed, sealed atmospheric and terrain cassettes fit their certified family allowances | `OPEN / HOLD` |
| `H2` | atmospheric carrier node preserves mission behavior in removal-paired trials | `OPEN / HOLD` |
| `H3` | terrain node and skin preserve the ground-pressure claim on registered soils | `OPEN / HOLD` |
| `H4` | all five nodes record 168 hours without mission energy | `OPEN / HOLD` |
| `H5` | all nodes retain the complete local interval through link loss | `OPEN / HOLD` |
| `H6` | diverse clocks demonstrate `U95 ≤ 0.01 s` through denial | `OPEN / HOLD` |
| `H7` | heat rejects outward without helping the mission | `OPEN / HOLD` |
| `H8` | removal leaves control behavior and public effect invariant | `OPEN / HOLD` |
| `H9` | receiver truth remains separate from service provision | `OPEN / HOLD` |
| `H10` | measured mass, volume, access, heat and hazard envelopes close after P08 | `OPEN / HOLD`; rendering `BLOCKED` |

No vendor, packaging geometry, material system, mounting pattern, production sensor suite or operational evidence set is selected. Even internal diagrams would imply interfaces and access paths that the prototype program has not earned. The correct next representation is a supplier-neutral interface competition and a serial prototype configuration record, not a polished vehicle image.

## 10. What this pass changes

MESA-1R converts the shadow measurement formation from a constitutional idea into an explicit physical burden.

- The generic article kit becomes two mode-specific cassettes at `110 kg` and `135 kg`.
- The generic carrier node becomes `1.2 t` atmospheric and `2.6 t` terrain configurations.
- A separate `2.8 t` receiver station protects civil-effect authority.
- Every node is allocated for seven-day independent power and complete local retention.
- The terrain pressure skin becomes a `4,560`-cell, `18,240`-channel, `1.14 t` strategic subsystem.
- Carrier-gross and ground-pressure calculations now include evidence hardware.
- The permissible terrain uncertainty narrows because the test system consumes physical margin.
- The USD `6.8B` prototype campaign and mode-specific equipment are reconciled inside the existing USD `24B` metrology family.

The pass also sharpens a general doctrine for the Department of Resilience: proof is not paperwork after engineering. Proof is a purpose-built force with its own mass, energy, logistics, authority and industrial base. When the public claim is difficult enough, the state must project measurement capacity alongside service capacity—and must be willing to let that measurement formation disqualify the machines it accompanies.

The next pass should compete supplier-neutral architectures for the cassettes, carrier nodes, pressure skin, receiver station and one-way interface; select the serial prototype configuration; and write the P01–P08 execution protocol. Renderings remain premature until representative evidence closes the internal envelopes.

## Model boundary

The companion workbook is the arithmetic authority for this pass. Its masses, powers, data rates, specific energy, uncertainty terms, costs and quantities are planning assumptions derived from the current internal force references; they are not observations, vendor quotes or probability distributions. Root-sum-square uncertainty is a design allocation pending calibrated covariance. `PASS` means a stated relationship reconciles. `OPEN` means the required physical evidence does not yet exist. No exterior or internal platform form is authorized.
