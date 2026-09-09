# F36 observed-throughput update and residual-campaign admission constitution

## Executive judgment

The first F36 wave cannot be allowed to update its own success assumptions by dividing favorable packets by all started events. The wave contains ordinary work, an intentionally induced campus denial, right-censored station histories, replacement events and decisions that may fail because of the article, the range, safety, evidence or an unresolved cause. Those states answer different questions. Pooling them would make the Department learn the wrong lesson from the most expensive evidence it has created.

This constitution freezes the update before any live first-wave result is visible. It separates intrinsic range invalidity from forced-denial consequence, article failure, safety stop and indeterminate evidence. A deliberately injected `NRC-B` loss may test the consequence of a campus shock, but it cannot estimate how often such shocks occur. A shortened, interrupted station record may describe exposure before denial, but it cannot be treated as a fast completed cycle. An article failure remains a valid technical result and never becomes a range retry merely because the campaign needs another success.

The planning model uses a transparent beta-negative-binomial posterior predictive distribution rather than carrying forward the Pass 104 normal approximation. The prior effective sample is twenty attempts: `Beta(3,17)` for closure invalidity and `Beta(4,16)` for damage invalidity. Those priors preserve the former fifteen- and twenty-percent planning means without pretending they were observations. Only completed, ordinary-exposure event packets update the intrinsic invalidity model.

No live first-wave data exist in this research package. A fully labeled synthetic conformance vector proves the estimator and release logic. It contains eighteen ordinary credited closure events, six ordinary credited damage events and the four forced-denial invalids required by Pass 105. The intervention invalids remain in the causal record but contribute zero trials and zero failures to the intrinsic-rate update. Under that synthetic vector, the exact posterior predictive P90 requirement for the remaining fifty-four closure credits is sixty-four attempts. The corresponding requirement for the remaining twenty damage credits is twenty-eight attempts.

The conformance vector also tests time and availability updates. Completed uncensored events produce one-sided ninety-percent planning cycle limits of 8.542 closure days and 15.211 damage days. Routine productive availability updates to conservative lower planning values of 65.9 and 60.7 percent. Four surviving closure bays can supply 882.09 productive bay-days over the remaining eleven-month window against 546.69 demanded, or 62.0 percent utilization. Four surviving damage cells can supply 665.13 productive cell-days over nine months against 425.91 demanded, or 64.0 percent utilization.

The residual event compiler assigns sixty-four closure and twenty-eight damage reservations to immutable station intervals. It preserves three-root primary counts, uses new identities for every possible replacement, holds closure and damage WIP at four and three, rotates damage work across four cells so one cell-equivalent remains outside WIP, and closes the last conservative closure packet by day 300.5 and the last damage packet by day 340.4. Both are inside the inherited day-425 and day-365 lane horizons. The synthetic decision is therefore **preserve the six-bay/six-cell architecture and conditionally admit two-campus residual scheduling**. This is a conformance result, not an observed campaign decision.

The physical-regeneration claim remains separate. Pass 104 set a 180-day lost-campus recommissioning target, but Pass 105 rehearsed denial rather than physical destruction. One-third of the campus-local capital estate is approximately USD 1.340B. The range carries USD 0.250B of reset/modular reserve and USD 0.210B of controlled program reserve across the whole estate. Even if every dollar were assignable to one destroyed campus, only USD 0.460B is visibly reserved, leaving a USD 0.880B replacement exposure. This does not enlarge the present program automatically. It creates a required capital decision before the Department may claim that complete-campus physical regeneration is funded.

The remaining twenty-seven months of standing range support cost USD 0.8955B at the inherited USD 0.398B annual rate. A modeled one-cell complete-chain damage augmentation would add USD 0.480B of capital and USD 0.0945B of support over the same period, producing a USD 1.470B residual outlay. The synthetic evidence does not trigger that option. It remains a quantified branch for a live result that breaches the seventy-percent utilization ceiling.

Planning can authorize the estimator, data schema, conformance tests and decision ladder. It cannot turn the synthetic vector into observed evidence. Live observation authority, complete event packets, an independent cause board, constituted rosters, residual campaign approval, root credit, production, form and rendering remain held.

## 1. The decision this constitution owns

Pass 105 established how the first wave behaves through a complete campus denial. This pass establishes how the institution is allowed to learn from that wave.

It owns six decisions:

1. which event records enter each estimator;
2. how prior planning assumptions become posterior predictive attempt requirements;
3. how completed cycle, packet and productive-availability observations change scheduling limits;
4. how common-cause intervention evidence affects consequence planning without contaminating frequency estimates;
5. how the remaining fifty-four closure and twenty damage credits receive immutable station reservations; and
6. what evidence permits the range to preserve, augment or redesign its force before residual campaign admission.

It does not declare live first-wave results, accept a technical root, restore `NRC-B`, authorize a capital supplement, select production hardware or release any exterior form.

## 2. The update is an institutional act

A model update changes future physical exposure. It decides how many articles must exist, which stations remain protected, how much time and support the remaining campaign receives and whether a root can continue. The update therefore requires the same separation of powers as a test event.

The minimum authority chain is:

```text
NATIVE EVENT RECORDS
        │
        ▼
SCHEMA + IDENTITY VALIDATION
        │
        ▼
INDEPENDENT CAUSE CLASSIFICATION
        │
        ├── article result ──► technical root record
        ├── intrinsic range cause ──► invalidity estimator
        ├── forced intervention ──► consequence model only
        ├── safety stop ──► safety model and bounded eligibility review
        └── indeterminate ──► uncertainty register
        │
        ▼
FROZEN ESTIMATOR IMPLEMENTATION
        │
        ▼
POSTERIOR PREDICTIVE DEMAND + TIME LIMITS
        │
        ▼
RESIDUAL EVENT COMPILER
        │
        ▼
ADMISSION BOARD
```

The builder, campus operator, scheduler, estimator custodian and admission board may not collapse into one authority. The estimator custodian executes the registered method. It does not reclassify cause or choose which inconvenient records to omit.

## 3. The immutable observation object

Every started event creates one observation object, whether or not the event completes. At minimum it binds:

- event token, schema version and immutable article or cassette identity;
- root, condition family, campus, station and roster identities;
- exposure class: `ROUTINE`, `FORCED_INTERVENTION` or `UNPLANNED_COMMON_CAUSE`;
- registered start, last trustworthy observation, physical release and packet-terminal times;
- terminal disposition and cause-board class;
- completed-cycle flag, right-censor flag and censor boundary;
- productive station days, packet latency and every support-service burden;
- safety stops, configuration changes and missing-record flags;
- two original locations, native record hashes and replay decisions;
- blind commitment, unblinding transition and forensic custody; and
- signatures from evidence, cause, estimator and admission authorities.

No null is silently converted to zero. `0` means the event produced a measured zero for that field. `NOT_OBSERVED` means the field was not measured. `NOT_APPLICABLE` means the registered method does not require it. A right-censored duration carries the last trustworthy exposure and a censor flag, not a fabricated completion time.

## 4. Cause classes are not interchangeable

| Class | Meaning | Updates intrinsic invalidity? | Updates cycle distribution? | Creates automatic retry? |
| --- | --- | ---: | ---: | ---: |
| `CREDITED` | complete admissible packet reaches registered credit state | yes, as non-invalid exposure | yes, if cycle is complete | no |
| `ARTICLE_FAILED` | complete packet proves the article missed a requirement | yes, as non-range-invalid exposure | yes, if cycle is complete | no |
| `INTRINSIC_RANGE_INVALID` | an ordinary range, reference, operator or support failure prevents the registered decision | yes, as invalid exposure | only with registered outcome-specific treatment | once, subject to stop law |
| `FORCED_DENIAL_INVALID` | declared exercise action makes the event impossible to complete | no | no; history is right-censored | replacement belongs to rehearsal law |
| `SAFETY_STOP` | safety authority stops exposure before a terminal technical packet | no until independent eligibility finding | no unless a complete safe cycle exists | never automatic |
| `INDETERMINATE` | evidence cannot distinguish permitted terminal states | no until cause classification | no unless complete and registered | bounded causal experiment only |
| `OPEN` | packet or cause decision is not terminal | no | no | no |

An article failure is evidence about the root, not evidence that the range was unavailable. A forced denial is evidence about shock consequence, not the background shock rate. An indeterminate packet is an unresolved obligation, not half a failure or half a success.

## 5. Exposure law

The intrinsic invalidity estimator admits an event only when all of the following are true:

1. exposure class is `ROUTINE`;
2. the event token, article, station and root identities reconcile;
3. the packet is terminal;
4. the independent cause board has assigned either intrinsic range invalid or non-range-invalid disposition;
5. every required original, clock and native record is present;
6. the event was not selected or reclassified after observing its technical result; and
7. no estimator exclusion was created outside the preregistered rule.

The denominator is eligible ordinary exposure. The numerator is independently classified intrinsic range invalidity. Forced interventions remain visible in the same event table with `eligible = 0`. This prevents exclusion from becoming deletion.

The update freezes at a declared cutoff. Events still open at cutoff do not enter the binary rate model. Their count, age and cause status appear in a separate unresolved register. The admission board cannot advance the cutoff to include a favorable packet while leaving a slow adverse packet open.

## 6. Posterior predictive attempt demand

### 6.1 Prior constitution

The Pass 104 rates were prospective design assumptions. This pass expresses them as weak prior distributions with an effective sample of twenty attempts:

| Lane | Prior mean | Prior effective attempts | Prior invalid parameter | Prior non-invalid parameter |
| --- | ---: | ---: | ---: | ---: |
| closure | 15% | 20 | 3 | 17 |
| damage | 20% | 20 | 4 | 16 |

The effective sample is strong enough to prevent six or eighteen clean events from erasing design caution and weak enough to let several independently classified intrinsic invalids change the plan. It is a policy prior. It is not retrospective data.

For prior `Beta(α,β)`, observed eligible invalids `x` and eligible non-invalids `m − x`, the posterior is:

`q | data ~ Beta(α + x, β + m − x)`

### 6.2 Exact predictive distribution

For `r` remaining credits and `k` future invalid events before those credits are obtained, the beta-negative-binomial predictive probability is constructed by recurrence. The zero-invalid probability is:

`P(K=0) = product from j=0 to r−1 of (β′ + j) / (α′ + β′ + j)`

Subsequent probabilities are:

`P(K=k+1) = P(K=k) × ((k+r)/(k+1)) × ((α′+k)/(α′+β′+r+k))`

The required attempt count is `r + k` at the first cumulative probability at or above 0.90. This preserves posterior parameter uncertainty directly. It does not insert an upper invalid-rate estimate into the old normal approximation.

### 6.3 Synthetic conformance result

| Lane | Eligible ordinary events | Intrinsic invalids | Forced-denial invalids excluded | Posterior | Remaining credits | Predictive P90 attempts |
| --- | ---: | ---: | ---: | --- | ---: | ---: |
| closure | 18 | 0 | 2 | `Beta(3,35)` | 54 | 64 |
| damage | 6 | 0 | 2 | `Beta(4,22)` | 20 | 28 |

The reduction from the original planning burden does not mean the campus loss was harmless. It means an induced shock is not evidence about intrinsic event invalidity. Its consequence remains in the two-campus capacity and common-cause branches.

## 7. Cycle and packet-time update

Only complete, uncensored station histories enter the ordinary cycle estimator. The registered one-sided planning limit is:

`U90 = max(registered cycle, sample mean + 1.2816 × sample standard deviation × sqrt(1 + 1/n))`

This is a small-sample prediction screen, not a claim that station times are normally distributed. The live successor must preserve the empirical distribution and replace the screen with resampling or a validated event-time model after enough observations exist. The first update uses the screen because eighteen closure and six damage completions cannot support a stable tail model.

The same rule applies to packet latency. Cycle time governs physical station return to `READY`. Packet latency governs evidence-queue closure. Neither may substitute for the other.

| Lane | Complete uncensored cycles | Mean days | Sample deviation | Registered days | Planning cycle U90 | Packet-latency U90 |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| closure | 18 | 8.161 | 0.289 | 8.000 | 8.542 | 6.556 |
| damage | 6 | 14.500 | 0.514 | 14.000 | 15.211 | 8.844 |

The four forced-denial histories remain right-censored at the loss boundary. Treating their three-day and one-day observed exposures as completed cycles would reduce the schedule burden precisely because the campus was destroyed. The conformance suite must reject that error.

## 8. Productive availability update

Availability uses at-risk asset-days, not total calendar days. The declared `NRC-B` denial is excluded after day 38 because the assets are no longer at risk of routine readiness; they are absent from the residual force. An at-risk asset-day reconciles among productive, planned-unavailable and unplanned-unavailable states.

For each service, the prior mean from Pass 104 receives an effective sample of sixty asset-days. Observed productive and nonproductive asset-days update a beta distribution. The planning availability is the lower one-sided moment bound:

`L90 = posterior mean − 1.2816 × posterior standard deviation`

The value is bounded between zero and one. Missing state time or an unreconciled asset-day blocks the update rather than lowering the denominator.

The synthetic service ledger yields:

| Service | Eligible asset-days | Productive-equivalent days | Posterior mean | Planning L90 |
| --- | ---: | ---: | ---: | ---: |
| closure bays | 434 | 298.0 | 68.6% | 65.9% |
| damage cells | 350 | 222.5 | 63.8% | 60.7% |
| forensic lines | 217 | 152.0 | 70.0% | 65.8% |
| sanitary laboratories | 434 | 280.0 | 65.0% | 62.3% |
| metrology detachments | 434 | 295.0 | 68.1% | 65.4% |
| evidence replay cells | 434 | 281.0 | 65.0% | 62.3% |
| blind/configuration shops | 217 | 143.0 | 65.7% | 61.4% |

The exact values belong to the workbook and synthetic vector. Live productive time must come from immutable station state transitions, not retrospective timesheets or the scheduler's expected availability.

## 9. Residual demand and capacity

The posterior predictive attempt counts drive every support demand. For the remaining campaign:

| Service | Updated demand | Residual capacity basis | Productive capacity | Utilization |
| --- | ---: | --- | ---: | ---: |
| closure bays | 64 × 8.542 = 546.69 bay-days | 4 bays, 11 months, 65.9% | 882.09 bay-days | 62.0% |
| damage cells | 28 × 15.211 = 425.91 cell-days | 4 cells, 9 months, 60.7% | 665.13 cell-days | 64.0% |
| forensic lines | 268 line-days | 2 lines, 11 months, updated availability | workbook-calculated | below 70% |
| sanitary laboratories | 4,896 panels | 4 labs, 11 months, 14 panels/day | workbook-calculated | below 70% |
| metrology detachments | 184 brackets | 4 teams, 11 months, 5/week | workbook-calculated | below 70% |
| evidence replay cells | 1,728 hours | 4 cells, 11 months, 16 hours/day | workbook-calculated | below 70% |
| blind/configuration shops | 36 conservative blind states | 2 shops, 11 months, 2/week | workbook-calculated | below 70% |

The blind count includes eighteen remaining registered blind primaries plus all eighteen predictive excess attempts. It assumes every possible replacement receives fresh blind truth. This is deliberately conservative.

Aggregate utilization is necessary but insufficient. The event compiler must also prove station non-overlap, WIP, root balance, reserve posture, packet queue and terminal deadline on the actual reservation calendar.

## 10. Residual event compiler

### 10.1 Closure reservations

Sixty-four closure reservations use four surviving bays. The first fifty-four are primary credit intentions: eighteen for each root. The final ten are contingent range-invalid replacements with no root assigned before causal activation.

The compiler assigns consecutive four-event waves across `CB-A1`, `CB-A2`, `CB-C1` and `CB-C2`. Wave spacing equals the conservative 8.542-day cycle divided by 65.9-percent planning availability. This protects ordinary unavailable time between registered events rather than assuming every bay immediately starts the next article.

### 10.2 Damage reservations

Twenty-eight damage reservations rotate across `DC-A1`, `DC-A2`, `DC-C1` and `DC-C2`. Only three events may be in damage-cell WIP at once, so one cell-equivalent always remains protected; the idle identity rotates rather than creating an unexercised fixed spare. The first twenty primary intentions preserve the inherited root remainder: six `R1`, six `R2` and eight `R3`. Eight contingent replacements receive no root until an eligible range cause exists.

Three-event waves are separated by the conservative 15.211-day cycle divided by 60.7-percent planning availability. The last damage packet closes by day 340.4, before the day-365 lane horizon.

### 10.3 Daily laws

The compiled schedule must satisfy every day:

- no station carries more than one active token;
- closure WIP does not exceed four;
- damage WIP does not exceed three;
- at least one surviving damage cell remains protected;
- every primary root count matches the residual matrix;
- no contingent token is treated as a credit before activation;
- packet queues remain inside the registered support ceiling;
- the last closure packet is no later than day 425; and
- the last damage packet is no later than day 365.

The conformance calendar closes the last closure packet at day 300.5 and the last damage packet at day 340.4. The difference is not free schedule. It is margin for empirical tails, forensic escalation and common-cause work.

## 11. Common-cause learning

The day-38 injection creates one observed conditional-consequence record:

| Shock record | Frequency information | Consequence information |
| --- | --- | --- |
| complete denial of one campus | none; the event was imposed | two closure and two damage events interrupted; 410 public personnel and one full service island unavailable |
| four outside originals | no shock-frequency information | whether records remain replayable without the campus |
| `CW-C010` remote packet | no shock-frequency information | whether physical completion survives loss of its originating evidence dependencies |
| residual schedule | no shock-frequency information | whether two campuses can compile and execute a bounded continuation |

The force may update recovery times, dependency graphs and conditional loss burden from the rehearsal. It may not infer a natural annual campus-loss probability from one scheduled injection. Natural shocks, if later observed, require a separate exposure denominator based on campus-time at risk.

A second campus denial during the two-campus residual campaign has zero protected tolerance. It automatically stops new credit-bearing starts. The first wave proves survival of one declared loss, not indefinite attrition.

## 12. Admission ladder

### 12.1 Method authorization

Planning authorizes the update method only when:

1. schema, priors, cutoff, cause classes and censor rules are frozen;
2. the exact predictive recurrence reproduces registered conformance values;
3. raw event and service records do not read back from results;
4. forced interventions contribute zero intrinsic trials and failures;
5. right-censored cycles contribute zero completed-cycle observations;
6. every residual reservation has one immutable token and station interval;
7. all daily, root, support and financial controls close; and
8. hostile conformance vectors fail in the expected state.

### 12.2 Live update authorization

A live update additionally requires:

- an authorized first-wave observation cutoff;
- complete native event and service-state records;
- independent cause classifications;
- resolved or explicitly held open packets;
- evidence that the implementation hash matches the preregistered estimator; and
- two independent reproductions of the posterior demand and residual schedule.

### 12.3 Force decision

Each lane receives one of four decisions:

| Decision | Rule |
| --- | --- |
| `PRESERVE` | base residual force stays at or below 70% utilization and all event-calendar gates pass |
| `AUGMENT` | base force breaches a limit, but one registered complete-chain increment closes every gate |
| `REDESIGN` | neither base force nor bounded augmentation closes demand, time, support or common-cause gates |
| `INDETERMINATE` | data identity, cause, censoring, completeness or implementation evidence is missing |

Integrated residual admission requires both lane decisions, root balance, common-cause closure, named rosters and constituted approval. A planning workbook can demonstrate the rule. It cannot supply these physical predecessors.

## 13. Financial constitution

### 13.1 Remaining operating support

Twenty-seven months remain after the first ninety-day wave. At USD 0.398B per year, standing support is:

`0.398 × 27 / 12 = USD 0.8955B`

This is a time-phased operating authorization, not new annual run rate or capital.

### 13.2 Bounded augmentation branch

If live damage evidence breaches the base capacity rule but one complete-chain cell closes the plan, the model opens a planning branch:

| Item | Planning reference |
| --- | ---: |
| one modular 120 m damage cell with dedicated utility, sanitary, metrology, evidence and reset interfaces | USD 0.480B capital |
| added annual support | USD 0.042B/year |
| twenty-seven-month added support | USD 0.0945B |
| base residual support plus augmentation | USD 1.470B |

The USD 0.480B reference is a clean-sheet complete-chain increment, not a bare concrete cell and not a vendor estimate. No capital is triggered by the synthetic conformance case.

### 13.3 Destroyed-campus exposure

Pass 104 allocated USD 4.020B to the nine campus-local asset groups: closure bays, damage cells, utility islands, laboratories, forensic lines, metrology, evidence/replay, blind shops and site separation. One-third is USD 1.340B.

| Capital boundary | USD B |
| --- | ---: |
| attributed one-campus local estate | 1.340 |
| reset stock and modular reserve, entire national estate | 0.250 |
| controlled program reserve, entire national estate | 0.210 |
| maximum visible reserve if both were wholly assignable | 0.460 |
| **unfunded physical-replacement exposure** | **0.880** |

Denial does not prove destruction, and this paper does not book USD 1.340B of damage. It proves that the prior 180-day complete-campus recommissioning statement is not yet matched by an explicit replacement-capital constitution. Before claiming physical regeneration, the program must distinguish recoverable denial, modular-lane replacement and complete estate loss; assign reserve by state; and demonstrate the industrial path that can rebuild the whole service island.

## 14. Technology program created by the update

The estimator creates physical technology requirements rather than an analytics office detached from the range.

### 14.1 Evidence-native causal state recorders

Every station, laboratory and custody node should emit signed state transitions that distinguish command, observed state, quality, uncertainty, authority and clock. The record must remain replayable without the campus control system.

### 14.2 Intervention-aware range compiler

The scheduler and estimator should share immutable event identities while retaining separate authority. The compiler must understand censoring, cause eligibility, support queues, root balance and protected reserve. It may calculate a schedule. It may not classify cause or grant credit.

### 14.3 Portable outside-original kits

Develop field-hardened evidence stores, clocks, witness interfaces and physical-package custody that leave the originating campus before the local dependency becomes decisive. `CW-C010` is the first minimal use case.

### 14.4 Modular complete-chain damage increments

A surge cell must include source, receiver, containment, injury system, sanitary laboratory interface, metrology, evidence, waste and reset. A structure without that chain adds hazard and apparent capacity without adding admissible decisions.

### 14.5 Autonomous state-accountable reset

Robotic cleaning, liner exchange, instrument replacement and geometry survey should write native custody and verification records as part of the action. Faster reset is useful only if it returns the cell to a registered known state.

### 14.6 Campus regeneration kits

The 180-day claim requires prequalified civil modules, utilities, controls, reference artifacts, trained teams and exerciseable industrial options. The kits must restore an entire truth-producing island, not only two station shells.

## 15. Failure modes

**Intervention contamination.** Counting the four imposed invalids as ordinary failures would update a frequency the rehearsal never observed.

**Short-cycle illusion.** Treating day-38 interruption as a completed three-day closure or one-day damage cycle would reward destruction with apparent productivity.

**Outcome-dependent exclusion.** Removing a record after its result is known changes the estimand and blocks admission.

**Article-to-range laundering.** Relabeling a technical failure as a range invalid buys another attempt and corrupts root evidence.

**Open-packet disappearance.** Advancing the cutoff while adverse packets remain open creates survivorship bias.

**Mean-only capacity.** Dividing total work by annual average capacity can conceal station overlap, WIP concentration and support queues.

**Reserve consumption.** Scheduling all four surviving damage cells would erase protection against an ordinary local outage.

**Synthetic-to-observed promotion.** A conformance vector proves formulas and gates. It cannot become campaign evidence through a label change.

**Denial-to-reconstruction leap.** Surviving without a campus for ninety days does not prove the physical estate can be rebuilt in 180 days.

**Unfunded regeneration.** A clock without reserved capital, industrial options and complete-chain modules is an aspiration.

## 16. What this pass establishes

### Established in planning

- the observation schema, cause taxonomy, censoring rule and cutoff law;
- separate intrinsic invalidity and forced-intervention consequence estimands;
- beta priors that preserve Pass 104 assumptions as assumptions;
- an exact beta-negative-binomial posterior predictive attempt distribution;
- one-sided small-sample cycle, packet and availability limits;
- a residual event compiler with station, WIP, root, reserve and deadline controls;
- preserve, augment, redesign and indeterminate decision states;
- a USD 0.8955B remaining support view and USD 1.470B bounded augmentation branch; and
- an explicit USD 0.880B unreserved complete-campus physical-replacement exposure.

### Demonstrated only by synthetic conformance data

- sixty-four closure and twenty-eight damage P90 residual reservations;
- 62.0-percent closure and 64.0-percent damage residual utilization;
- terminal closure packets by day 300.5 and damage packets by day 340.4;
- preservation of the six-bay/six-cell force for residual scheduling; and
- no trigger for the one-cell augmentation branch.

### Still physical and unearned

- every first-wave observation and cause classification;
- actual posterior predictive demand, cycle tail and productive availability;
- named residual rosters and station readiness;
- execution of the compiled residual schedule;
- recovery or reconstruction of `NRC-B`;
- root admission, production, form and rendering authority; and
- any claim that the 180-day destroyed-campus regeneration clock has passed.

### Next experiment

The next pass should define the **F36 campus-regeneration capital and industrial exercise constitution**. It must distinguish recoverable denial, modular-station loss and complete physical destruction; assign the USD 0.250B reset stock and USD 0.210B program reserve to explicit states; define the complete bill of regenerable campus services; establish unlike industrial build paths; and run a 180-day cold reconstruction exercise without borrowing the lost campus's workforce, technical data or utility island.

## 17. Model verification

The companion workbook contains sixteen sheets. Seventy-three terminal audits reproduce the observation counts, causal partition, posterior parameters, predictive attempt demand, time limits, availability bounds, seven service-capacity calculations, ninety-two residual reservations, 335 daily controls, three-root balance, financial branches and authority states. All seventy-three pass after export, and the saved-workbook formula-error scan is empty.

Eleven disposable perturbations test the decision surface. They reject an unauthorized forced-denial reclassification, an incomplete event record, a duration assigned to a right-censored event, an ordinary intrinsic invalid, reduced damage-cell productive time, an overlapping station interval, a root-count change and an altered annual-support basis. They also prove that live cutoff alone cannot admit the residual campaign, production and rendering flags cannot outrun residual admission, and a campus requalification flag cannot substitute for funded replacement. Every case changes or preserves the intended gate and is discarded after verification.

All sixteen sheets are rendered and visually reviewed. The final workbook is 105,220 bytes with SHA-256 `af52787f7d6d61a06fb999337afd50d64684418d02fa3aa372ea01c343521ed4`.

## Authority and limitations

This is a clean-sheet estimator and admission constitution under the project's full-authorization assumption. It uses only internal Pass 101–105 lineage and no external sites. All event and service observations in the companion model are explicitly synthetic conformance records. They demonstrate calculation and release behavior but contain no live campaign evidence.

The workbook owns the raw conformance tables, cause partition, posterior predictive recurrence, cycle and availability updates, residual capacity, event calendar, daily controls, root balance, common-cause states, financial branches and release logic. The paper owns their institutional meaning. Neither can authorize a live observation, roster, event, root, capital supplement, production form or rendering.

## Related work

- [F36 first campaign wave and complete-campus-loss rehearsal constitution](f36-first-campaign-wave-and-complete-campus-loss-rehearsal-constitution.md)
- [F36 range-complex throughput and regeneration architecture](f36-range-complex-throughput-and-regeneration-architecture.md)
- [F36 fixture commissioning and first-run data constitution](f36-fixture-commissioning-and-first-run-data-constitution.md)
- [F36 closure-kernel and full-bore damage-cell protocol](f36-closure-kernel-and-full-bore-damage-cell-protocol.md)
- [Workbook: F36 observed-throughput update and residual-campaign admission constitution](../../../models/force/generation/f36-observed-throughput-update-and-residual-campaign-admission-constitution.xlsx)
