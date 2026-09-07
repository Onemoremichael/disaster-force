# New York `L0` atomic-basis registration

**Registration:** `DF-NYC-L0-PR52-ATOMIC-BASIS-v3B0`

**Decision:** the published catchment point vectors are feasible on an explicit nonnegative integer support, but they do not identify the latent civil state and do not authorize a stochastic target ensemble.

**Paired model:** [New York `L0` atomic-basis registration](../../../../models/proving/campaigns/new-york/nyc-l0-atomic-basis-registration.xlsx)

**Successor note:** [Pass 53](l0-atomic-moment-cone-audit.md) adds the authoritative under-five margin but rejects the proposed exact moment-calibration objective. Seven zero-point, positive-SE margins cannot be the mean and variance of any nonnegative state distribution. Official covariance remains authoritative in a measurement likelihood.

## Executive judgment

Pass 51 established that the official covariance blocks, all registered marginal standard errors and six exact additive identities can coexist. It also showed why that was insufficient: a Gaussian distribution with those linear moments repeatedly left the nonlinear civil-state region. Pass 52 asks the logically prior question that the Gaussian construction had concealed: **what primitive nonnegative objects are allowed to exist, and how must the published margins be derived from them?**

The answer is a factorized atomic basis with three ledgers per catchment: 596 person cells, 960 occupied household-unit cells and one vacant-unit cell. Every one of the 456 published catchment margins is reconstructed exactly by a nonnegative integer witness. The aggregation matrix has 1,557 columns but rank only 32, leaving a nullity of 1,525. Point feasibility is therefore established; population reconstruction is not.

That distinction is operationally decisive. None of nine tested joint quantities is point-identified in any of the twelve catchments. Plausible allocations can differ by thousands of people or households while producing exactly the same published margins. Selecting one sparse feasibility witness would silently decide who needs cooling, medical power, contact, accessible movement or building support before either `A2` or `S3` is tested.

No target ensemble, donor fit, synthetic record, building assignment or architecture outcome is admitted. The next method, `v3B1`, must calibrate a distribution over feasible atomic states to the Pass 51 mean and covariance authority, explicitly bound unidentified dependence, and add an authoritative under-five partition before age-valid disability patterns can be sampled.

## 1. Why the support must precede the stochastic law

An aggregate target vector can satisfy familiar totals and subset inequalities while still describing no possible population. The reason is semantic: published tables report overlapping projections of an unobserved joint state. “Any disability” is a union of age-valid difficulty patterns, not an independent count. A one-person household with an older adult is an intersection, not a freely drawn margin. A household living alone cannot also contain a child. Vacant units have no occupied tenure, heating or structure attributes. These facts belong in the state space, not in a repair step applied after sampling.

The registered basis therefore changes the generative order:

```text
ALLOWED PERSON + HOUSEHOLD-UNIT ATOMS
                 │
                 ▼
NONNEGATIVE INTEGER CELL COUNTS
                 │
                 ▼
PUBLISHED MARGINS BY FIXED AGGREGATION
                 │
                 ▼
MOMENT AND CEILING TESTS
```

This architecture does not claim that the atoms are observed. It establishes the lawful support on which a future probability distribution may be defined.

## 2. Factorized civil-state architecture

### 2.1 Person ledger

The person basis crosses six age bands—`0–4`, `5–17`, `18–64`, `65–74`, `75–84` and `85+`—with the civilian-noninstitutionalized universe, group-quarters status and age-valid disability patterns.

Disability patterns are structurally restricted:

- ages `0–4` permit hearing and vision difficulty only;
- ages `5–17` permit hearing, vision, cognitive, ambulatory and self-care difficulty;
- ages `18+` permit all six registered difficulties, including independent living;
- atoms outside the civilian-noninstitutionalized universe carry no disability classification; and
- every disabled atom contains at least one age-valid difficulty.

The 596 cells aggregate to total population, age margins, civilian-noninstitutionalized population, group-quarters population, any disability, disability by age and the six difficulty margins.

### 2.2 Occupied household-unit ledger

The occupied ledger crosses family status, living alone, child presence, older-adult presence, vehicle access, limited-English status, electric heat, tenure and six structure classes. Living-alone atoms are nonfamily and cannot contain a child. The age-65 one-person margin is derived as `living alone AND age 65 present`; it is not independently assigned. Every occupied household atom contributes one household, one occupied housing unit and one total housing unit.

The resulting 960 occupied cells aggregate to the registered household, tenure, structure, vehicle, language and heating margins. A separate vacant-unit atom contributes only to total and vacant housing units because occupied attributes are outside its statistical universe.

### 2.3 Cross-ledger bridges

The factorization avoids pretending that public margins identify person-to-household records. Three necessary capacity bridges are nevertheless enforced:

1. minimum implied household occupants cannot exceed the non-group-quarters population;
2. households with children cannot exceed the non-group-quarters population under eighteen; and
3. households with an older adult cannot exceed the non-group-quarters population age 65 or older.

These are necessary conditions, not a reconstructed relational population. Household membership, caregiving and building assignment remain outside the public basis.

## 3. Aggregation geometry and exact feasibility

Let `x_c` be the 1,557-cell nonnegative integer vector for catchment `c`, and let `A` be the fixed 38-by-1,557 aggregation operator. The point-feasibility problem is:

```text
find x_c ∈ Z⁺¹⁵⁵⁷ such that A x_c = y_c and B x_c ≤ 0,
```

where `y_c` is the published 38-margin vector and `B` contains the three cross-ledger bridges.

The operator rank is 32. Six published additive identities reduce the 38 reported directions to 32 independent ones, leaving 1,525 invisible directions in the atomic state. All twelve catchments have an exact integer witness. Maximum reconstruction residual is zero across all 456 margin checks. Minimum bridge slack is nonnegative in every catchment.

The witnesses are deliberately not interpreted as estimates. A zero-objective feasibility solver returns sparse extreme points: only 16–22 person cells and 16–20 household cells are nonzero in each catchment. That sparsity is a property of linear-program geometry, not evidence that the real population occupies so few joint states.

## 4. The aggregate rulebook was incomplete

The atomic basis implies restrictions that were absent from the 33 Pass 51 aggregate checks:

- the sum of the six difficulty margins must be at least the any-disability total;
- independent-living difficulty cannot exceed disability among adults;
- living-alone and child-present households are disjoint; and
- the observed age-65 one-person count must satisfy the lower bound implied by living-alone and age-65-present household margins.

All 48 catchment-by-rule checks pass. Four adversarial vectors were then constructed so that each satisfies all 33 parent equalities and inequalities but violates one of these atomic consequences. Each is correctly rejected on the registered support. This is not merely a stronger error screen. It demonstrates that semantic exclusions must be generated from the basis itself; a hand-maintained aggregate checklist will otherwise remain incomplete.

## 5. Feasibility is not identification

For each catchment, linear programs minimize and maximize nine latent joint quantities over the complete feasible polytope. All 108 intervals are valid; none collapses to a point.

| Latent joint quantity | Largest feasible maximum | Median bound width | Largest bound width |
| --- | ---: | ---: | ---: |
| people age `0–4` | 10,108 | 7,090 | 10,108 |
| group-quarters population under 18 | 1,686 | 501 | 1,686 |
| disabled people age `0–4` | 1,281 | 343.5 | 1,281 |
| civilian-noninstitutionalized group-quarters population | 1,686 | 64 | 810 |
| households with both a child and an older adult | 3,428 | 2,374.5 | 3,428 |
| households with both no vehicle and limited English | 6,661 | 1,740 | 5,096 |
| renter-occupied units in structures with 50+ units | 10,685 | 3,122 | 6,676 |
| family households with children | 4,875 | 743.5 | 2,628 |
| electric-heat households in structures with 50+ units | 5,818 | 1,816 | 5,303 |

These are continuous linear-relaxation bounds. They are conservative diagnostics of what the margins fail to identify, not posterior intervals and not forecasts. The widths reveal where additional evidence could most change force requirements: vertical-building heating and tenure, overlapping mobility and language constraints, intergenerational households, institutional settings and the under-five population.

## 6. The under-five authority gap

The current target surface publishes one under-eighteen total, while the disability universe changes at age five. The atomic basis can allocate the under-eighteen population between `0–4` and `5–17`, but the result is not identified by the registered margins. The component cells needed to derive that split exist in ACS table `B01001`; they were not registered as target authority in Pass 44.

`v3B1` must add the split explicitly and carry its official variance-replicate covariance with the existing age margins. It may not infer the split from a feasibility witness, a national ratio or donor records. This is a small statistical-table addition with a large semantic consequence: without it, the generator cannot lawfully distinguish disability patterns for young children from those for school-age children.

## 7. Registered successor: distribution over feasible states

The next implementation must choose and preregister a stochastic calibration method over `x`, not over independently sampled aggregate margins. Candidate methods include constrained maximum entropy, moment-constrained transport and generalized method-of-moments calibration over feasible atomic draws. Method choice remains open because it determines how unidentified dependence is regularized.

Whichever method is selected must:

1. preserve every official within-table covariance block and registered marginal standard error from Pass 51;
2. generate only nonnegative states satisfying the atomic support and bridges;
3. disclose which dependence directions are identified, externally informed, bounded or regularized;
4. report partial-identification and minimum-conflict surfaces rather than choosing one convenient joint state;
5. retain the nested `K=125–1,000` prefixes and all center, spread, tail, repair-distance and integrity gates;
6. pass the four new semantic contradictions and all inherited failure injections; and
7. stop before donor fitting if no ensemble clears the ceiling.

The factorized basis is not a substitute for protected relational evidence. A later household-preserving donor fit may distribute mass within the feasible surface, but it must label local, adjacent and citywide support and cannot convert a donor into a known resident of a tract or building.

## 8. Institutional consequence

A mature Department of Resilience requires a **Civil State Authority** with responsibilities analogous to a mapping agency, statistical office, intelligence production system and public-rights regulator—but designed for service continuity rather than surveillance. Its core products would include:

- versioned semantic registries for people, households, buildings, utilities and services;
- machine-checkable aggregation operators and structural-zero rules;
- automated support and facet compilation from those semantics;
- partial-identification reports attached to operational demand estimates;
- protected relational fusion under explicit purpose, access, retention and disclosure controls;
- disconnected local reconciliation and auditable field updates; and
- independent reproduction, cryptographic commitments and revocable operational attestations.

The authority would not exist to create a perfect national population file. It would make uncertainty and missing relationships visible enough that the force does not confuse an optimization artifact with a person, household or building. That capability is itself force infrastructure: it governs how cooling, water, medical-power, contact, transport and reception capacity are sized and routed under damaged communications.

## 9. Decision boundary

Pass 52 establishes three claims and no more:

1. the registered point margins admit exact nonnegative integer representation on the factorized support;
2. the atomic semantics expose valid constraints that the aggregate rulebook missed; and
3. the published margins do not identify operationally important joint state.

It does not admit a probability distribution, donor weights, synthetic people or households, building occupancy, operational building state, demand, architecture performance or campaign outcomes. Formal `L0`, every `NCAC` evidence gate and all renderings remain closed.

The workbook records the full person and household bases, aggregation map, integer witnesses, exact reconstructions, implied constraints, adversarial failures, identification bounds, empty downstream tables and formula-backed integrity controls. All 21 sheets passed visual inspection; the formula-error scan is empty; the Open XML archive validates. Workbook SHA-256 is `8e488633ef63b8b0dc09f4f694aa01474bf7d32beea55436dbcab12b436c22ba`.
