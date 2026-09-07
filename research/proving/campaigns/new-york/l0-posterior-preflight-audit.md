# New York `L0` posterior preflight audit

**Audit:** `DF-NYC-L0-PR55-POSTERIOR-PREFLIGHT-v3C0`

**Decision:** **STOP—amend `G04` before full posterior execution.** The likelihood construction, posterior-propriety argument and reduced-support move grammar pass their preflight tests. The preregistered native-coordinate covariance-recovery gate does not apply a common statistical standard across covariance spectra or likelihood families: 37 of 48 fixed-state paths pass and 11 fail. No posterior state, donor fit, synthetic record, building assignment or architecture result is created.

**Paired model:** [New York `L0` posterior preflight audit](../../../../models/proving/campaigns/new-york/nyc-l0-posterior-preflight-audit.xlsx)

**Workbook SHA-256:** `b9a5a1a968dab8db2b5a658c552bc7f73bc65a33e870aa1a5a37b43d898cdab9`

## Executive judgment

Pass 54 authorized an architecture-blind challenge before a 1,152-chain posterior computation could begin. Pass 55 performs that challenge. It reconstructs the source estimates, rebuilds the lawful aggregation operator, completes three covariance cases, reduces every likelihood to the registered 33-dimensional independent observation space, proves the twelve likelihood–prior combinations proper, enumerates five reduced-support move graphs, injects five known defects and draws 100,000 fixed-state estimator replicates for each of four likelihoods in each of twelve catchments.

The preflight works as intended because it stops. All 1,584 simulated marginal-variance ratios fall inside the registered `0.98–1.02` interval, the deterministic covariance factors are correct and the observed Frobenius errors are of the size predicted by sampling theory. Yet the absolute native-coordinate relative-Frobenius ceiling of `0.01` rejects 11 paths. The failure rate is one of twelve under the zero cross-table Gaussian, none under the shared Gaussian, two under the concordant Gaussian and eight under the covariance-preserving Student-`t₇` case. A single common cutoff is therefore partly a test of covariance effective rank and fourth moments, not merely implementation fidelity.

That is a defect in the registered gate, not a license to waive it. `v3C0` remains binding and the full 57.6-million-transition run remains prohibited. This audit freezes a successor, `v3C0A`, that keeps the same 100,000 draws, paths, likelihoods and seeds but replaces `G04` with a whitened, element-wise and campaign-familywise calibrated discrepancy test. The amendment is not executed here. The next pass must rerun the entire 48-path preflight under the new rule before any posterior chain starts.

## Why a preflight precedes 57.6 million transitions

The registered posterior is not one model fit. It is a twelve-case sensitivity experiment over twelve catchments, with eight chains per path, 10,000 warmup transitions and 40,000 production transitions per chain. Its ceiling is:

\[
12\ \text{catchments}\times 12\ \text{cases}\times 8\ \text{chains}\times 50{,}000
=57{,}600{,}000\ \text{transition proposals}.
\]

That computation would be scientifically wasteful if a covariance factor were scaled incorrectly, a redundant estimator coordinate were treated as independent, the flat ledger-total prior produced an improper posterior, or the move grammar disconnected lawful states. The preflight therefore tests deterministic construction, fixed-state estimator behavior and small exact support graphs before producing a candidate posterior state. It also preserves the architecture firewall: zero `A2` or `S3` outcome reads occurred.

The stopping rule is constitutional. The research program does not compensate a failed gate with a high score elsewhere, silently select the likelihood that passed, increase the Monte Carlo sample until the same numerical cutoff passes, or inspect architecture consequences before deciding whether a discrepancy matters.

## Reconstructed authority and independent observation space

The audit begins from the Pass 51 covariance method, the Pass 52 lawful atomic operator, the Pass 53 authoritative under-five correction and the Pass 54 registration. It exactly reconstructs 276 variance-replicate point and standard-error authorities. The 39 published margins map from 1,557 nonnegative integer atomic coordinates. Six exact row identities leave a rank-33 likelihood basis and a 1,524-dimensional atomic null space. The relative projection residual is `1.76×10⁻¹⁵`; the largest singular value is `72.36` and the smallest retained value is `0.970`.

This separation is central. Rank 33 describes the information carried by the estimator vector after exact identities are removed. Nullity 1,524 describes the many lawful civil-state directions not identified by those estimates. The former belongs in the likelihood. The latter cannot be erased by numerical factorization; it is addressed only through declared state priors and sensitivity reporting.

## Covariance completion and positive definiteness

The three Gaussian covariance cases are regenerated without outcome access:

- `L0_GAUSS_ZERO`, with zero cross-table starting structure;
- `L1_GAUSS_SHARED`, with shared geographic and population structure; and
- `L2_GAUSS_CONCORDANT`, with concordant cross-table structure.

All converge after 56 reconciliation iterations. Their identity residuals are `9.49×10⁻¹¹`, `7.95×10⁻¹¹` and `7.60×10⁻¹¹`; official within-table Gram errors remain below `3.60×10⁻¹⁵`. Across three cases and twelve catchments, all 36 reduced covariance matrices have rank 33 and are positive definite. The fourth likelihood, `L3_T7_ZERO`, reuses the `L0` covariance but uses a multivariate Student-`t` law with seven degrees of freedom. Its scale must be `5V/7`, because the covariance of a `t₇` variable is `7/5` times its scale matrix.

The audit detects both relevant construction defects. Attempting to factor all 39 coordinates exposes rank 33 and rejects the singular full covariance. Passing `V` directly as the `t₇` scale produces marginal variance ratios from `1.388` to `1.423` and fails immediately.

## Posterior propriety before sampling

Every registered prior retains an improper flat prior over the two nonnegative ledger totals. That shortcut is lawful only if the likelihood makes the posterior normalizing constant finite. The audit closes the proof for all twelve likelihood–prior cases.

For each Gaussian case, positive definiteness in the reduced observation space supplies quadratic decay in the ledger-total directions. Conditional branch-composition references are proper. The PUMS partial-pooling prior has a positive probability floor, and the adverse tilt is bounded by construction, so neither destroys integrability.

For `t₇`, the reduced likelihood has dimension 33 and polynomial radial decay. Along the two-dimensional ledger-total lattice the resulting tail exponent is 40, which exceeds the dimension requiring summability. The same proper conditional references and bounded tilt preserve finiteness. This is an analytical precondition, not evidence of good mixing or predictive calibration.

## Fixed-state likelihood calibration

For each of the 48 likelihood–catchment paths, the audit freezes a lawful state, draws 100,000 estimator residuals and compares the empirical covariance with the registered target. The diagonal test covers `48×33=1,584` coordinates. Every diagonal ratio passes. Failures arise only from the single relative-Frobenius requirement.

| likelihood | paths passing | paths failing | median observed error | median analytical RMS | maximum observed error |
|---|---:|---:|---:|---:|---:|
| `L0_GAUSS_ZERO` | 11 | 1 | 0.00799 | 0.00821 | 0.01070 |
| `L1_GAUSS_SHARED` | 12 | 0 | 0.00817 | 0.00797 | 0.00997 |
| `L2_GAUSS_CONCORDANT` | 10 | 2 | 0.00729 | 0.00753 | 0.01177 |
| `L3_T7_ZERO` | 4 | 8 | 0.01113 | 0.01091 | 0.01395 |

For a Gaussian target covariance `V`, the leading relative root-mean-square sample-covariance error is approximately

\[
\operatorname{RMS}_{G}\approx \sqrt{\frac{r_{\mathrm{eff}}+1}{N}},
\qquad
r_{\mathrm{eff}}=\frac{\operatorname{tr}(V)^2}{\lVert V\rVert_F^2}.
\]

The catchment-case effective ranks range from `4.07` to `8.01`. The same absolute cutoff therefore has different false-stop behavior as the spectrum changes. For an elliptical distribution with fourth-moment factor `κ`, the corresponding approximation is

\[
\operatorname{RMS}_{\kappa}\approx
\sqrt{\frac{\kappa r_{\mathrm{eff}}+2\kappa-1}{N}}.
\]

Gaussian draws have `κ=1`; Student-`t₇` draws have `κ=(7-2)/(7-4)=5/3`. Equal target covariance does not imply equal sample-covariance noise. The observed pattern—roughly 0.8-percent median Gaussian error and 1.1-percent median `t₇` error—is what the fourth moments predict. The original `0.01` cutoff therefore cannot be interpreted as a common fidelity test.

## Reduced-support move challenge

Exact irreducibility over the full 1,557-coordinate, unbounded state space is not established here. Instead, the audit enumerates five small support problems chosen to isolate the registered move families:

- a 56-state scale-and-composition simplex is connected by total and person reallocation moves; removing the composition move produces 21 components;
- a three-state fixed-margin `2×2` interaction fiber is connected by the registered cycle move; removing it produces three components;
- a 21-state duplicate-aggregate fiber is connected by the integer-kernel move; removing it produces 21 components;
- a six-state person–household bridge corner is connected with diameter two; removing bridge relief retains connectivity but doubles diameter to four; and
- a two-state fixed-margin table with a structural zero is connected by lawful rectangles without entering the prohibited cell.

These tests show that the implementation expresses the intended local mechanisms and detects known stuck-chain constructions. They do not prove that every full-scale fiber is connected or that the eventual Markov chains mix efficiently. Full-chain convergence, dispersed starts, effective sample size and tail stability remain admission gates.

## Failure-oriented evidence

Five seeded defects are detected:

1. the wrong Student-`t` scale inflates variance;
2. retaining all 39 estimator coordinates exposes a singular covariance;
3. clipping a centered estimator residual at zero creates a `0.401`-standard-deviation mean shift and reduces variance to `0.342` of target;
4. removing the `2×2` interaction move yields three disconnected components; and
5. removing the integer-kernel move yields 21 disconnected components.

Passing known-failure tests matters because a plausible-looking posterior can still be generated by a semantically invalid likelihood or a sampler trapped in one part of a lawful fiber. The Department of Resilience concept requires a standing ability to prove how a model fails, not only to publish its favored output.

## Frozen amendment `v3C0A`

The amended test retains exactly 100,000 draws per path, all 48 paths, the committed seed grammar and the 33-dimensional basis. It does not increase the sample after observing failure. Before stochastic testing, the implementation must prove relative factor-covariance error at or below `10⁻¹²`: `LLᵀ=V` for Gaussian cases and `(7/5)LLᵀ=V` for the `t₇` case.

For stochastic calibration, center each simulated path and whiten it with the registered target Cholesky factor. Test the 561 unique elements of the 33-by-33 whitened sample covariance. Across 48 paths that creates 26,928 simultaneous two-sided comparisons. `v3C0A` fixes familywise alpha at `0.01` and the Bonferroni critical value at `|z|≤5.083081293`.

With `N=100,000`, the standardized element errors use

\[
SE(\hat S_{ii})=\sqrt{\frac{3\kappa-1}{N-1}},
\qquad
SE(\hat S_{ij})=\sqrt{\frac{\kappa}{N-1}}\quad(i\ne j),
\]

where `κ=1` for Gaussian and `κ=5/3` for Student-`t₇`. Native and whitened Frobenius errors remain reported diagnostics with analytical RMS references, but they no longer govern admission. The amendment is a version boundary, not an editorial correction. It receives identifier `DF-NYC-L0-PR55A-POSTERIOR-PREFLIGHT-v3C0A` and must be rerun in a later pass.

## Institutional meaning

This preflight illustrates what a mature Civil State Authority inside a Department of Resilience would do. It would own estimator semantics, covariance lineage, lawful state support, prior governance, numerical assurance, privacy, model-case separation and independent reproduction as a mission system. It would budget for failed tests and prevented runs, because stopping an invalid model before it influences fleet posture, hospital allocation or evacuation policy is an operational success.

That institution is not a renamed statistical office. Its output is deployable civil-state confidence: knowing which population, building and dependency claims are measured; which are inferred; which depend on priors; which remain partly identified; and which cannot yet support an operational decision. Military force projection invests in test ranges, independent verification, red teams and configuration control. Equal civil projection requires the same depth of epistemic infrastructure.

## Decision boundary and next admissible work

Pass 55 establishes that the source reconstruction, lawful row basis, three covariance completions, 36 reduced positive-definite matrices, twelve propriety arguments, five reduced-support graphs and five seeded failure responses pass. It also establishes that the original `G04` gate fails 11 of 48 paths for a statistically interpretable reason and cannot be silently relaxed.

It does **not** establish full-space irreducibility, chain convergence, posterior calibration, prior robustness, donor adequacy, privacy, building operability or architecture performance. It executes zero posterior transitions and produces zero posterior states, donor rows, synthetic records, building assignments and outcome reads.

The next admissible pass is narrow: implement `v3C0A`, rerun all 48 fixed-state paths from the committed seed grammar and evaluate the amended gate. The 57.6-million-transition posterior remains prohibited until that preflight passes. Rendering work remains deferred until the force and asset requirements have matured.
