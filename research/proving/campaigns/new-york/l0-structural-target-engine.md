# New York `L0` structural target engine

**Registration:** `DF-NYC-L0-PR50-STRUCTURAL-TARGETS-v2`

**Parents:** `DF-NYC-L0-PR44-INPUTS-v1`, `DF-NYC-L0-PR46-COMPILER-v1`, `DF-NYC-L0-PR48-DONORS-v1`, `DF-NYC-L0-PR49-TARGETS-v1`

**Decision:** no target ensemble is admitted; donor fitting, synthesis, building assignment and architecture execution remain sealed

**Workbook SHA-256:** `023a99e009fe2b2fa36b01287f7053890f25582bcf4c8afa87ea4c56a1dfc851`

## Executive finding

Structural coordinates solve the wrong-kind-of-coherence defect in the first target engine, but they do not yet solve the statistical problem.

The engine generates population, age, disability, household, occupancy, tenure and building-form relationships as identities before integer projection. Across 36,000 case–member–catchment targets, every cell is a nonnegative integer, every row satisfies six equalities and twenty-seven inequalities, no row crosses a projection-distance stop, and median mean repair is about `0.0015` input standard errors. The projection is now doing what it should do: rounding and residual reconciliation, not inventing a coherent population.

No covariance case is nevertheless admissible. All three miss the registered `0.0050` selected-tail convergence limit at `K=1,000`, and all three fail a published-margin calibration gate fixed before the ceiling run. The largest defect is housing-unit uncertainty: its ensemble standard deviation reaches `1.73–1.81` times the published standard error. A single directed hierarchy is accumulating uncertainty from upstream population, group-quarters, household-size and vacancy coordinates when independently published tables are forced to agree.

More samples will not cure that distortion. The next engine must reconcile moments across an ensemble or estimate a defensible latent atomic-cell system; it cannot merely choose a different upstream table or relax the gate.

## Why the coordinate system changed

The superseded `v1` engine drew many published margins separately and then used a mixed-integer program to impose civil identities. That produced feasible integers, but thirteen rows required excessive repair and tail behavior remained unstable. The optimizer was partly creating coherence after the draw.

`v2` instead draws a smaller structural grammar:

| Coordinate | Construction | Governing implication |
| --- | --- | --- |
| population | positive total | no negative population state |
| age | closed under-18 / 18–64 / 65+ composition with nested 75+ and 85+ shares | age exhaustion and nesting hold by construction |
| civilian status | bounded institutional/armed-forces complement | civilian noninstitutionalized population cannot exceed population |
| disability | age-specific bounded rates with an exact total | disability classes sum to any disability and remain within age populations |
| functional difficulty | bounded shares of any disability | each difficulty remains a subset without forcing mutual exclusivity |
| group quarters | bounded population share | household population is the complement |
| household size and type | household population divided by a feasible average size; closed family/nonfamily split | household-person minimum holds |
| household subsets | bounded shares of their governing household or person total | children, older-adult, living-alone and service-demand subsets remain legal |
| occupancy | vacancy share applied to occupied households | households equal occupied units; occupied plus vacant equals housing units |
| tenure | two-part occupied-unit composition | owner plus renter equals occupied |
| structure | six nonnegative component draws closed to occupied units | structure classes exhaust occupied units |

This is a first-principles modeling change. The metric vector is no longer treated as thirty-eight interchangeable Gaussian totals. It is understood as a civil state with totals, complements, nested populations, overlapping need indicators and exhaustive partitions.

## Registered design

The official input surface and twelve outcome-blind catchments remain unchanged. For eight ACS tables, the engine reconstructs every estimate and standard error from the published estimate and eighty variance replicates; all 264 catchment–metric reconstructions agree within numerical tolerance. Sixteen margins without variance-replicate coverage retain the disclosed approximation in the parent input registration.

One deterministic nested Latin-hypercube design supplies prefixes of `125`, `250`, `500` and `1,000` members across 849 latent dimensions. Each registered prefix is exactly stratified. The same three missing-covariance cases remain co-governing:

| Case | Cross-table structure | Interpretive role |
| --- | --- | --- |
| `T0_TABLE_BLOCK` | preserves published covariance within available ACS table blocks | minimum declared structure |
| `T1_SHARED_CATCHMENT` | adds moderate metropolitan and catchment common movement | shared-place sensitivity |
| `T2_CONCORDANT_DOMAIN` | adds stronger metropolitan, catchment and domain movement | concordant-tail stress |

These are structural sensitivities, not occurrence probabilities. No case can be selected because it yields a preferred force result.

For each real-valued structural state, one weighted-`L1` mixed-integer program performs nonnegative integer closure. Four gates then co-govern target admission:

1. **row integrity:** every target must be a nonnegative integer and satisfy all hard constraints;
2. **projection distance:** mean repair must not exceed `0.50` input standard errors, no screen-precision margin may exceed `5`, and no margin may exceed `8`;
3. **nested stability:** from `K/2` to `K`, the maximum mean-share change must not exceed `0.0025`, the maximum selected-quantile change must not exceed `0.0050`, and no row may be rejected;
4. **marginal calibration:** every ensemble mean must remain within `0.50` input standard errors of its published estimate, and every interior margin must retain a standard-deviation ratio between `0.75` and `1.25`.

A margin is treated as boundary-limited when its point estimate is less than two input standard errors above zero. Such a nonnegative ensemble cannot reproduce a symmetric input standard error; its center remains governed, while its spread is disclosed and exempt from the ratio gate. This prevents zero and rare cells from being granted an impossible symmetric target or silently removed from review.

## Ceiling result

| Case | Mean-share change | Selected-quantile change | Center failures | Spread failures | Worst spread ratio | Admission |
| --- | ---: | ---: | ---: | ---: | ---: | --- |
| `T0_TABLE_BLOCK` | `0.000592` | `0.006324` | 2 | 16 | `1.805` | not met |
| `T1_SHARED_CATCHMENT` | `0.000521` | `0.005427` | 0 | 13 | `1.798` | not met |
| `T2_CONCORDANT_DOMAIN` | `0.000534` | `0.007567` | 0 | 43 | `1.733` | not met |

All three mean-share changes are comfortably within the registered limit. All three selected-tail changes are not. The miss is relatively small in `T1`, but the threshold is a design commitment, not a ranking device.

The calibration result is more consequential than the convergence miss. `T0` has two center failures, both in households with a person age 65 or older; its worst absolute mean bias is about `0.575` input standard errors. The shared-factor cases pull the worst center error inside the gate, but they do not repair spread. `T2` causes forty-three interior spread failures, showing that stronger common movement can preserve legal civil states while badly changing marginal uncertainty.

Housing units are the worst spread failure in every case, centered on `NYC-V1-R03`. This is not an integer-projection artifact. The largest single-cell repair anywhere in the 36,000-row surface remains below `0.272` input standard errors, and no target is rejected. The distortion arises upstream in the structural hierarchy.

## What the negative result means

The hard identity `households = occupied housing units` joins estimates originating in different ACS table systems. In the present hierarchy, households are generated from population minus group quarters and a household-size coordinate. Housing units are then derived by applying a vacancy share. Each upstream coordinate carries uncertainty. When their perturbations are combined, the derived housing total can become much more variable than the separately published housing-unit estimate.

Reversing the direction would move rather than solve the problem: generating households from housing units and occupancy would distort household and population-linked uncertainty instead. Selecting one table as authoritative for every joint relationship would be an undocumented statistical preference with operational consequences.

The deeper issue is that exact sample identities, separately published estimates and separately published standard errors do not automatically define a feasible joint probability law. Public variance replicates identify important covariance inside tables, but not every cross-table covariance required by this civil-state grammar. A coherent row generator can therefore be locally correct and globally miscalibrated.

The appropriate successor is an ensemble-level reconciliation engine. Two candidate approaches merit a registered comparison:

- a constrained moment-reconciliation procedure that adjusts latent dependence and atomic components so all interior published means and variances are matched jointly while preserving every row identity; and
- a latent atomic-cell model whose aggregations generate the published margins, with covariance learned only where official replicates or governed microdata provide authority and otherwise bounded by declared sensitivity sets.

Both approaches need impossibility diagnostics. If the published centers, variances and hard identities cannot coexist inside the registered tolerance, the engine must produce a certificate or minimum-conflict surface—not hide the conflict through a preferred hierarchy.

## Department-level consequence

A mature Department of Resilience needs a standing civil-state production capability comparable in seriousness to military intelligence preparation, logistics estimation and operational test. It must convert protected local records, official statistics, building-system evidence and field observations into uncertainty-aware operating pictures while preserving rights and refusing false precision.

This pass identifies part of that institution’s technical mandate:

- maintain semantic authority for totals, nested groups, overlaps and exhaustive partitions;
- estimate or bound cross-system dependence rather than assume it away;
- publish calibration, convergence, impossibility and privacy evidence alongside every operational population state;
- separate lawful protected relational data from public aggregate releases;
- preserve an explicit stop between civil-state estimation and force optimization; and
- sustain independent red-team and reproduction capacity able to block deployment of a convenient but invalid operating picture.

This is not back-office analytics. Water, cooling, medical power, accessible movement, household contact and reception capacity are sized from these states. A statistically distorted tail becomes a mis-sized formation.

## Boundary and next move

This pass produces no donor weights, synthetic households, persons or group quarters; no building assignment; no operational building state; and no `A2` or `S3` outcome. Candidate targets are diagnostic, not an accepted population ensemble.

The companion [workbook](../../../../models/proving/campaigns/new-york/nyc-l0-structural-target-engine.xlsx) contains the registration, sources, coordinate register, covariance cases, hard constraints, nested convergence results, calibration surface, projection summary, deliberate structural injections, target-integrity audit, full cryptographic commitments and a 1,000-member focal diagnostic from every case.

The next admissible pass is not donor fitting. It is a registered structural target engine `v3` that treats cross-table moment reconciliation as the central problem, compares at least the two candidate approaches above, and reruns all four gates without loosening them after observation. Architecture access remains prohibited.
