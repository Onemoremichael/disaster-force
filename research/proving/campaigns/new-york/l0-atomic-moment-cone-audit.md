# New York `L0` atomic moment-cone audit

**Registration:** `DF-NYC-L0-PR53-ATOMIC-MOMENT-CONE-v3B1A`

**Decision:** exact cloning of published point estimates and estimator covariance as moments of a nonnegative civil-state distribution is rejected. The official covariance remains authoritative, but it belongs in a measurement likelihood rather than in the covariance of true states.

**Paired model:** [New York `L0` atomic moment-cone audit](../../../../models/proving/campaigns/new-york/nyc-l0-atomic-moment-cone-audit.xlsx)

**Successor:** Pass 54 has now frozen the [`v3C0` atomic posterior preregistration](l0-atomic-posterior-preregistration.md). The specification below is retained as the requirement lineage; the later registration is current authority.

## Executive judgment

Pass 52 registered a lawful atomic support and proved that all 456 published point margins could be reconstructed by nonnegative integer states. It then proposed a natural successor: calibrate a distribution over those states whose aggregate mean and covariance exactly equal the published ACS point estimates and variance-replicate covariance.

Pass 53 proves that proposal is not merely difficult. It is impossible for the registered data.

Seven catchment margins report zero occupied mobile-home-or-other units and positive sampling standard errors. If a true state count `X` is nonnegative and `E[X] = 0`, then `X = 0` with probability one and `Var[X] = 0`. No probability distribution over lawful nonnegative civil states can therefore have both the required zero mean and positive variance. These seven one-dimensional contradictions are sufficient to place the requested aggregate moment vector outside the nonnegative moment cone. Higher-dimensional calibration cannot repair them.

The failure reveals a deeper category error. An ACS variance-replicate covariance matrix describes how an **estimator** would vary under repeated samples. It is not automatically the covariance of uncertainty over the unknown true population after the estimates have been observed. Pass 51 preserved the estimator covariance but used it as a cross-world state generator. Pass 52 fixed the state support but retained exact moment cloning as the intended calibration target. Pass 53 separates the two objects.

The correct successor is a measurement-error construction:

```text
p(x | ŷ) ∝ p(ŷ | A x, V) p₀(x),    x ∈ nonnegative integer atomic support,
```

where `ŷ` is the published estimator, `V` is its registered sampling-error covariance, `A x` is the aggregate implied by one lawful civil state, and `p₀(x)` is a disclosed sensitivity prior or regularizer over unidentified atomic relationships. This does not make the prior true. It makes the source of uncertainty explicit and testable.

No target ensemble, donor fit, synthetic population, building assignment or architecture outcome is admitted in this pass.

## 1. The question that changed

The initial stochastic objective treated the published points and covariance as a complete description of the desired target ensemble:

```text
E[A x] = ŷ
Cov[A x] = V.
```

That objective appeared conservative because it preserved official statistical uncertainty. It was also attractive computationally: Pass 51 demonstrated three linear completions that exactly retained the official within-table covariance blocks, all registered marginal standard errors and six additive identities.

But the objective silently identified two different probability spaces:

1. the repeated-sampling distribution of the published estimator; and
2. the epistemic distribution over possible true civil states after observing that estimator.

Those probability spaces need not share a mean, covariance, support or boundary behavior. The distinction becomes unavoidable when an estimate lies on the boundary of the state space.

Pass 53 therefore asks a more basic question before any ensemble is generated:

> Can the requested first and second moments belong to any probability distribution over the registered nonnegative aggregate support?

The answer is no.

## 2. The nonnegative moment-cone theorem

### 2.1 One-dimensional boundary result

Let `X` be a nonnegative random variable. If `E[X] = 0`, then:

```text
P(X > 0) = 0,
```

because any positive probability mass above zero would contribute a positive amount to the expectation. Therefore `X = 0` almost surely and:

```text
Var[X] = E[(X - E[X])²] = 0.
```

Consequently, the moment pair

```text
(E[X], Var[X]) = (0, σ²),    σ² > 0
```

does not belong to the moment cone of distributions supported on the nonnegative real line or the nonnegative integers.

### 2.2 Application to the registered targets

Seven of the 468 catchment–metric pairs require exactly that impossible pair.

| Catchment | Published point | Sampling SE | Requested state variance |
| --- | ---: | ---: | ---: |
| `NYC-V1-R02` | 0 | 46.201 | 2,134.496 |
| `NYC-V1-R03` | 0 | 46.694 | 2,180.320 |
| `NYC-V1-R04` | 0 | 54.386 | 2,957.844 |
| `NYC-V2-R03` | 0 | 56.046 | 3,141.139 |
| `NYC-V2-R04` | 0 | 55.636 | 3,095.315 |
| `NYC-V3-R02` | 0 | 52.533 | 2,759.768 |
| `NYC-V3-R04` | 0 | 56.987 | 3,247.568 |

Every conflict concerns occupied mobile-home-or-other units. The substantive category is less important than the proof. A single impossible marginal invalidates the complete exact-moment system, regardless of the covariance completion, optimizer or sampler.

### 2.3 Why projection cannot solve the problem

A Gaussian draw can carry positive variance around zero only by placing mass below zero. Truncation or projection removes that negative mass, but it necessarily changes the mean, variance or both. Restoring the original moments would reintroduce inadmissible support. The conflict is mathematical, not an implementation defect.

Pass 51 observed the practical signature of this geometry: boundary repair shifted centers, rejected extreme rows and destabilized selected tails. Pass 53 supplies the proof those symptoms were expressing.

## 3. Estimator uncertainty is not state variation

The registered statistical objects now have separate meanings.

| Object | Symbol | Meaning | Governing authority |
| --- | --- | --- | --- |
| published estimate | `ŷ` | observed estimator for an unknown finite-population margin | official point estimate |
| estimator covariance | `V` | repeated-sample uncertainty of `ŷ` | official variance replicates or registered approximation |
| atomic civil state | `x` | nonnegative counts of lawful person and household-unit cells | semantic support plus later evidence |
| aggregate true state | `A x` | margins implied by one lawful atomic state | fixed aggregation operator |
| likelihood | `p(ŷ | A x, V)` | how observed estimators inform feasible states | registered measurement model |
| prior or regularizer | `p₀(x)` | disclosed treatment of unidentified dependence | sensitivity case pending evidence |
| posterior ensemble | `p(x | ŷ)` | support-feasible uncertainty after evidence and assumptions | future `v3C0` only |

The official covariance loses no authority in this change. Its role becomes more precise. It governs the relationship between a hypothetical true aggregate state and the estimator that was observed. It no longer dictates an ontic population of parallel New Yorks whose covariance must reproduce estimator sampling error.

This distinction also prevents a second mistake. The published point estimate need not be forced to equal the posterior mean at a nonnegative boundary. A zero estimate with positive sampling error can be compatible with positive true counts under a measurement model. The posterior treatment then depends on the likelihood, prior, structural support and nearby evidence, all of which must be disclosed.

## 4. Authoritative under-five extension

Pass 52 identified a specific source gap: the disability universe changes at age five, but the target surface contained only an under-eighteen total. Pass 53 adds `age_under_5` from male and female under-five cells in ACS table `B01001` and preserves its official variance-replicate covariance with every other registered `B01001` metric.

The twelve catchment estimates range from 964 to 2,621 people. Standard errors range from 185.6 to 500.1. All 72 reconstructed `B01001` point-and-standard-error checks are exact within floating-point tolerance, and the workbook records 252 lower-triangle covariance entries for the six registered age metrics across twelve catchments.

The extension has the intended semantic effect. The count of people age `0–4` is now point-identified in all twelve catchments, reducing its median feasible width from 7,090 to zero. This permits age-valid disability support without borrowing a national age ratio or allowing a solver to invent the split.

It does not solve the larger identification problem.

## 5. Point support remains feasible

The atomic basis now maps 39 published metrics onto 1,557 nonnegative coordinates per catchment:

- 596 person cells;
- 960 occupied household-unit cells; and
- one vacant-unit cell.

The under-five row increases the aggregation rank from 32 to 33 and reduces nullity from 1,525 to 1,524. All twelve catchments still admit exact nonnegative integer witnesses. All 468 published points reconstruct with zero residual, and every cross-ledger bridge retains nonnegative slack.

This is an important compatibility result. The new authority improves semantic precision without making the observed point surface internally infeasible.

The witnesses remain proofs of existence, not estimates. Their density varies sharply because the zero-objective feasibility solver may return different extreme points or degenerate bases. Neither a sparse nor a diffuse witness receives statistical authority from feasibility alone.

## 6. What remains unidentified

The under-five addition collapses exactly one tested interval. The other eight operational quantities remain unidentified in every catchment.

| Latent quantity | Median feasible width | Largest feasible width | Point-identified catchments |
| --- | ---: | ---: | ---: |
| group-quarters population under 18 | 501 | 1,686 | 0 of 12 |
| disabled people age `0–4` | 343.5 | 1,281 | 0 of 12 |
| civilian-noninstitutionalized group-quarters population | 64 | 810 | 0 of 12 |
| households with both a child and an older adult | 2,374.5 | 3,428 | 0 of 12 |
| households with no vehicle and limited English | 1,740 | 5,096 | 0 of 12 |
| renter-occupied units in structures with 50+ units | 3,122 | 6,676 | 0 of 12 |
| family households with children | 743.5 | 2,628 | 0 of 12 |
| electric-heat households in structures with 50+ units | 1,816 | 5,303 | 0 of 12 |

These are continuous linear-relaxation bounds, not posterior intervals. They show which quantities the public aggregates cannot determine. A future posterior may assign probability within these ranges only by adding a declared dependence model, donor evidence, protected relational data or another source of information.

The distinction matters directly to force design. The unknown intersections govern accessible mobility, language-capable contact, vertical-building continuity, medical-power support, household preservation and receiving capacity. An apparently precise synthetic population can make these requirements look measured even when they are primarily consequences of a hidden regularizer.

## 7. Boundary classification beyond the proof

The workbook classifies all 468 catchment–metric pairs by their distance from the nonnegative boundary using the ratio of published point to sampling standard error.

| Classification | Pairs | Distinct metrics | Interpretation |
| --- | ---: | ---: | --- |
| impossible exact moments | 7 | 1 | zero point and positive requested variance |
| boundary-sensitive | 15 | 6 | positive point no more than two sampling SEs from zero |
| interior | 446 | 38 | point more than two sampling SEs from zero |

The seven impossible pairs alone reject exact cloning. The additional fifteen boundary-sensitive pairs warn that a symmetric likelihood, flat prior or post-draw repair can still have consequential behavior even when no formal contradiction exists. `v3C0` must therefore register boundary-specific diagnostics rather than treating the problem as a generic high-dimensional Gaussian update.

## 8. Alternatives and decision

Three method families are evaluated.

### Alternative A: exact moment cloning

Force `E[A x] = ŷ` and `Cov[A x] = V` on nonnegative support.

**Decision:** rejected. Seven marginal moment pairs are impossible, and the construction conflates estimator error with state uncertainty.

### Alternative B: truncated or repaired Gaussian

Draw from the Pass 51 law and project each vector into civil support.

**Decision:** rejected. Pass 51 already demonstrates boundary bias, candidate rejection and tail instability. Pass 53 shows why exact repair cannot preserve the original boundary moments.

### Alternative C: atomic measurement-error posterior

Place a disclosed law on lawful atomic states and evaluate the observed estimates through a registered likelihood.

**Decision:** advance to preregistration. This construction preserves semantic support, retains official sampling-error information in its proper role and makes unidentified dependence explicit.

Advancement is not admission. No choice of likelihood, prior or sampler has yet passed the campaign ceiling.

## 9. Registered successor `v3C0`

The next pass must freeze its statistical constitution before producing candidate states.

### 9.1 Observation model

Register `p(ŷ | A x, V)` with the official variance-replicate blocks and the previously disclosed residual-sum-of-squares approximations for cross-table relationships. Test whether the Gaussian approximation is adequate near zero and for small housing categories. If a robust or transformed likelihood is used, it must reproduce estimator behavior rather than merely improve posterior appearance.

### 9.2 State support

Retain the Pass 53 nonnegative integer basis, all structural zeros and all cross-ledger bridges. No latent state may be made legal through after-the-fact clipping or projection.

### 9.3 Reference law and sensitivity cases

Register a maximum-entropy or weak loglinear reference law over atomic cells. Freeze at least three dependence cases before examining architecture performance:

1. weak association constrained primarily by observed margins;
2. a PUMS-informed association structure with local, adjacent and citywide support labels; and
3. an adverse rare-cell structure that increases operationally difficult intersections without violating evidence.

The reference law is a regularizer, not a discovered population. Every posterior result must distinguish likelihood information from prior structure.

### 9.4 Computation and diagnostics

The implementation must establish effective constrained sampling rather than return a collection of optimization points. It must report mixing or transport diagnostics, integer-support validity, bridge slack, weight concentration, rare-cell behavior and sensitivity to initial conditions.

### 9.5 Posterior-predictive admission

Before donor fitting, the ensemble must reconstruct the observed estimators under the registered measurement process, attain the declared interval-coverage tolerances, preserve nested `K=125–1,000` prefixes and clear all selected center, spread and tail-stability gates. The four Pass 52 semantic contradictions and every inherited failure injection remain mandatory.

No single preferred prior may be selected because it produces a favorable `A2` or `S3` result. If decision-relevant outcomes change materially across admissible dependence cases, the campaign result remains partially identified.

## 10. Institutional consequence: measurement-model custody

The finding expands the proposed Civil State Authority from a data custodian into a measurement-model institution. A mature Department of Resilience would routinely combine surveys, administrative systems, sensors, building records and field reports whose errors live on different probability spaces. Operational pressure will encourage analysts to turn all uncertainty into one convenient synthetic-world distribution. That shortcut can create impossible populations with internally polished confidence intervals.

The Authority therefore requires six standing functions:

1. **semantic support registry** — define lawful people, household, building, utility and service states;
2. **estimator registry** — preserve what each source measures, its sampling or observation process and its covariance authority;
3. **likelihood custody** — govern how observations update latent civil state without turning measurement error into state variation;
4. **prior governance** — disclose which dependencies are learned, borrowed, bounded or regularized and prohibit architecture-dependent tuning;
5. **posterior attestation** — certify support, calibration, sensitivity, privacy and reproducibility before operational use; and
6. **coverage evaluation** — compare predicted observations with later records and revise measurement models when coverage fails.

This is not an academic refinement. It determines whether the force deploys enough cooling, accessible transport, language capability, medical power and household support to the right places. Measurement-model custody is part of force readiness.

## 11. Decision boundary

Pass 53 establishes five claims:

1. the authoritative under-five margin and its complete within-table covariance are registered;
2. the extended 39-row point surface remains exactly feasible on the atomic support;
3. under-five population becomes point-identified, while eight other operational joints remain unidentified in every catchment;
4. exact cloning of published points and estimator covariance as state moments is impossible because seven marginal targets lie outside the nonnegative moment cone; and
5. the next defensible method is a preregistered measurement-error posterior over lawful atomic states.

It does not establish a posterior law, an admitted ensemble, donor weights, synthetic households, building occupancy, post-event building operability, demand, architecture performance or campaign outcomes. Formal `L0`, all `NCAC` performance gates, national force credit and renderings remain closed.

The paired workbook records the complete source extension, covariance authority, point-feasibility reconstruction, moment-boundary audit, partial-identification comparison, successor specification, empty outputs and formula-backed integrity checks. All sixteen sheets passed visual inspection, the formula-error scan found no errors and the Open XML archive validates. Workbook SHA-256 is `ed0a8c7dec3d08f4f508101faf97fd5baece19a33e38fc94cd5719a8cfe536f6`.
