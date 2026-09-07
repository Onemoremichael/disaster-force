# New York `L0` coherent target engine ceiling audit

**Registration:** `DF-NYC-L0-PR49-TARGETS-v1`

**Parents:** `DF-NYC-L0-PR44-INPUTS-v1`, `DF-NYC-L0-PR46-COMPILER-v1`, `DF-NYC-L0-PR48-DONORS-v1`

**Decision:** no target ensemble is admitted; donor fitting, synthesis, building assignment and architecture execution remain sealed

**Workbook SHA-256:** `133cebc151f3f7ea7cd6f67448cf47eab03ff6f8d94a38dcfa5336fa39a073e5`

## Finding

The first executable target engine does not pass its registered ceiling. It produces 36,000 nonnegative integer candidate target vectors—1,000 members for each of twelve catchments under three covariance cases—and every vector satisfies six equalities and twenty-seven inequalities. That mathematical closure is insufficient. At `K=1,000`, all three covariance cases exceed the registered `0.0050` selected-quantile stability limit, and thirteen candidate rows require more feasibility repair than the registered distance rule permits.

The failure is informative. Mean shares stabilize: the largest `K=1,000` to `K=500` change is between `0.00135` and `0.00180`, inside the `0.0025` limit. The lower and upper tails do not. Their worst changes range from `0.00774` to `0.00964`. The engine can therefore create plausible central populations while still moving the rare states that govern life safety, accessibility, staffing and neighborhood service demand. A Department of Resilience could not treat that as an adequate operating picture.

No ensemble is selected. Increasing the sample beyond the registered `K=1,000` ceiling, loosening the tail limit or choosing the case with the smallest miss would be a new method—not completion of this one.

## What was built

The engine begins with the 87-tract official input surface and the twelve outcome-blind catchments frozen by the preceding registrations. For eight ACS tables it reconstructs each catchment estimate and standard error directly from the published estimate plus eighty variance replicates. All 264 registered catchment–metric reconstructions match exactly within numerical tolerance. Sixteen metrics without published variance-replicate coverage retain the disclosed root-sum-square margin approximation from the input registration; their missing cross-table covariance is not silently treated as known.

One deterministic, exactly nested Latin-hypercube design supplies the first `125`, `250`, `500` and `1,000` members. Every registered prefix occupies every marginal stratum exactly. This is important because ordinary prefixes of a low-discrepancy design do not automatically preserve balance at these non-power-of-two sample sizes.

Three structural covariance cases expose what the public data do not identify:

| Case | Retained dependence | Purpose |
| --- | --- | --- |
| `T0_TABLE_BLOCK` | published variance-replicate covariance within each available table and geography | minimum declared cross-table structure |
| `T1_SHARED_CATCHMENT` | moderate metropolitan and catchment common movement | dependence sensitivity |
| `T2_CONCORDANT_DOMAIN` | stronger metropolitan, catchment and domain common movement | concordant-tail sensitivity |

These are not estimated probabilities and cannot be selected after observing an attractive force result. They are bounded structural cases for a missing-covariance problem.

Each case–member–catchment vector is projected once through a nonnegative integer weighted-`L1` mixed-integer program. The program enforces the population, household, occupancy, tenure, structure and disability identities registered in the compiler, plus monotonic and subset relations. Ten deliberate contradictions test the stop logic. All ten are rejected.

## Ceiling result

| Case | Maximum mean-share change | Maximum selected-quantile change | Rejected rows | Gate |
| --- | ---: | ---: | ---: | --- |
| `T0_TABLE_BLOCK` | `0.001797` | `0.008906` | 8 | not met |
| `T1_SHARED_CATCHMENT` | `0.001494` | `0.009638` | 4 | not met |
| `T2_CONCORDANT_DOMAIN` | `0.001352` | `0.007738` | 1 | not met |

The largest `T0` tail movement is the fifth percentile of population in `NYC-V2-R01`, shifting from `0.955464` to `0.964370` of the registered point estimate as `K` doubles. `T1` is worst on the fifth percentile of housing units in the same catchment. `T2` is worst on the fifth percentile of no-vehicle households there. This concentration does not authorize local tuning; it identifies a useful falsification site for the next method.

Across all 36,000 candidates there are no negative cells, no noninteger cells and no hard-constraint violations. Thirteen rows are nevertheless rejected because the joint projection moves one or more margins too far from their sampled value. Under `T0`, the maximum standardized repair reaches `6.478`; under `T1`, `5.318`; under `T2`, `5.139`. The screen-precision threshold is five standard errors.

## Diagnosis

The failed engine samples several published totals as if they were separate primitive coordinates and asks the feasibility projection to repair the relationships afterward. Some of those totals are definitional cousins rather than independent quantities: population and civilian noninstitutionalized population; households and occupied units; occupied and vacant units; owner and renter occupancy; structure classes and occupied housing. Within-table variance replicas preserve important covariance, but the public surface does not publish every cross-table relation needed to draw those totals jointly.

Conditioning tenure and structure partitions on occupied housing reduced obvious contradictions. It did not solve the deeper parameterization problem. The projection remains one-sided near boundaries and can alter rare-tail behavior even when central means look stable. In effect, the solver is being asked to invent a coherent population after the random draw rather than the generator drawing a coherent population by construction.

The appropriate successor is a structural-coordinate generator. It should draw primitive totals and simplex shares or complements—household population, group quarters, institutional complement, occupancy and vacancy, tenure shares, structure shares and disability subpartitions—and derive dependent counts before integer projection. Published margins and variance replicates remain calibration targets. The projection should become a small rounding and reconciliation step, not the mechanism that creates coherence.

## Institutional consequence

This is not merely a campaign implementation issue. A mature Department of Resilience would need an independent target authority able to produce uncertainty-aware civil operating pictures under damaged communications, reconcile protected local records with official statistics and field observations, and refuse downstream optimization when tail behavior is unstable. The authority would need statisticians, privacy engineers, survey methodologists, operations researchers, building-system specialists and field operators under one safety case.

That capability is as fundamental as logistics. Force design depends on who needs water, cooling, medical power, accessible movement and household continuity—not only on total population. A model that preserves the mean while shifting the fifth percentile can mis-size precisely the scarce formations that determine whether the public guarantee is met.

## Boundaries

This pass does not create a synthetic population. It does not fit PUMS donors, integerize donor classes, infer protected relational records, assign households to public building classes, estimate building operability, evaluate `A2` or `S3`, or fill any registered architecture outcome. The 36,000 vectors are diagnostic candidates, not an accepted uncertainty ensemble.

The companion [workbook](../../../../models/proving/campaigns/new-york/nyc-l0-target-engine-ceiling-audit.xlsx) contains the registrations, sources, reconstruction checks, metric definitions, covariance cases, constraints, convergence results, projection summaries, rejected rows, distribution diagnostics, failure injections, integrity controls, and a 1,000-member focal diagnostic for each case. The full case arrays are cryptographically committed in the workbook.

The [structural-coordinate successor](l0-structural-target-engine.md) changes coordinates before changing the ceiling. It eliminates excessive projection repair and produces 36,000 coherent integer states, but still admits no case: all three miss tail stability and published-margin calibration. The subsequent [moment-reconciliation engine](l0-moment-reconciliation-engine.md) preserves official covariance and all additive identities, proving linear feasibility while failing nonlinear civil-state, center and tail gates. The next method must generate nonnegative latent atomic cells. Donor fitting remains downstream.
