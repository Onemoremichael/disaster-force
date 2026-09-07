# New York `L0` atomic measurement-error posterior preregistration

> **Successor authority:** The [Pass 55 posterior preflight audit](l0-posterior-preflight-audit.md) implements the preregistered construction but stops before posterior execution because `G04` passes only 37 of 48 fixed-state paths. It freezes a versioned `v3C0A` replacement gate; the amended preflight has not yet run.

**Registration:** `DF-NYC-L0-PR54-ATOMIC-POSTERIOR-v3C0`

**Decision:** freeze a twelve-case factorial measurement-error posterior over lawful atomic civil states before sampling. No posterior state, donor fit, synthetic record, building assignment or architecture outcome is produced or admitted in this pass.

**Paired model:** [New York `L0` atomic posterior preregistration](../../../../models/proving/campaigns/new-york/nyc-l0-atomic-posterior-preregistration.xlsx)

## Executive judgment

Pass 53 proved that the proposed exact state-moment target was impossible. Seven official margins have point estimate zero and positive sampling error; no distribution over nonnegative states can simultaneously have mean zero and positive variance. That proof did more than stop a bad engine. It exposed a category error between uncertainty in a published estimator and uncertainty about the true civil state after the estimator is observed.

Pass 54 replaces that category error with a statistical constitution. The observed 39-margin estimator for each catchment is evaluated through a rank-reduced likelihood conditional on the aggregate margins implied by one lawful 1,557-cell integer state. Official variance-replicate covariance remains in the measurement model. Dependence among the unobserved atomic cells enters through three declared state-prior cases rather than masquerading as observed covariance. Four likelihood cases crossed with those three priors create twelve cases, all of which remain separate through donor fitting and any later architecture analysis.

The design deliberately refuses to produce a single preferred posterior. Its primary Gaussian likelihood is accompanied by two cross-table covariance completions and a covariance-preserving heavy-tail boundary case. Its weak branch-balanced prior is accompanied by a geographically labeled PUMS partial-pooling prior and a bounded adverse operational-dependence tilt. If the later force decision changes across these cases, the result is likelihood-sensitive, prior-dominant or both. It does not become certain because one case looks plausible or performs well for `A2` or `S3`.

The registered execution is substantial: twelve catchments, twelve cases, eight chains per catchment-case, 10,000 warmup and 40,000 production transitions per chain. That is 1,152 chains and 57.6 million transition proposals. A deterministic hash-ordered retention rule selects 125 production states per chain and interleaves them into exactly nested `K=125, 250, 500, 1,000` prefixes, producing at most 144,000 candidate posterior states. The dense atomic payload ceiling is 224,208,000 values, or 896,832,000 raw bytes at four bytes per integer, before compression and manifests.

None of those candidate states is admitted by preregistration. Twenty-five co-governing gates must later pass without a compensating score. They cover custody, rank, covariance, posterior propriety, estimator simulation, boundary behavior, semantic support, sampler convergence, nested-prefix balance, tail stability, posterior-predictive behavior, sensitivity disclosure, privacy, the architecture firewall and independent reproduction. Twenty-three deliberate failure injections specify how the implementation must fail before it is trusted.

This pass is therefore progress without fabricated evidence. It converts “build a posterior” into a falsifiable, architecture-blind research program. It also sharpens the institutional case for a standing Civil State Authority inside the Department of Resilience: operational civil knowledge requires permanent custody of semantics, measurement models, priors, computation, privacy and independent attestation—not an improvised synthetic-data exercise during a catastrophe.

## 1. Why preregistration is the next scientific act

The New York campaign is intended to compare a conventional neighborhood continuity and access cell, `A2`, with a technology-forward rival, `S3`, under vertical heat-blackout conditions. The comparison is unusually vulnerable to hidden analytical choice. Public data identify many one-way margins but not the operationally decisive joints: who lives alone and cannot use stairs, which medically dependent households occupy high-rise buildings, where language access and mobility needs overlap, or which buildings retain water pressure and cooling when power fails.

A synthetic civil state must therefore add structure that the public margins do not observe. If that structure is chosen after architecture performance is visible, the experiment ceases to be confirmatory. A prior that concentrates difficult households in high-rise buildings could favor or punish one architecture. A covariance completion, boundary transformation, repair rule, chain initialization or sample-retention rule could do the same. Even apparently technical choices can function as unrecorded outcome tuning.

Preregistration closes that path in four ways:

1. it names every likelihood and prior case before posterior execution;
2. it requires the full likelihood-by-prior factorial rather than allowing case deletion;
3. it keeps all architecture outcomes cryptographically and procedurally inaccessible during model fitting; and
4. it defines numerical, semantic, predictive, privacy and reproduction gates in advance.

The pass does not claim that these are the only reasonable models. It claims that they are a bounded, auditable challenge set sufficient to expose whether a later conclusion depends on measurement covariance, tail shape, geographic donor borrowing or adverse operational dependence. A later amendment is possible, but it must create a new registration and cannot overwrite this one.

## 2. The statistical constitution

### 2.1 Separate objects and probability spaces

For catchment `c`, let:

- `x_c` be a vector of 1,557 nonnegative integer atomic counts;
- `A` be the fixed `39 × 1,557` aggregation operator;
- `y_c = A x_c` be the true aggregate margins implied by the state;
- `ŷ_c` be the published 39-margin estimator;
- `Q` be a fixed orthonormal basis for the 33-dimensional independent row space of `A`; and
- `V_cm` be the measurement covariance under likelihood case `m` after rank reduction.

The target for likelihood case `m` and prior case `p` is:

```text
p(x_c | ŷ_c,m,p) ∝ p(ŷ_c | A x_c,V_cm) p₀(x_c | p)
                    × 1{x_c is a lawful nonnegative integer state}.
```

The likelihood evaluates the reduced residual:

```text
r_c(x) = Qᵀ(ŷ_c − A x_c).
```

Only 33 independent coordinates enter because the 39 registered margins contain exact additive identities. Evaluating all 39 residuals as independent would count deterministic information more than once and produce a singular covariance. The rank basis is fixed before any chain begins, and the reduced covariance must be positive definite with minimum eigenvalue greater than `10⁻¹⁰` times its maximum eigenvalue.

This construction assigns distinct authority to distinct objects. `V` describes repeated-sample estimator error. The prior describes unobserved state composition and dependence. The atomic support defines legal civil states. The posterior describes uncertainty after those authorities are combined. None is allowed to impersonate another.

### 2.2 Boundary behavior

The estimator residual remains real-valued even when the corresponding state margin is constrained to be nonnegative. A published estimate of zero is not clipped evidence that the true state must equal zero; it is one estimator realization with known sampling uncertainty. Conversely, a negative simulated estimator residual is not an illegal civil state. It is legal behavior in the measurement process.

The implementation must therefore never truncate, clip or project the estimator residual at zero. It must also never repair an illegal atomic proposal after drawing it. Illegal states receive posterior probability zero. This two-sided discipline preserves the essential separation revealed by Pass 53: the observation model may cross a boundary that the latent state may not.

## 3. Four registered likelihood cases

The likelihood set tests two uncertainties: unidentified cross-table estimator covariance and approximation error near a nonnegative boundary.

### `L0_GAUSS_ZERO`: primary Gaussian measurement case

This case uses the Pass 51 `R0` completion: official within-table covariance blocks are retained, while unidentified cross-table covariance is set to zero. The rank-reduced residual follows a multivariate Gaussian law. This is the primary measurement case because it adds the fewest cross-table assumptions.

It is not called truth. Zero cross-table covariance is an explicit completion of missing information.

### `L1_GAUSS_SHARED`: moderate shared-place covariance

This case uses the Pass 51 `R1` completion, which induces moderate covariance among tables through shared geographic and population structure while preserving each official within-table block and marginal standard error. It tests whether the posterior changes when estimator errors from different tables are not conditionally independent.

### `L2_GAUSS_CONCORDANT`: strong concordant covariance

This case uses the Pass 51 `R2` completion, a stronger same-direction cross-table dependence case. It is not promoted because it fits a preferred result. Its function is to bound a material but unidentified part of the measurement model.

### `L3_T7_ZERO`: covariance-preserving heavy-tail case

This case retains the `R0` covariance authority but replaces the Gaussian residual with a multivariate Student `t` distribution with seven degrees of freedom. For a `t_ν` law, covariance equals `ν/(ν−2)` times the scale matrix. The registered scale is therefore `5/7 V`, so the covariance remains exactly `V` rather than being accidentally inflated by `7/5`.

The case tests sensitivity to outliers and boundary-adjacent estimator behavior. It is not a license to use heavy tails to rescue a poor posterior-predictive result. A unit test that substitutes `V` directly as the `t` scale is a mandatory failure injection.

No likelihood transformation may be selected from posterior appearance or architecture performance. The four cases remain separate.

## 4. Three lawful state-prior cases

The aggregate operator has rank 33 and the atomic basis has 1,557 cells, leaving 1,524 directions that the registered margins cannot identify. A likelihood alone cannot choose among all states on that fiber. The prior cases make that choice visible.

### `P0_WEAK_BRANCH`: weak branch-balanced reference

The weak case assigns equal probability at each lawful categorical branch rather than equal weight to every terminal atomic cell. Equal terminal-cell weights would silently favor categories with more encoded subcells. The branch-balanced construction avoids that enumeration artifact.

Ledger totals receive the registered improper flat prior on the nonnegative integers. That weak reference is permitted only if posterior propriety is proved for every likelihood-prior case: the measurement likelihood must make the normalizing constant finite rather than merely appear numerically concentrated. `P1` and `P2` inherit the same ledger-total prior. All optional loglinear association coefficients are fixed to zero.

`P0` is a weak-information sensitivity case, not a claim that civil attributes are actually independent.

### `P1_PUMS_POOL`: tiered PUMS partial pooling

The empirical-reference case uses the Pass 48 donor classes, but only as association evidence. PUMS geography is labeled at three support tiers: local, touching-PUMA and citywide. No tier is allowed to masquerade as tract residence or post-event building occupancy.

Every categorical probability receives a floor of `10⁻⁸` so observed sparsity does not become an accidental structural zero. The pooling concentration is selected solely by leave-one-PUMA-out predictive log loss over the fixed grid `{1, 4, 16, 64, 256}`. That selection is completed and hashed before posterior sampling. It cannot use architecture outputs, posterior operational estimands or a later donor-fit score.

The resulting prior is evidence-informed, but its information remains limited: PUMS supports household and person relationships at public-use geography and does not observe which tract household occupies which building or what remains operable during an outage.

### `P2_ADVERSE_TILT`: bounded operational stress prior

The adverse case begins with `P1` and multiplies its weight by:

```text
exp(log(4) × H(x)),    0 ≤ H(x) ≤ 1.
```

`H(x)` is the equal-weight mean of eight operational joint quantities, each normalized to the feasible range established in Pass 53. The maximum prior odds tilt is therefore `4:1`, large enough to test decision relevance without collapsing the support onto an engineered extreme.

This is a stress prior, not a belief distribution. It asks whether a modest, explicitly adverse concentration of hard-to-serve relationships changes the later architectural judgment. The eight terms, their equal weights, the normalization ranges and the `4:1` cap are frozen. Changing the tilt after observing results invalidates the version.

## 5. The full factorial is the result surface

Four likelihoods crossed with three priors produce twelve cases. Each of the twelve catchments is sampled separately under every case, yielding 144 catchment-case paths. All are retained as coequal sensitivity evidence.

This design rules out a common but consequential shortcut: selecting one “best” posterior and treating model uncertainty as resolved. The later reporting grammar is instead:

- **measurement-robust** if the decision is stable across likelihood cases;
- **prior-robust** if it is stable across state-prior cases;
- **likelihood-sensitive** if a likelihood-family change reverses a decision;
- **prior-dominant** if the normalized posterior-median range across `P0/P1/P2` exceeds `0.25` of the feasible width; and
- **partially identified** if important case variation remains after numerical gates pass.

Prior dominance is not a numerical failure. It is a substantive finding that prohibits a single-state claim. A likelihood reversal similarly requires retaining the cases and refusing confirmatory architectural language. Neither condition may be hidden by pooling case outputs.

## 6. Constrained computation on civil support

### 6.1 Chain design

Each catchment-case path uses eight independently initialized Markov chains. Every chain has:

- 10,000 warmup iterations;
- 40,000 production iterations;
- adaptation ending at the warmup boundary; and
- 125 deterministically retained production states.

The target is evaluated by a parallel Metropolis-within-Gibbs scheme on integer atomic states. All diagnostics use the complete post-warmup chain, not only the thinned downstream sample. Warmup states can never enter the retained ensemble.

Seeds follow a versioned grammar derived from SHA-256 of the registration, case, catchment and chain identity. This provides separation and exact rerun capability without implying that deterministic pseudorandomness is independent reproduction.

### 6.2 Registered move mixture

The sampler must mix across aggregate scale, within-ledger composition, unidentified interactions and tight bridge facets. Six move families are frozen:

| Move | Weight | Function |
| --- | ---: | --- |
| total birth/death | 0.10 | change a lawful ledger scale with asymmetric boundary correction |
| person reallocation | 0.25 | move mass among person atoms |
| household reallocation | 0.25 | move mass among occupied household atoms |
| `2×2` interaction cycle | 0.20 | change dependence while preserving selected one-way margins |
| integer null-`A` circuit | 0.10 | move on the exact likelihood-flat aggregate fiber |
| bridge relief | 0.10 | move near population–household feasibility boundaries |

The weights sum to one and may adapt only during warmup under a recorded rule. Their existence does not prove that the chain is irreducible. Connectivity must be demonstrated on reduced enumerated supports, and dispersed chains must traverse both aggregate-changing and aggregate-neutral directions.

### 6.3 Exactly nested retention

Downstream architecture comparisons require `K=125, 250, 500, 1,000` ensembles that are exact prefixes of one deterministic ordering. Independent redraws at each `K` would confound ensemble size with different random states.

For each chain, the implementation orders its 40,000 production indices by a SHA-256 key and takes the first 125. It then interleaves the eight chain-specific selections using a case-specific rotation. Every nested prefix must differ by no more than one state in its contribution from any two chains.

This rule makes the convergence ceiling architecture-blind, reproducible and chain-balanced. Selecting favorable retained draws or reordering them after seeing operational outcomes is a registered failure.

## 7. Execution and storage envelope

The workbook derives the complete ceiling from registered inputs:

| Object | Count |
| --- | ---: |
| factorial cases | 12 |
| catchment-case paths | 144 |
| Markov chains | 1,152 |
| transition proposals | 57,600,000 |
| retained candidate states | 144,000 |
| retained atomic values | 224,208,000 |
| dense `int32` payload ceiling | 896,832,000 bytes |
| aggregate values | 5,616,000 |
| posterior-predictive estimator values | 5,616,000 |

The raw byte figure is a planning ceiling, not a file-format prescription. Controlled execution should use chunked compressed arrays, immutable manifests and per-chunk hashes. Public artifacts may contain only disclosure-safe aggregates, diagnostics and commitments. They may not contain household/person identities, relationship keys, addresses, serial numbers or row-level synthetic records that could be joined back to protected data.

## 8. Twenty-five co-governing admission gates

No weighted score can compensate for a failed gate. The implementation either passes every applicable gate or stops at the registered ceiling.

### Custody and likelihood construction

1. Every source, code, seed and case manifest is present and SHA-256 valid.
2. The independent-row basis has dimension 33 in every catchment-case.
3. Every reduced covariance is positive definite above the registered eigenvalue ratio.
4. A finite posterior normalizing constant is established for every likelihood-prior case.
5. A 100,000-draw fixed-state simulation recovers the registered covariance: diagonal ratios must lie in `[0.98,1.02]` and relative Frobenius error must be at most `0.01`.
6. A boundary test confirms that a zero observed estimate may coexist with positive latent count and that the estimator residual is never truncated.

### Semantic support

7. Every warmup and production state is a nonnegative integer vector.
8. Structural zeros and age-valid disability rules have zero violations.
9. Cross-ledger bridges have zero accepted violations.
10. Post-draw repair and projection are never called and shift zero states.

### Sampling and nested convergence

11. Rank-normalized split `R̂` is at most `1.01` for every registered margin and operational estimand.
12. Bulk effective sample size is at least 400 for each reported quantity and catchment-case.
13. Tail effective sample size is at least 200.
14. Maximum dispersed-start mean contrast is at most `0.10` pooled posterior standard deviations.
15. Every nested prefix has a maximum chain-contribution difference of one.
16. Maximum `K/2`-to-`K` mean-share change is at most `0.0025`.
17. Maximum selected-quantile change is at most `0.0050`.
18. Maximum Jensen–Shannon divergence for registered joint diagnostics is at most `0.010`.

### Predictive behavior and sensitivity

19. Fixed-state simulations attain 50/80/90/95-percent empirical interval coverage inside simultaneous 99-percent binomial bands.
20. The observed rank-space Mahalanobis discrepancy lies inside the central 98-percent posterior-predictive reference interval in every catchment-case.
21. A prior range above `0.25` of feasible width triggers `PRIOR_DOMINANT`, retention of separate cases and prohibition of a single-state claim.
22. Any likelihood-family decision reversal triggers `LIKELIHOOD_SENSITIVE` and prohibition of confirmatory architecture language.

### Rights, firewall and reproduction

23. Public relational or donor identity fields have zero records and zero identifiers.
24. Architecture outcomes are read zero times during posterior fitting.
25. An independent implementation reaches the same gate decisions and reproduces numerical summaries within declared Monte Carlo error.

The gates distinguish numerical failure from epistemic sensitivity. `PRIOR_DOMINANT` and `LIKELIHOOD_SENSITIVE` preserve evidence rather than discard an inconvenient case. All other stop failures deny ensemble admission.

## 9. Posterior-predictive validation is not self-congratulation

Posterior-predictive checks can be misleading if they merely confirm that the same flexible model can reproduce data it was designed to fit. This registration uses two distinct predictive obligations.

First, fixed-state calibration tests the likelihood in isolation. A known lawful state generates repeated synthetic estimators. Coverage and covariance recovery are assessed without state inference. This catches covariance indexing, rank reduction, Student-`t` scaling and boundary-residual errors.

Second, the fitted posterior generates one predictive estimator vector per retained state. The observed reduced-space discrepancy must not be an extreme draw under any admitted case. This asks whether the combined likelihood and prior can reproduce the estimator actually observed without placing it in a tail.

Passing these checks does not prove that the latent joint state is true. A prior can be predictive at observed margins while controlling unidentified joints. That is why partial-identification bounds and prior-sensitivity reporting remain co-governing.

## 10. The operational estimands remain exposed

The nine quantities carried forward from Pass 53 are not selected because they are statistically convenient. They are the joints most likely to change access labor, language capacity, vertical movement, utility support and reception demand:

1. people age `0–4`;
2. group-quarters population under 18;
3. disabled people age `0–4`;
4. civilian-noninstitutionalized group-quarters population;
5. households containing both a child and an older adult;
6. households with no vehicle and limited English;
7. renter-occupied units in structures with 50 or more units;
8. family households with children; and
9. electric-heat households in structures with 50 or more units.

Only the under-five total is point-identified by the registered margins. The other eight have nonzero feasible width in all twelve catchments. Later reporting must show posterior medians, 50/80/90/95-percent intervals, prior-to-posterior shift and normalized position within the feasible range for every case. A narrow posterior interval on one of these quantities is not automatically strong evidence; it may be concentrated prior structure.

## 11. Deliberate failure before trust

Twenty-three injected defects form a minimum adversarial test suite. They cover:

- negative and fractional atoms;
- structural-zero and cross-ledger bridge violations;
- duplicated identities in a singular 39-row likelihood;
- non-positive-definite covariance;
- incorrect Student-`t` scaling;
- estimator truncation at zero;
- renewed cloning of estimator covariance as state covariance;
- omission of an unfavorable prior case;
- silent citywide donor pooling;
- post-output adverse-tilt changes;
- unregistered seeds and warmup leakage;
- stuck chains and outcome-selected retention order;
- posterior-predictive conflict;
- concealed prior dominance;
- architecture-outcome access during fitting;
- public donor or relational identities;
- source, code or output hash mismatch;
- disagreement between independent implementations; and
- nested prefixes dominated by one chain.

Each defect has an expected stop, invalidation or sensitivity response. A test system that cannot detect its own seeded errors has not earned the right to interpret an unseeded run.

## 12. The architecture firewall

The posterior workstream may read source estimates, variance replicates, the atomic schema, PUMS donor evidence and frozen case labels. It may not read `A2` or `S3` outcome tables, building-assignment results, campaign aggregates or any derivative that reveals which architecture benefits from a modeling choice.

Six rules govern the separation:

1. architecture outcome tables remain inaccessible until posterior, donor, compiler and reproduction gates pass;
2. architecture labels exist only as schema strings outside likelihood, prior, proposal and diagnostic code;
3. prior hyperparameters use semantic and donor evidence only and are hashed before sampling;
4. all twelve cases remain in the manifest with no post-fit deletion or promotion;
5. public release is limited to disclosure-safe aggregates, diagnostics and commitments; and
6. formal `L0` cannot change until every co-governing gate and external custody obligation is satisfied.

The firewall is both technical and organizational. Separate access roles, immutable audit logs and countersigned release decisions are required. A promise that analysts will ignore visible outcomes is not adequate blinding.

## 13. What the preregistration refuses to create

Ten output families are intentionally present with zero rows: posterior atomic states, posterior aggregate margins, posterior-predictive estimators, convergence diagnostics, prior-sensitivity results, donor weights and integer donor counts, synthetic households and persons, building assignments and operability, architecture outcomes, and campaign aggregates.

This negative result surface prevents a registration artifact from being mistaken for an executed model. It also creates a clear custody boundary: any nonzero row in these tables before a registered execution and independent attestation is a defect, not progress.

## 14. Institutional consequence: a Civil State Authority

A mature Department of Resilience cannot rely on a one-time analytical team to improvise population truth during a catastrophe. It needs an institution with responsibilities analogous to intelligence preparation, hydrographic authority, operational test and configuration control—but governed for civil rights, purpose limitation and public legitimacy.

The emerging **Civil State Authority** would own at least eight permanent functions:

1. **semantic constitution** — define lawful person, household, building, utility and service states and their bridges;
2. **measurement registry** — record what every survey, administrative system, sensor and field report actually measures, including error and covariance authority;
3. **protected data federation** — reconcile local, state, tribal, federal, utility and health records without creating a general-purpose surveillance repository;
4. **prior and model governance** — distinguish observed relations from borrowed, regularized, bounded and stress-tested dependence;
5. **disconnected operational updating** — merge field observations and service changes under degraded communications with provenance and conflict handling;
6. **privacy and rights engineering** — enforce minimum necessary access, retention limits, public disclosure controls, contestability and independent civil-rights review;
7. **computational assurance** — maintain reproducible samplers, adversarial tests, model manifests and independent implementations; and
8. **decision attestation** — state what is measured, inferred, sensitive, unknown and prohibited before operational plans receive evidence credit.

This is a new public technical profession, not simply a larger data office. Its output must be useful enough to route cooling, water, clinical power, accessible transport, language support and household-preserving reception while remaining constrained enough that emergency capability does not become permanent population monitoring.

The `v3C0` registration is a small prototype of that institutional grammar. It shows how a national resilience force would treat civil knowledge as a governed mission system: designed from first principles, exercised under failure, independently reproduced and denied operational authority until it passes.

## 15. Decision boundary and next admissible work

Pass 54 establishes that:

1. estimator uncertainty, latent-state uncertainty and semantic support have separate governing authorities;
2. four likelihood cases and three prior cases are frozen as a twelve-case factorial challenge set;
3. a lawful constrained sampler, move grammar, seed grammar and exactly nested retention order are specified;
4. the complete execution and storage ceiling is reconciled;
5. twenty-five admission gates and twenty-three deliberate failures are fixed before posterior execution; and
6. architecture outcomes remain sealed and all posterior-derived output tables remain empty.

It does not establish that the posterior is proper in implementation, that chains mix, that the likelihood reproduces its covariance, that any candidate ensemble is calibrated, that PUMS partial pooling is decision-robust, that a donor compiler works, or that either architecture performs. It creates tests for those claims.

Pass 55 subsequently performs that architecture-blind preflight and stops before posterior chains: reduced-support connectivity passes, but the registered `G04` fixed-state covariance rule passes only 37 of 48 paths. The live next action is therefore the versioned `v3C0A` preflight rerun described in the successor audit, not execution of all 144 catchment-case paths. If the amended preflight passes, the full factorial may begin; any later stop-gate failure still denies ensemble admission. If all numerical gates pass but prior dominance or likelihood reversal appears, the cases remain separate and the campaign result remains partially identified.

Only an admitted posterior ensemble may proceed to the already registered tier-labeled household-preserving donor fit. Medical-power coverage, protected household–building binding, operational building state, observed service territories, causal-feasibility rules, salted external holdout custody and independent human-subject, disability, civil-rights, ethics and worker-safety review remain parallel obligations. Formal `L0`, all twenty `NCAC` gates, national force credit and renderings remain closed.

The paired workbook contains the version identity, source commitments, probability objects, likelihoods, priors, full case matrix, target construction, sampler, move mixture, estimands, gates, failure tests, firewall, formula-derived scale, empty outputs and integrity controls. Every one of its 17 sheets passed visual inspection; all 14 formula-backed integrity checks report `Met`; the formula-error scan found zero errors; and the Open XML archive validates. Workbook SHA-256 is `47ff05bb55cc89f326225ca79de304f8110f4707baaef34a8715529d8de22231`.
