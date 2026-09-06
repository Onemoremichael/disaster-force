# New York `L0` civil-state compiler registration

**Registration:** `DF-NYC-L0-PR46-COMPILER-v1`

**Parents:** `DF-NYC-HB-PR38-v1`, `DF-NYC-L0-PR42-EMPTY-v1`, `DF-NYC-L0-PR43-GEN-v1`, `DF-NYC-L0-PR44-INPUTS-v1`

**State:** method, constraints, ensemble ladder, validation, privacy boundary and failure tests registered; zero target draws, donor weights, synthetic records, building states or architecture outcomes exist

**Decision:** admit the compiler specification to implementation and independent reproduction; continue to prohibit architecture execution and public relational microdata

## Executive judgment

The New York campaign now has a falsifiable method for turning published marginal evidence into an ensemble of possible civil states. It still does not have a synthetic population.

That distinction is the center of this registration. A tract total is observed only within the limits of its source. A PUMS household is a survey donor observed at PUMA resolution, not a hidden tract household. A household–building assignment is synthetic. Medical-power need, caregiver status, exact floor, unit, address and outage operability remain `UNKNOWN` unless governed evidence later establishes them. The compiler may create structured possibilities; it may not convert possibility into observation.

The registered system preserves households, draws coherent uncertain targets, fits household and person controls together, converts continuous weights to nonnegative integer donor-class counts, assigns households only to public tract-by-structure-by-tenure capacity classes, and publishes rejection diagnostics without releasing relational records. Its candidate ensemble sizes are nested at `K = 125, 250, 500, 1,000`. The primary planning candidate is 250, but it can be selected only from input fit and convergence. The frozen `A2` and `S3` architectures, the 24,000 architecture rows and the 2,000 campaign aggregates remain unavailable to the compiler team.

This is not an analytical convenience. It specifies a new sovereign capability: a rights-preserving **civil-state production system** able to represent who needs which service, with whom, in what class of occupied place and under what uncertainty. A Department of Resilience would need such a system before impact, through disconnected operations and during recovery. It would require its own data engineering, survey science, privacy, civil-rights, local-government, field-observation and independent assurance professions.

The companion [registration workbook](../../../../models/proving/campaigns/new-york/nyc-l0-civil-state-compiler-registration.xlsx) contains the complete machine-readable method surface. Its sixteen formula-backed integrity controls pass. Workbook SHA-256 is `e75b0f24355d32de342855be98c2bc3b8e59db8949ba6d41641ab0fba0b77cdb`.

No rendering is authorized.

## The epistemic contract

The compiler has four truth states, not one blended table:

| State | Meaning | Permitted use |
| --- | --- | --- |
| observed | value and geography are supported by a registered source | constrain or validate within the source's universe and uncertainty |
| synthetic | value is generated under the registered method | scenario analysis inside controlled custody |
| unknown | required state lacks authorized evidence or an admissible generator | preserve explicitly; drive evidence collection or bounded stress cases |
| sealed | value exists in another custody domain but is inaccessible at this stage | never tune the compiler against it |

This prevents three common category errors. First, fit to published margins does not establish tract-level joint truth. Second, a synthetic record is not anonymous merely because it does not copy one source row. Third, missingness is not a negative observation. `UNKNOWN`, `NOT_APPLICABLE`, `STRUCTURAL_ZERO` and observed zero remain distinct machine states.

The campaign also keeps two population universes separate. The exact 2020 Census count of 414,234 people remains the authority for explaining outcome-blind catchment selection. The 2020–2024 ACS five-year estimates—403,320 people, 170,678 households, 170,678 occupied units, 188,061 housing units and 7,808 group-quarters residents—govern the analytic compiler. No silent rescaling between vintages is allowed. The ensemble represents uncertainty within the declared analytic universe; it does not pretend the multiyear ACS is a point-in-time incident roster.

## Why one synthetic population would be false precision

The service problem is relational. Household verification workload depends on household composition and communication access. Vertical assistance depends on a person's mobility, the household members who move with that person and the building route. Local power demand depends on devices, permissible interruption, batteries and the building circuit. Transport demand depends on whether safe service can reach the occupied place, whether the household is indivisible and whether a destination will admit it.

Published margins do not disclose those joints. A single deterministic population would hide uncertainty in target estimates, donor selection, integerization and building assignment behind one apparently precise file. It would also encourage architecture teams to tune to an accidental realization.

The registered answer is a metropolitan ensemble. Each member contains a coherent set of tract targets and household-preserving donor selections. The same member identity applies across all twelve catchments, preserving metropolitan co-variation rather than mixing independently favorable local draws. Architecture results are later paired to those fixed identities; compiler design never sees them.

## Compiler architecture

The registered pipeline has eleven controlled stages.

1. **Verify custody.** Hash every source and parent registration. A mismatch stops the run.
2. **Declare universes.** Bind analytic population, household, occupied-unit, housing-unit and group-quarters totals without substituting the selection count.
3. **Construct uncertainty.** Use ACS variance replicates where available; register alternate covariance cases where they are not.
4. **Draw coherent targets.** Generate one multilevel target vector per ensemble member, then project it to the nearest feasible nonnegative integer system under all published subtotal identities.
5. **Prepare household donors.** Join PUMS household and person records by `SERIALNO`, retain household relationships and seed fit from `WGTP` and `PWGTP`.
6. **Audit support.** Test every requested donor class. Expand only through the registered ladder—eligible local PUMAs, adjacent New York City PUMAs, then citywide—and stop if support remains absent.
7. **Fit continuous weights.** Use survey-weight-seeded iterative proportional updating with entropy regularization so household and person controls are solved together without gratuitous donor concentration.
8. **Integerize households.** Solve nonnegative integer donor-equivalence-class counts under hard identities; report objective, bound and an optimality gap no greater than 0.1 percent. Truncate–replicate–sample is a benchmark, not the primary method.
9. **Instantiate linked state.** Replicate whole donor households, issue synthetic identifiers in a separate namespace and keep group quarters distinct.
10. **Assign public building classes.** Use min-cost flow across tract × structure × tenure classes without exceeding occupied capacity. Do not assign an exact address, floor, unit or outage state.
11. **Validate and publish diagnostics.** Admit or reject members, evaluate nested convergence and release only approved aggregates, hashes and rejection logs.

The household is the replication unit because independent person draws destroy the relationships that govern care, consent, accessible movement and service delivery. The method follows the multilevel-control logic of iterative proportional updating and alternative household-selection methods while adding explicit integer feasibility, survey-weight priors, donor-support failure and custody controls ([Ye et al.](https://trid.trb.org/View/881554); [Auld and Mohammadian](https://doi.org/10.3141/2175-16); [Ma and Srinivasan](https://doi.org/10.1111/mice.12085)). Integerization is separately benchmarked against the reproducible truncate–replicate–sample method ([Lovelace and Ballas](https://doi.org/10.1016/j.compenvurbsys.2013.03.004)).

## Target uncertainty and feasible projection

Where variance replicate estimates exist, the target authority constructs covariance from the eighty published replicates:

```text
Σ = (4 / 80) × Σᵣ (θᵣ − θ)(θᵣ − θ)′
```

This retains covariance among component sums, ratios and geographic aggregates. The Census Bureau publishes eighty replicate weights in PUMS as well, while `SERIALNO` links person and housing records; `WGTP` and `PWGTP` remain distinct household and person weights ([2020–2024 ACS PUMS User Guide](https://www2.census.gov/programs-surveys/acs/tech_docs/pums/2020_2024ACS_PUMS_User_Guide.pdf)).

For tables without variance replicates, the compiler does not label an RSS approximation as known covariance. It runs preregistered alternate cases, reports sensitivity and refuses to infer zero correlation. Every sampled target vector is projected through one deterministic constrained optimization so counts are nonnegative integers and identities such as persons, households, occupied units and group quarters remain feasible. Projection distance, active constraints and rejected draws are retained as diagnostics. Silent clipping is prohibited.

## Donor geography and support

PUMS is the donor source because it preserves household–person relationships absent from published tract margins. It does not observe the selected tracts. PUMA is the smallest published PUMS geography; PUMAs contain at least 100,000 people, do not overlap and are built from nested census tracts ([Census PUMA guidance](https://www.census.gov/programs-surveys/geography/guidance/geo-areas/pumas.html); [ACS PUMS documentation](https://www.census.gov/programs-surveys/acs/microdata/documentation.html)).

Every synthetic record therefore carries its donor-support tier, never a false tract origin. A target class with zero eligible support triggers a logged pool expansion. If citywide support is still absent, the member is rejected; a structurally impossible household is not invented to make a margin close. Sensitivity reporting compares the primary pool with the broader eligible pool and records Jensen–Shannon distortion in registered PUMA-level joint tables.

## Building assignment without invented interiors

The public assignment layer ends at tract × structure × tenure class. It reconciles household demand to occupied capacity and preserves structure-type and tenure margins. It can distinguish, for example, a renter household assigned to a large multifamily capacity class from an owner household assigned to a small-building class. It cannot claim that either occupies a named building.

This limit is operationally consequential. PLUTO floors, residential units, footprints and elevator administrative records do not establish incident occupancy, emergency-power topology, elevator-bank availability, domestic-water pressure, resident-serving cooling or thermal response. Those variables stay `UNKNOWN` pending a governed building-systems observatory or representative archetype evidence. The architecture model must encounter the unknown-state case rather than receive an invented easy building.

## Nested ensemble and world pairing

The candidate ladder is fixed at 125, 250, 500 and 1,000 members. Each candidate divides the 1,000 already registered global campaign replicates exactly. Member assignment is:

```text
member = 1 + MOD(73 × (replicate − 1) + 19, K)
```

Because 73 is coprime to every candidate `K`, each member appears equally often: eight uses at `K=125`, four at `K=250`, two at `K=500` and one at `K=1,000`. The complete maps are cryptographically committed before outcomes. `K=250` is the primary planning candidate, representing about 100.83 million person-realization rows and 42.67 million household-realization rows before normalization. That scale argues for immutable base household records plus member deltas and class counts, not 250 duplicated full files.

Ensemble admission depends only on fit, variance reproduction, donor distortion, feasibility, split-half stability and convergence between `K` and `K/2`. The maximum registered changes are 0.0025 for proportions, 0.0050 for selected quantiles and 0.010 Jensen–Shannon divergence for joint diagnostics. Failure escalates `K`; failure at 1,000 stops the compiler. No architecture score can justify a different ensemble size.

## Validation is broader than marginal fit

Twenty registered checks cover five different questions:

- **identity:** do all person, household, group-quarter, occupancy and capacity equations close exactly?
- **fit:** do controlled margins fall within source-aware tolerances without impossible donor distortion?
- **generalization:** do externally selected, withheld cross-tabs pass thresholds frozen by a separate custodian?
- **stability:** do the mean, tails, joints, donor concentration and feasibility stabilize as `K` grows?
- **reproduction:** does an independent implementation recover the registered counts, hashes and diagnostics?

The donor-distortion limit is not a claim of tract truth. The holdout custodian—not the compiler operator—chooses and salts the unexposed validation tables and freezes their thresholds before access. A failure rejects the member or registration; it is not an invitation to tune against the holdout.

Eighteen deliberate injections require the implementation to fail closed. They include contradictory subtotals, negative draws, structural zero support, PUMA-to-tract leakage, household splitting, donor monopoly, solver timeout, building shortage, unknown-state coercion, vintage substitution, holdout leakage, architecture leakage, privacy attack and independent reproduction mismatch.

## Privacy, release and civil custody

Synthetic data does not automatically provide a formal privacy guarantee. NIST warns that synthetic data without a differential-privacy mechanism offers only informal protection, and empirical work shows that inference risk and privacy–utility tradeoffs can remain difficult to predict ([NIST SP 800-226](https://doi.org/10.6028/NIST.SP.800-226); [Stadler, Oprisanu and Troncoso](https://www.usenix.org/conference/usenixsecurity22/presentation/stadler)). This registration therefore sets neither epsilon nor delta. Those parameters would express a social and legal privacy decision, not a spreadsheet tuning choice.

Public release is limited to method, sources, cryptographic commitments, aggregate diagnostics and rejection logs. Relational person, household and building-class records remain in a controlled research enclave. Exact location and protected operational state are outside public research custody. Membership inference, attribute inference, nearest-neighbor disclosure, rare-household uniqueness, auxiliary linkage and aggregate-query leakage all require adversarial testing before any broader release.

Authority is separated among source custodian, target authority, compiler operator, privacy and civil-rights authority, independent reproducer, holdout custodian and architecture operator. The compiler operator cannot see holdout content or architecture outcomes. The architecture operator receives only an approved aggregate demand interface after formal `L0`, never protected donor records or exact household location.

## What this means for the Department of Resilience

The mature capability is not a national list of vulnerable people. It is a federated public infrastructure for producing the minimum civil state needed for a declared mission, under local authority, with explicit expiration and auditable purpose limitation.

That infrastructure would combine:

- continuously maintained statistical and building-state standards;
- protected local source custody and disconnected field reconciliation;
- rapid survey and observation teams for states public records cannot establish;
- privacy-preserving linkage, uncertainty ensembles and machine-readable provenance;
- interfaces that deliver workload and service requirements without unnecessary identity;
- independent civil-rights, disability, statistical and security authorities; and
- a proving program that attacks both operational usefulness and disclosure risk.

Military force projection invests heavily in intelligence preparation, operational pictures, mission data, simulation and command systems because platforms without state knowledge cannot create controlled effects. A coequal resilience force needs an analogous investment, but its legitimacy depends on minimizing coercion and surveillance while preserving household agency. That is a first-principles technology program in its own right.

## What closes and what remains open

This pass closes the operator-side method registration. The workbook binds 28 hard constraints, 20 validation rules, 18 deliberate failure tests, 20 schema fields, four nested pairing maps and twelve empty output objects. Its principal commitments are:

| Object | SHA-256 |
| --- | --- |
| specification | `17fe27f1c3e7c1a1813b03e6797037e10bba88d8dec93ce2dc3136efd26aa86b` |
| constraints | `3fe2de071aba4e07d0b625a11e56efc91d4d65823b1b3b43fa97f727ddced871` |
| validation rules | `d3492da9d54145c15effed39b9d21386746b94105940bb05a19082cfcb5f2f6f` |
| failure tests | `b53db83134d3511d032e30ce2e067f004211dd72a49f75be248654c73308a948` |
| state schema | `6501c4fc57a843b23add5c42b56ad0d2bcc429d5f9adcb892b2ea549f4ef9eca` |
| complete registration | `1e38c1dbeb96dd816641b0da0dfa554fb8a1713b71e5149285094c9525d8d5b3` |

No generated state exists. The subsequent [PUMS donor custody and support audit](l0-pums-donor-support-audit.md) completes official source acquisition, exact verification, relational checks and the empirical local → adjacent → citywide support ladder without generating a target. The next gate is the coherent target engine and tier-labeled hierarchical fit, followed by implementation and independent reproduction of the public-class compiler. Formal `L0` still requires external salted holdout custody, operational building and medical-power evidence or bounded unknown-state treatment approved for the test, service-territory authority, causal feasibility, alternative dependence cases and independent reconstruction of the earlier New York lineage.

The pass does not close any `NCAC` evidence gate. It does not validate `A2`, `S3`, a national formation, a procurement quantity or an incident registry. Its value is narrower and foundational: it makes the next synthetic artifact capable of being rejected before that artifact can shape the answer.
