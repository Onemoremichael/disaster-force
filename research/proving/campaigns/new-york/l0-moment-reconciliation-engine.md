# New York `L0` moment-reconciliation engine

**Registration:** `DF-NYC-L0-PR51-MOMENT-RECONCILIATION-v3A`

**Parents:** `DF-NYC-L0-PR44-INPUTS-v1`, `DF-NYC-L0-PR46-COMPILER-v1`, `DF-NYC-L0-PR48-DONORS-v1`, `DF-NYC-L0-PR50-STRUCTURAL-TARGETS-v2`

**Decision:** linear moment reconciliation succeeds; no target ensemble is admitted because nonlinear feasibility repair creates center bias, candidate rejection and unstable tails

**Workbook SHA-256:** `46a203402135428721bf6352fa5f794fd14114165f24e7bd489dc7ef4dba7320`

## Executive finding

The published linear moments are not the contradiction. The geometry of a valid civil population is.

This engine constructs three covariance completions that preserve every official ACS variance-replicate covariance block, retain every published or registered marginal standard error and satisfy all six exact additive identities. Each reconciliation reaches a relative identity residual below `1 × 10^-10`; the largest relative change to any official covariance Gram matrix is below `2.5 × 10^-15`. The spread failures that defeated the structural target engine disappear: all `1,302` governed interior margin–case combinations remain within the registered `0.75–1.25` standard-deviation ratio.

No completion is nevertheless admissible. A multivariate Gaussian with the correct means, variances and linear identities does not respect nonnegativity or nonlinear subset relations. Depending on completion, `5,248–5,293` of `12,000` raw catchment states contain a negative cell and `5,902–5,993` violate at least one civil subset inequality. Integer projection repairs every final row, but a one-sided repair cannot be distribution-neutral. It shifts population centers upward, rejects two extreme rows and leaves selected tails unstable at the registered `K=1,000` ceiling. Center failures fall from eight to one across the three completion starts, but the least-failing start cannot be selected after observation.

The result separates two questions that earlier engines conflated:

1. **linear moment feasibility:** can published means, standard errors, official covariance blocks and exact additive identities coexist? Yes;
2. **civil-state feasibility:** can a distribution with those moments remain on the nonnegative, nested and capacity-bounded state space without distorting its moments? Not under this Gaussian-plus-projection construction.

The next engine must therefore begin with latent nonnegative atomic cells and generate aggregates from them. Another hierarchy, covariance start or projection rule would only move the boundary distortion.

## The question this pass answers

The structural `v2` engine generated legal rows with negligible numerical repair, but it forced separately published margins through one directed hierarchy. That caused housing-unit dispersion as high as `1.81` times the published standard error. Two explanations remained possible:

- the published marginal variances and the exact identities were mutually incompatible; or
- the chosen hierarchy imposed the wrong unidentified cross-table dependence.

Pass 51 isolates those possibilities. It asks whether a covariance matrix can be constructed that simultaneously:

- preserves the complete official covariance within every available variance-replicate table;
- preserves the registered standard error of every RSS-only margin;
- preserves all published point estimates;
- satisfies every exact additive identity in every stochastic realization; and
- leaves unidentified cross-table covariance explicitly unresolved rather than silently declaring it zero or estimated.

This is a ceiling test, not a preferred operational model. Success would prove that the linear constraints can coexist. It would not prove that the resulting stochastic states are possible households, people or buildings.

## Covariance authority

The metric vector contains `38` quantities for each of `12` catchments. Eight ACS tables provide eighty variance replicates. For those tables, the replicate system determines not merely marginal standard errors but complete within-table covariance across all constituent geographies and catchments. That covariance is treated as official statistical authority and is not tunable.

Other margins have registered RSS uncertainty but no cross-metric covariance authority. Their standard-error norms are preserved, while their directions in latent-factor space remain unidentified. Cross-table covariance is also unidentified. The model does not collapse “unidentified” into “zero.” It carries three starting structures to expose path dependence:

| Completion | Starting condition | Interpretive role |
| --- | --- | --- |
| `R0_ZERO_START` | zero unidentified cross-table loading | minimum-structure start, not a claim of independence |
| `R1_SHARED_START` | moderate shared metropolitan and catchment loading | common-place sensitivity |
| `R2_CONCORDANT_START` | stronger domain-concordant loading | correlated-boundary sensitivity |

These are covariance completions, not probabilities and not rival forecasts. The final official covariance blocks are identical in all three cases. Only the unidentified portion is permitted to differ.

## Reconciliation method

Let the centered metric state be represented by a factor loading matrix `B`:

```text
x = μ + Bz,       E[z] = 0,       Cov(z) = I
Σ = BBᵀ
```

Let `A` encode the six exact additive identities. Exact satisfaction in every linear realization requires both:

```text
Aμ = 0
AB = 0
```

The published point estimates already satisfy `Aμ = 0` within the registered numerical tolerance. The problem is to place the loading rows in the nullspace of `A` while preserving the authoritative Gram matrices `B_g B_gᵀ` for every official variance-replicate block `g` and the row norms of the RSS-only margins.

The engine alternates two factor-space projections:

1. **identity projection:** project each catchment loading block into the nullspace of `A`, forcing every stochastic perturbation to respect all six exact identities;
2. **authority restoration:** for every official table block, apply a fixed-Gram polar projection that restores its complete covariance matrix; for every RSS-only margin, restore its prescribed row norm.

Iteration stops when the maximum relative identity residual is at most `1 × 10^-10`. The procedure does not estimate a uniquely true joint covariance. It finds a point in the intersection of the linear-identity manifold and the statistical-authority manifolds, conditional on a disclosed start. Differences among converged cases measure unresolved completion dependence.

The three cases each converge in `56` iterations:

| Completion | Identity residual | VRE Gram relative error | RSS norm error | Maximum official-correlation change | Gate |
| --- | ---: | ---: | ---: | ---: | --- |
| `R0_ZERO_START` | `9.49 × 10^-11` | `2.40 × 10^-15` | `4.44 × 10^-16` | `3.33 × 10^-15` | met |
| `R1_SHARED_START` | `7.95 × 10^-11` | `2.25 × 10^-15` | `4.44 × 10^-16` | `4.22 × 10^-15` | met |
| `R2_CONCORDANT_START` | `7.60 × 10^-11` | `2.45 × 10^-15` | `4.44 × 10^-16` | `3.55 × 10^-15` | met |

Small negative covariance eigenvalues, with magnitude below `1.1 × 10^-9`, are numerical roundoff relative to the scale of the matrices. The factor representation itself remains positive semidefinite by construction.

The converged completions remain materially different where evidence is absent. Pairwise correlation RMS differences range from `0.0357` to `0.0813`; the largest individual difference is `0.8467`. This is a finding, not a defect to average away. Official data constrain important blocks but do not identify the full civil joint distribution.

## Registered sampling and admission rules

Each completion uses the same deterministic, exactly nested Latin-hypercube design as the prior engines: `1,000` members with exactly stratified prefixes at `K=125`, `250`, `500` and `1,000`. Across three completions and twelve catchments, the ceiling therefore contains `36,000` candidate rows.

The same integer weighted-`L1` mixed-integer program enforces nonnegativity, six equalities and twenty-seven inequalities. It remains a diagnostic repair layer. A row is rejected if the solver fails, its mean standardized movement exceeds `0.50`, a screen-precision cell moves more than five input standard errors, or any cell moves more than eight.

Four gates remain co-governing:

1. covariance reconciliation must preserve statistical authority and exact linear identities;
2. final target rows must be nonnegative integers satisfying all hard constraints;
3. nested mean and selected-tail summaries must stabilize within `0.0025` and `0.0050`, with no rejected row; and
4. ensemble centers must lie within `0.50` input standard errors and interior spreads within `0.75–1.25` input standard errors.

The gates are evaluated jointly. Passing reconciliation and spread calibration cannot compensate for failed center, tail or row-rejection controls.

## Ceiling result

| Completion | Mean-share change | Selected-quantile change | Rejected rows | Center failures | Spread failures | Admission |
| --- | ---: | ---: | ---: | ---: | ---: | --- |
| `R0_ZERO_START` | `0.001706` | `0.006348` | 1 | 8 | 0 | not met |
| `R1_SHARED_START` | `0.001608` | `0.007619` | 1 | 5 | 0 | not met |
| `R2_CONCORDANT_START` | `0.001630` | `0.009174` | 0 | 1 | 0 | not met |

All three mean summaries meet the `0.0025` limit. Every selected-tail summary misses the `0.0050` limit. `R0` and `R1` each include one row rejected by the pre-registered screen-precision rule. `R2` avoids row rejection but has the largest tail movement. No completion dominates all gates.

The removal of every spread failure is the central positive result. The worst interior standard-deviation ratio is now `0.838`, `0.870` and `0.885` respectively—well inside the registered band. This proves that exact identities do not require the `1.73–1.81` housing-unit inflation observed in `v2`.

The remaining center failures are concentrated in total population for `NYC-V2-R01`. Worst absolute mean bias declines from `0.592` to `0.553` and `0.520` input standard errors as the start becomes more concordant. The last value is close to the gate, but proximity is not admission and the direction was observed only after the cases were run.

## Why nonlinear feasibility changes the answer

The reconciled Gaussian states satisfy the additive identities before integer projection to numerical precision. They do not satisfy the full civil state space.

| Completion | Raw rows | Rows with a negative cell | Negative cells | Rows with a subset violation | Largest subset violation |
| --- | ---: | ---: | ---: | ---: | ---: |
| `R0_ZERO_START` | 12,000 | 5,250 | 5,617 | 5,993 | 9,472.16 |
| `R1_SHARED_START` | 12,000 | 5,248 | 5,601 | 5,947 | 8,764.47 |
| `R2_CONCORDANT_START` | 12,000 | 5,293 | 5,637 | 5,902 | 6,771.42 |

A Gaussian perturbation has unbounded support. Rare margins can cross zero; a subset can exceed its parent even when both means and covariances are individually plausible. The feasible civil-state region is instead a bounded polytope with sharp faces: counts cannot be negative, nested groups cannot exceed parents, households require people, and tenure or structure components must close to occupied units.

Projection maps every infeasible raw state back onto this region. Near a boundary the map is one-sided: negative values can move upward but corresponding positive values are not symmetrically moved downward. The output mean therefore changes even if the raw design is centered exactly. This is why population-center bias appears after the linear moment problem has been solved.

Projection movement is no longer negligible. Median mean standardized shift is `0.0184`, `0.0175` and `0.0167` across the cases—more than ten times the `v2` median—and the maximum individual screen-precision movement reaches `5.53`, `5.15` and `4.93` input standard errors. All final rows are legal integers, but legality obtained through asymmetric repair is not distributional validity.

## What is learned—and what is not

This pass establishes four results.

First, the official table covariances, registered marginal standard errors and exact additive identities have a common linear completion. The `v2` spread defect was methodological, not an unavoidable conflict in the published statistics.

Second, that completion is not unique. Unidentified cross-table dependence remains consequential even after all authoritative covariance is held fixed. Operational planning must preserve sensitivity across that uncertainty rather than select whichever completion makes the force look best.

Third, matching linear moments is insufficient for a civil-state generator. The generator must live on the feasible state space before aggregation; projection cannot be asked to transform an unbounded distribution into lawful households and retain all of its moments.

Fourth, sample convergence remains a separate claim. Even the completion with only one center failure misses the registered tail ceiling. More samples might characterize its limiting distribution more precisely, but they would not justify the distributional form or remove one-sided boundary effects.

This pass does **not** establish a household distribution, tract truth, building occupancy, incident operability, medical-power demand, caregiver relations or architecture performance. It fits no donor, produces no public relational record and opens no downstream campaign table.

## Successor: latent atomic-cell authority

The next target engine should generate a set of nonnegative latent atomic cells whose sums define all published margins. Instead of drawing aggregate totals and repairing contradictions, it should draw only feasible atoms and calculate totals, complements, nests and partitions as deterministic aggregations.

A credible `v3B` comparison should include:

- nonnegative latent variables for mutually exclusive atomic states, with explicit separate treatment of overlapping functional-need indicators;
- exact aggregation matrices connecting atoms to every published margin;
- calibration of aggregate centers and covariances against official VRE authority;
- bounded sensitivity sets for unidentified cross-table dependence;
- a likelihood, generalized method-of-moments or constrained optimal-transport objective that reports the minimum conflict rather than hiding it;
- structural-zero and rare-cell treatment that cannot manufacture unsupported combinations;
- deterministic nested sampling and the unchanged convergence, calibration, projection and rejection gates;
- donor-support labels and privacy review only after the aggregate ensemble is admitted; and
- an explicit impossibility surface if no atomic distribution can reproduce the registered moments.

The atomic model should be tested against the reconciled Gaussian result, not assumed superior. It must demonstrate that it reduces one-sided repair while retaining official covariance and without concentrating mass in implausible boundary cells.

## Department-level consequence

This technical failure changes the institutional design. A Department of Resilience cannot treat civil-state estimation as ordinary analytics purchased after an event. It needs a permanent **Civil State Authority** with powers and restraints analogous to a safety-critical mission-data enterprise.

That authority would maintain common statistical semantics, aggregation graphs, protected local interfaces, covariance provenance, uncertainty completions, feasibility geometry, privacy controls and independent reproduction. It would certify operating pictures for specific public-service purposes, not assemble a generalized population-surveillance system. It would also publish stop decisions when the available evidence cannot support a lawful, calibrated joint state.

The capability is strategic because formation size follows from the tails of these states. Cooling, water, medical power, vertical access, household contact, accessible transport and receiving capacity are all mis-sized if the underlying joint population is coherent only after asymmetric repair. A force capable of projecting physical service at continental scale also needs the statistical-industrial machinery to know what service is required without inventing vulnerable people or erasing rare ones.

## Boundary and next move

No target ensemble is admitted. Donor fitting, integer donor-class selection, synthetic households and persons, group-quarters synthesis, public building-class assignment, operational building state, `A2`/`S3` execution and campaign aggregation remain at zero.

The companion [workbook](../../../../models/proving/campaigns/new-york/nyc-l0-moment-reconciliation-engine.xlsx) contains the complete registration, source lineage, method register, covariance starts, constraints, reconciliation history, official-covariance checks, path-dependence diagnostics, preprojection boundary audit, convergence and calibration surfaces, integrity controls, deliberate contradictions, `3,000` focal candidate rows and cryptographic commitments to all `36,000` candidate targets.

The next admissible pass is `v3B`: a registered latent atomic-cell generator tested against the same ceiling. The Gaussian reconciler remains a useful linear benchmark and an impossibility diagnostic, but it is rejected as the target authority. Architecture access and renderings remain prohibited.
