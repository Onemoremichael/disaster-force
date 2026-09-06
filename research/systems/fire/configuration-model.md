# Fire response force configuration model

## Decision purpose

This pass converts the fire-force architecture into an editable configuration study. Its question is not which airtanker the Department of Resilience should buy. It is:

> What combination of distributed readiness, sensing, aircraft, airspace, bases, ground control, water and agent supply, community protection, strategic movement, workforce and research capacity can intervene before an ignition escapes—and, when interception fails, create and hold control faster than the fire creates new control requirements?

The answer is a two-force architecture. A geographically distributed **Ignition Intercept Network** (`IIN`) buys minutes. A deployable **Integrated Fire Control Group** (`IFCG`) buys massed, sustained control. The workbook shows why these cannot be collapsed into one nominally efficient formation. Under the explicit WUI reference assumptions, an intercept cell has an 81.2% modeled chance of acting before the 50-minute escape threshold but cannot close the growing control feature. The campaign group can close it, with a positive 4.77 km/h margin, but has only a 33.4% modeled chance of arriving before that threshold. The national force must overlap the two systems: local cells act while campaign formations assemble, move and take over.

The accompanying [`fire-response-force-engineering.xlsx`](../../../models/systems/fire/fire-response-force-engineering.xlsx) workbook contains 23 linked sheets. It is a design-study instrument, not a fire-behavior forecast, an aircraft specification, an incident-action plan, a cost estimate or a claim of field performance. Yellow cells are editable assumptions and controls; blue cells are calculated outputs. All four fire cases and all three formation states recalculate from the same visible logic.

This configuration advances `IIN` and `IFCG` to `R2+`: the first-order operational, mass, workforce, throughput and portfolio balances are explicit enough to direct experiments and reject internally inconsistent concepts. It does not advance an aircraft or ground vehicle to `R3`. Eighteen evidence gates remain open, and renderings remain prohibited.

## What the model changes

The most important result is architectural, not numerical.

1. **Early action and sustained control are different production systems.** Intercept probability depends on geographical distribution, alert posture, launch latency, local travel distance and decision authority. Campaign control depends on airspace density, sortie flow, base and agent capacity, connected ground line, hold probability, multi-shift labor and sustainment.
2. **Aviation is an input to control, not the product.** The baseline campaign generates almost 800 effective sorties per day, yet durable aerial line contributes only about one-quarter of effective control line after placement, interaction, completion and hold factors.
3. **Autonomous ground production is potentially decisive and therefore dangerous to assume.** Robotic tractors contribute roughly half of baseline effective line. If their productivity, autonomy, repair or communications assumptions fail together, the modeled closure margin can disappear. The research program must treat robotics as a testable force multiplier, not a balancing plug.
4. **The controlling bottleneck moves.** In the baseline, bases have substantial spare capacity, airspace is near saturation and retardant production constrains the aircraft families that require it. Buying aircraft without increasing airspace and agent-system capacity would not reproduce the modeled effect.
5. **The heavy formation is strategically heavy.** The preliminary dry deployment is about 42,339 tonnes and the external-lift share about 39,961 tonnes. A credible fire campaign force is inseparable from sealift, rail, road, reception, staging, workshops and prepositioning.
6. **Novel technology belongs inside the force equation.** The workbook does not assume that present daylight, piloting, drop, line-production or base limits are permanent. It exposes the performance increases required from sensing, autonomy, aircraft cycles, precision agents, deployable bases and robotic ground systems so the Department's research enterprise can buy down specific operational deficits.

## Workbook architecture

The model is divided into six linked analytical layers.

| Layer | Sheets | Function |
|---|---|---|
| Mission and controls | Summary & Sources; Controls; Fire Cases | Select formation and fire case; expose posture, reserve, rotation and portfolio assumptions |
| Intercept and growth | Detection Intercept; Fire Growth | Build the complete detection-to-action clock and a transparent fire-growth screen |
| Aerial system | Aircraft Families; Air Mission Cycle; Drop Yield; Airspace Capacity; Air Base Throughput | Convert owned aircraft into constrained cycles, delivered fluid and durable aerial contribution |
| Ground and civilian effect | Ground Production; Line Hold; Ground Robotics; Water Agent; Structure Defense; Smoke Thermal | Convert machines, crews, water, agents and protective systems into held line and people-centered outputs |
| Formation and institution | Deployment Manifest; Workforce Rotation; Readiness Concurrency | Calculate deployment mass, shift-complete staffing, institutional depth and national ready inventory |
| Innovation, resources and evidence | Technology Roadmap; Cost RDT&E; Failure Modes; R3 Evidence Gate | Connect unmet performance to research campaigns, capital portfolios, degraded cases and verification requirements |

The summary sheet intentionally reports effect and constraint measures together. A formation that has high sortie count but no positive closure margin is not labeled successful. A formation with positive line production but unacceptable intercept latency is not labeled an intercept force. A capital row that fits inside an allocation is not labeled affordable because the workbook is not an independent cost estimate.

## Reference formations

The model compares three formation states. These are not successive procurement blocks; they are operational echelons with different posture and employment logic.

| Formation | Posture assumption | Principal owned mission systems | Baseline dry mass | Deployed / service establishment |
|---|---|---|---:|---:|
| Ignition Intercept Cell | 40 km target distance; 16-hour air and ground period | 3 rapid aircraft, 4 amphibious aircraft, 2 vertical aircraft, 4 crews, 6 robotic tractors, local water/base/structure/smoke packages | 2,606 t | 1,393 / 5,222 |
| Reinforced Initial Attack | 70 km; 20-hour air and ground period | 6 rapid, 12 amphibious, 6 heavy, 4 vertical and 8 sensing aircraft; 16 crews; 24 robots; three bases | 14,952 t | 5,041 / 18,902 |
| IFCG Campaign | 120 km; 24-hour aviation and 20-hour ground period | 12 rapid, 24 amphibious, 16 heavy, 12 vertical and 18 sensing aircraft; 48 crews; 72 robots; six bases | 42,339 t | 12,330 / 46,237 |

The increasing target distance and launch delay are part of each posture assumption. The larger formations therefore have lower modeled probability of reaching a new ignition before escape. That does not mean a smaller formation is more capable in general. It means local readiness cannot be recovered by adding mass after an incident starts.

## Intercept model

The complete intercept clock is:

\[
T_{intercept}=T_{detect}+T_{verify}+T_{decide}+T_{launch}+T_{transit}+T_{target}
\]

The workbook carries P50 and P90 assumptions for every stage. It sums the stages to produce a total P50 and P90, then derives a screening distribution. The reported probability of action before escape uses a logistic cumulative distribution whose spread is matched to the P50–P90 interval:

\[
\sigma \approx \frac{T_{90}-T_{50}}{1.28155}
\]

\[
P(T\leq T_{escape}) \approx \frac{1}{1+e^{-\frac{T_{escape}-T_{50}}{0.5513\sigma}}}
\]

This is an analytical approximation, not an empirical arrival-time distribution. It exists to show the value of tail reduction and to provide a falsifiable target for field data. Detection, verification, dispatch, launch and first effective target action must eventually be measured as correlated distributions by geography, weather, false-alarm load, crew state and airspace condition.

For the WUI wind-driven case, the result is:

| Formation | P50 intercept | P90 intercept | Modeled action before 50-minute escape |
|---|---:|---:|---:|
| Ignition Intercept Cell | 28.2 min | 62.8 min | 81.2% |
| Reinforced Initial Attack | 45.6 min | 93.9 min | 55.3% |
| IFCG Campaign | 69.6 min | 135.4 min | 33.4% |

The implication is stronger than “respond faster.” The IIN requires permanent regional coverage, delegated civil authority, local sensor fusion, maintained alert aircraft and machines, pre-cleared operating envelopes, local water and agent access, and an escalation protocol that begins generating the campaign force before the cell is overwhelmed.

## Fire-growth screen

The workbook represents the growing fire as a constant-rate ellipse. For head-fire rate of spread `R`, elapsed time `t` and length-to-breadth ratio `q`:

\[
a=Rt,\qquad b=\frac{a}{q}
\]

It uses the Ramanujan perimeter approximation:

\[
P \approx \pi\left[3(a+b)-\sqrt{(3a+b)(a+3b)}\right]
\]

Spotting reserve expands the required control feature. After effective intervention, the workbook reduces—but does not eliminate—the growth rate using a case-specific post-intervention spread fraction. Closure occurs only if connected, held and verified line is produced faster than this continuing requirement grows.

The four cases are deliberate stressors rather than calibrated forecasts:

| Fire case | Head spread | Escape threshold | Length:breadth | Post-intervention spread | Control horizon |
|---|---:|---:|---:|---:|---:|
| WUI wind-driven | 3.0 km/h | 50 min | 4:1 | 55% | 24 h |
| Grass rapid | 5.0 km/h | 30 min | 5:1 | 50% | 12 h |
| Timber severe | 1.2 km/h | 90 min | 3:1 | 45% | 48 h |
| Timber moderate | 0.35 km/h | 180 min | 2:1 | 40% | 72 h |

The model does not claim that one constant-rate ellipse predicts an incident. Terrain, fuels, atmosphere, plume dynamics, spotting and suppression feedback are far richer. The screen is useful because it prevents a basic category error: initial perimeter is not the only control obligation; the fire continues to create new work while the force acts.

## Aircraft–base–airspace cycle

Each suppression aircraft family is evaluated as a mission cycle:

\[
T_{cycle}=T_{load/scoop}+T_{taxi}+T_{out}+T_{target}+T_{in}+T_{recover}+T_{inspect}
\]

Unconstrained sorties are aircraft quantity times integer cycles per operating period times dispatch availability. Effective sorties are the minimum of four capacities:

\[
S_{effective,f}=\min(S_{cycle,f},S_{airspace,f},S_{base,f},S_{fluid,f})
\]

The fluid constraint is applied by family. Water availability does not compensate for inadequate retardant production when a mission family requires retardant, nor does a global fluid ratio incorrectly penalize aircraft that can use another source.

For the WUI campaign baseline:

| Constraint | Result | Interpretation |
|---|---:|---|
| Unconstrained aircraft cycles | 873.84 sorties/day | Fleet-and-cycle ceiling before shared constraints |
| Effective sorties | 798.28 sorties/day | Family-specific minimum after airspace, base and fluid constraints |
| Usable airspace capacity | 921.6 operations/day | Four sectors, 12 operations/hour, 24 hours, 20% safety reserve |
| Airspace utilization | 94.8% | Near-binding shared constraint |
| Maximum base utilization | 28.8% | Considerable nominal spare capacity in this case |
| Water demand / capacity | 1.765M / 3.000M gal/day | Not binding |
| Retardant demand / capacity | 1.427M / 1.200M gal/day | Binding for relevant families; 84.1% scaling ratio |

This result gives the innovation program a concrete direction. More aircraft alone are low value at the margin if mixed-airspace capacity and agent production remain fixed. High-integrity cooperative separation, portable surveillance and command, weather-resilient navigation, faster aircraft servicing, distributed agent manufacture and more effective low-environmental-burden chemistry may buy more objective effect than a larger nominal tank.

## Drop yield and durable control

For an aerial delivery, the theoretical line screen is:

\[
L_{theoretical}=S_{effective}\left(\frac{100V}{c w}\right)(0.0003048)
\]

where `V` is payload in gallons, `c` is coverage in gallons per 100 square feet and `w` is swath width in feet. The workbook then discounts theoretical line by placement, fire interaction and ground completion. The `Line Hold` sheet applies continuity, hold probability and verification to every source of line:

\[
L_{effective}=L_{raw}\times p_{continuity}\times p_{hold}\times p_{verify}
\]

The baseline IFCG produces 411.80 km/day of effective control line:

| Source | Effective line | Share of total |
|---|---:|---:|
| Hand crews | 35.79 km/day | 8.7% |
| Conventional dozers | 69.08 km/day | 16.8% |
| Robotic tractors | 205.08 km/day | 49.8% |
| Aerial contribution | 101.86 km/day | 24.7% |
| **Total** | **411.80 km/day** | **100%** |

The initial WUI control feature at P90 arrival is 50.81 km. After intervention, the modeled required feature continues growing at 12.38 km/h. The formation produces effective line at 17.16 km/h, yielding:

\[
M_{closure}=17.16-12.38=+4.77\text{ km/h}
\]

The modeled time to close the initial feature is 10.64 hours. This is not a containment forecast. It is a consistency check that the assumed formation has positive production margin in the selected case.

The concentration of nearly half of effective line in robotic tractors is the workbook's most consequential technology dependency. It defines an Advanced Resilience Projects Agency (`ARPA-R`) program target: optionally crewed machines must demonstrate productive navigation in smoke, dust, heat and broken terrain; safe separation; tool effectiveness; local stop; intermittent-communications operation; recovery; field repair; and line-quality verification. Until those demonstrations exist, the robotics contribution is an explicit hypothesis and a common-mode failure risk.

## Scenario comparison

The 12 formation–fire combinations reveal four different force-design regimes.

| Fire case | Formation | Action before escape | Effective line | Closure margin | Modeled closure |
|---|---|---:|---:|---:|---:|
| WUI wind-driven | IIN cell | 81.2% | 30.23 km/day | −11.12 km/h | no closure |
| WUI wind-driven | Reinforced | 55.3% | 149.55 km/day | −6.15 km/h | no closure |
| WUI wind-driven | IFCG | 33.4% | 411.80 km/day | +4.77 km/h | 10.64 h |
| Grass rapid | IIN cell | 53.0% | 42.98 km/day | −13.96 km/h | no closure |
| Grass rapid | Reinforced | 32.1% | 211.54 km/day | −6.94 km/h | no closure |
| Grass rapid | IFCG | 19.8% | 597.77 km/day | +9.15 km/h | 7.77 h |
| Timber severe | IIN cell | 98.5% | 30.23 km/day | −2.65 km/h | no closure |
| Timber severe | Reinforced | 89.4% | 149.55 km/day | +2.32 km/h | 5.85 h |
| Timber severe | IFCG | 67.3% | 411.80 km/day | +13.25 km/h | 1.48 h |
| Timber moderate | IIN cell | 100.0% | 37.31 km/day | +0.58 km/h | 4.40 h |
| Timber moderate | Reinforced | 99.8% | 183.99 km/day | +6.69 km/h | 0.57 h |
| Timber moderate | IFCG | 98.0% | 515.12 km/day | +20.49 km/h | 0.27 h |

Three judgments follow.

First, early cells can plausibly intercept but should not be expected to contain every fast-moving case unaided. Their doctrine should include buying time, protecting priority objectives, marking control opportunities and preserving safe handoff—not only achieving independent containment.

Second, a reinforced initial-attack echelon is useful but not automatically sufficient. It closes the timber cases under these assumptions but not the rapid WUI or grass cases. The Department should not allow an intermediate organizational label to conceal negative closure margin.

Third, even the campaign force arrives after the assumed escape threshold in many fast cases. The mature architecture therefore needs both standing regional cells and a campaign reserve; predictive positioning and early generation orders are part of operational capability, not administrative optimization.

## Civilian protection outputs

The workbook includes two non-containment outputs to keep public purpose visible.

- The structure-defense screen produces 4.7 effective cluster-defense equivalents per day in the baseline. This is a work-throughput measure, not a structure-survival probability.
- The smoke and thermal package produces 146,880 public clean-air person-hours per day. This does not establish safe exposure because building leakage, filter performance, heat load, occupancy, accessibility and behavior are not yet modeled.

These outputs prevent the force from equating a contained perimeter with a successful campaign. A fire can be operationally bounded after large civilian loss, or remain uncontained while targeted protection saves communities, lifelines and health. Future models must attach consequence weights, evacuation and shelter decisions, medical load and post-fire watershed stabilization to the same operational timeline.

## Deployment and strategic mobility

The campaign formation has a preliminary dry deployment mass of 42,338.98 tonnes after a 15% configuration contingency. Approximately 39,960.8 tonnes require external movement. Operating fuel, water stocks, recurring agent, route-specific bridging, host-site works and some reception equipment are excluded.

This mass has institutional consequences.

1. National fire response cannot be designed independently of the Department's strategic lift and theater-opening forces.
2. A substantial share of bases, agent plant, robots, structure-defense kits and support equipment should be prepositioned in risk-weighted regional sets.
3. Rail and sealift matter even for a nominally aviation-centered mission because the campaign echelon's ground and support mass dominates rapid interregional movement.
4. Configuration control must distinguish alert packages, fly-away elements, follow-on ground echelons and replenishment flow.
5. The Department needs movement tables and reception exercises, not merely asset ownership.

The baseline workforce is 12,330 deployed people. Applying the explicit 3.75 institutional rotation multiplier produces 46,237.5 service billets for one continuously generatable IFCG-equivalent establishment. This includes relief depth but is not a complete national occupational model. The workforce sheet still relies on provisional positions per unit, shifts, relief and common-support assumptions. Qualification bottlenecks, seasonal concurrency, academy throughput, reserve activation, medical surveillance, family support and retention are open.

## National order-of-battle and capital screen

The national screen assumes 30 planned IIN cells and eight planned IFCGs, 75% package readiness, requirements for 12 simultaneous ready cells and three ready campaign groups, and a 25% procurement reserve. This yields 22 ready IIN cells and six ready IFCGs under the simple readiness rule. Correlated maintenance, regional hazard covariance, combat-style attrition analogues, training draws and damaged bases are not yet represented.

The illustrative aviation order of battle is:

| Family | Owned aircraft | Assumed airframe acquisition screen |
|---|---:|---:|
| FA-1 persistent fire sentinel | 233 | $11.65B |
| FA-2 rapid attack | 390 | $23.40B |
| FA-3 regional amphibious suppressor | 160 | $16.00B |
| FA-4 heavy line builder | 120 | $30.00B |
| FA-5 precision lift/suppression rotorcraft | 255 | $25.50B |
| **Total** | **1,158** | **$106.55B** |

The airframe screen is quantity times assumed unit acquisition cost. It is not the aviation program cost. The $250B aviation portfolio therefore leaves $143.45B for research, development, test, spares, training systems, bases, depots, software, mission equipment, attrition, production risk and other lifecycle-enabling capital. Calling that balance “savings” would reproduce the platform-only accounting error the project rejects.

The full $1T real-2026 capital/RDT&E thought experiment remains allocated across research, aviation, ground control and water, sensing and communications, bases and depots, community protection, strategic stocks, training/test infrastructure and program reserve. Routine personnel and operations remain outside the tranche. No row is an appropriation recommendation or independent cost estimate.

## Technology strategy

The model converts technological ambition into performance campaigns rather than speculative silhouettes. The Department should deliberately pursue capabilities beyond the current state of practice where they alter an operational constraint:

- **minutes-to-intercept:** persistent multimodal sensing, onboard verification, false-alarm rejection, delegated decision support and high-cycle regional alert systems;
- **continuous mixed airspace:** portable surveillance, cooperative separation, degraded-visual navigation, resilient local communications and progressive certification for optionally crewed and autonomous operations;
- **objective-yield aviation:** clean-sheet aircraft optimized around cycle life, maintainability, precision placement, austere servicing and system availability rather than maximum tank size;
- **robotic control line:** optionally crewed machines, autonomous tool control, line-quality sensing, local stop, remote recovery and high-temperature maintainability;
- **water and agent independence:** rapidly deployable pump/pipe networks, distributed mixing, closed-loop quality control and environmentally acceptable agents with higher persistence or lower required volume;
- **community-scale ember defense:** fast-installing, weather-tolerant systems that protect clusters rather than isolated demonstration structures;
- **human endurance:** filtered rest, heat recovery, exposure sensing, shift design and medical surveillance as readiness technology; and
- **model-to-test infrastructure:** calibrated fire digital twins, instrumented ranges, standardized objective-yield trials and an independent test authority empowered to disprove program claims.

The workbook's role is to make these programs accountable. A new capability should enter the model by changing a visible parameter, constraint or uncertainty distribution. It should not be credited to the force until evidence demonstrates the change under representative conditions and the complete mission thread still closes.

## Failure modes

The model retains explicit degraded cases because a nominally balanced formation can fail through its interfaces.

| Failure | Why the baseline is vulnerable | Required design response |
|---|---|---|
| Detection or communications loss | Intercept probability depends on the entire tail clock | independent sensing paths, edge verification, disconnected authority and manual fallback |
| Airspace capacity loss | baseline utilization is 94.8% | sectorization, portable surveillance, priority logic, lost-link procedures and graceful sortie shedding |
| Retardant-system loss | baseline retardant demand exceeds capacity | distributed plants, alternate formulations, water-capable tactics, stocks and fault isolation |
| Robotic common-mode failure | robots provide 49.8% of effective line | mixed crewed/optionally crewed fleet, local control, recovery teams and conservative credit until tested |
| Base closure | aircraft effect depends on servicing and queue control | dispersed bases, mobile cells, alternate-source mission cycles and rapid relocation |
| Line breach or poor continuity | raw production does not equal held control | instrumented inspection, redundant line, patrol, mop-up and probability-based reserve |
| Workforce exhaustion | machinery availability does not imply crew availability | independent personnel readiness, filtered rest, exposure limits and relief movement |
| Strategic-movement delay | nearly 40,000 t require external lift | prepositioned sets, echeloned manifests, rail/sealift contracts and exercised reception |

## Verification

The delivered workbook was subjected to four checks.

1. **Structural inspection:** all 23 intended sheets are present; formulas, controls, validation lists, number formats and source URLs were inspected after export.
2. **Scenario switching:** all 12 formation–fire combinations recalculated, and the delivered file was restored to the `IFCG Campaign` / `WUI wind-driven` baseline.
3. **Formula integrity:** pre-export and post-import scans found zero spreadsheet error values.
4. **Independent arithmetic:** 124 checks reproduced intercept totals and probability, aircraft cycles, minimum constraints, drop geometry, ground production, line-hold arithmetic, closure margin and time, deployment mass, workforce, capital totals, acquisition rows, the $143.45B aviation remainder, formula-error status and byte identity between the generated and repository copies. No check failed.

Every sheet was also rendered and reviewed for clipping, overlap, unreadable tables and broken charts. Verification demonstrates workbook coherence, not truth of assumptions.

## Limitations and R3 evidence gate

The principal limitations are material.

- Fire cases use simple constant-rate elliptical growth and illustrative escape thresholds, not calibrated regional fire-behavior ensembles.
- The arrival probability is a logistic approximation built from assumed P50 and P90 stage times; stages are not yet empirical correlated distributions.
- Aircraft payload, cycle, availability, drop, interaction and fatigue coefficients remain design hypotheses.
- Airspace and base capacities are deterministic screens rather than stochastic queues with failures, weather and mixed mission priority.
- Ground-production and hold factors do not yet contain fuel, slope, access, fatigue and breach distributions.
- Robotic productivity carries disproportionate weight without field evidence under smoke, heat, dust, broken terrain and communications loss.
- Structure-defense equivalents and clean-air person-hours are throughput screens, not demonstrated survival or health outcomes.
- The deployment manifest is preliminary and excludes operating stocks and route-specific works.
- Workforce coefficients do not yet represent qualification scarcity, training throughput or seasonal availability.
- National readiness uses an independent percentage rather than a reliability and correlated-demand model.
- Capital values are portfolio design assumptions and airframe acquisition screens, not lifecycle cost estimates.

All 18 gates in the workbook remain open: regional cases; intercept distributions; calibrated growth; aircraft–base–crew cycles; objective-yield trials; line production and hold; water, agent, fuel and base balances; mixed-airspace safety; vehicle loads and maintainability; robotics; structure defense; public and responder exposure; itemized deployment; workforce; concurrency; environmental fate; lifecycle cost and production; and independent complete-thread testing.

`IIN` and `IFCG` therefore stop at `R2+`. The next pass should not draw a rapid-attack aircraft, robotic tractor or deployable base. It should select the highest-leverage assumptions exposed here—robotic line productivity, mixed-airspace capacity, agent throughput and the intercept tail—and replace them with test plans, empirical distributions, subsystem configurations and sensitivity-driven technology requirements. Rendering begins only when a specific system reaches `R3` and can be shown inside its complete operating formation.
