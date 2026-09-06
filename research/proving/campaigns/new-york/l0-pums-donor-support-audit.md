# New York `L0` PUMS donor custody and support audit

**Registration:** `DF-NYC-L0-PR48-DONORS-v1`  
**Parent:** `DF-NYC-L0-PR46-COMPILER-v1`  
**State:** `SOURCE_CUSTODY_AND_SUPPORT_AUDIT_NO_SYNTHESIS`  
**Access date:** 5 September 2026  
**Workbook:** [NYC `L0` PUMS donor support audit](../../../../models/proving/campaigns/new-york/nyc-l0-pums-donor-support-audit.xlsx)  
**Workbook SHA-256:** `473c47b41ccb9d27e4642c3a25e17fce6b2030bcaff5a61210c55d083fac9fb9`

## Decision

The official 2020–2024 ACS Public Use Microdata Sample can support the registered household-preserving civil-state compiler, but it cannot observe a selected tract, catchment or building. The donor system must therefore expose a three-tier support ladder—local PUMA, geometrically adjacent New York City PUMAs and citywide remainder—and use hierarchical partial pooling or regularization when the narrower pool is weak. Borrowed donors must retain their support-tier label. They cannot be described as local evidence.

This pass establishes source custody, exact reproduction, household–person linkage integrity, public-use geography, donor-class sparsity and support diagnostics. It does not fit tract targets, generate continuous or integer donor weights, instantiate synthetic households, assign buildings, infer incident operability or execute either architecture. All registered output tables for those acts remain empty.

## Research question

The compiler registration made a methodological promise: preserve whole households; seed household and person controls with the correct survey weights; treat PUMA as donor support rather than tract observation; expose rare-cell, privacy and convergence problems; and separate group quarters from household synthesis. Before implementation, this pass asks whether the acquired New York files and selected catchment geography can actually sustain that promise.

The audit tests four propositions:

1. the acquired person and housing files are the intended official five-year release and reproduce Census verification totals exactly;
2. `SERIALNO` and `SPORDER` support a lossless, nonduplicated household–person relation for the New York City donor universe;
3. the public-use geography can be mapped to the selected tracts without claiming tract-level observation; and
4. the registered nine-dimensional household-class surface has enough empirical support to justify implementation without silent rare-class deletion or uncontrolled donor concentration.

## Frozen source custody

The operator acquired the official New York housing and person archives from the Census Bureau's [2024 five-year PUMS directory](https://www2.census.gov/programs-surveys/acs/data/pums/2024/5-Year/), the [2020–2024 PUMS User Guide](https://www2.census.gov/programs-surveys/acs/tech_docs/pums/2020_2024ACS_PUMS_User_Guide.pdf), the official data dictionary, PUMS verification estimates and unweighted record counts, the Census tract-to-2020-PUMA relationship file and the New York 2020 PUMA geometry. The workbook records the URL, byte size and SHA-256 digest for every committed source object. Raw microdata and record identifiers are not released into the repository.

The Census documentation defines separate housing-unit and person files joined by `SERIALNO`, with `WGTP` as the housing/household weight and `PWGTP` as the person weight. It also states that vacant units have no person records, group-quarters placeholders in the housing file carry zero weights, and PUMA is the lowest geography available in PUMS. The [PUMA program page](https://www.census.gov/programs-surveys/geography/guidance/geo-areas/pumas.html) describes PUMAs as non-overlapping state partitions built from census tracts and designed to contain at least 100,000 people. That makes PUMA suitable for bounded donor support and unsuitable as evidence that a public-use household occupied any particular tract.

The source-reproduction controls close exactly:

| Official New York control | Computed | Official | Difference |
| --- | ---: | ---: | ---: |
| housing-file records | 481,692 | 481,692 | 0 |
| person-file records | 984,474 | 984,474 | 0 |
| weighted total population | 19,852,366 | 19,852,366 | 0 |
| weighted housing-unit population | 19,227,424 | 19,227,424 | 0 |
| weighted group-quarters population | 624,942 | 624,942 | 0 |

Exact agreement establishes acquisition and interpretation fidelity against the published PUMS verification files. It does not make PUMS estimates equal to tabulated ACS estimates, convert a five-percent sample into a census or validate the campaign's unobserved joint state. Census explicitly warns that PUMS verification estimates may differ from published ACS tables because of sampling, weighting, confidentiality edits and the different production process.

## Relational integrity

The New York City donor universe contains 154,349 housing-file records and 326,729 person records. The linkage audit finds 144,611 unique person-file `SERIALNO` values, no duplicate housing serials, no duplicate `SERIALNO`–`SPORDER` person pairs, no serial spanning PUMAs and no housing–person PUMA mismatch.

Exactly 9,738 housing records have no person row. That count is identical to the number of vacant housing units. No occupied household or group-quarters placeholder is missing a person relation, and the person counts within every occupied household and group-quarters record reconcile to the housing-file `NP` field. This closes the relational acquisition check and preserves the ability to instantiate complete donor households later.

Group quarters remain a separate synthesis path. The New York City housing-file group-quarters placeholders number 21,148 and their `WGTP` sum is zero, while person-file `PWGTP` yields 213,616 weighted group-quarters residents. Any implementation that estimates group-quarters population from housing-file weights would erase the population by construction. The household compiler may use group-quarters placeholders for structural linkage, but group-quarters people, facilities, custody and service needs require their own evidence and controls.

## Donor geography

The official tract-to-PUMA relationship places the 87 registered reference tracts inside seventeen 2020 PUMAs. The New York City donor universe contains 55 PUMAs. The audit constructs adjacency from the official PUMA polygons using geometric contact, solely to define a reproducible donor-support expansion. It does not treat PUMA adjacency as street access, service territory, social similarity or incident traversability.

For each of the twelve catchments, the support ladder is:

- **local:** the PUMA or PUMAs containing the catchment's selected tracts;
- **adjacent:** all other New York City PUMAs touching at least one local PUMA; and
- **citywide remainder:** every other New York City PUMA.

This ordering is a prior over donor relevance, not a claim that the first tier is sufficient. Each synthetic household must retain the tier from which its donor evidence was borrowed. Fit and disclosure diagnostics must be reported by tier, class and catchment.

## Joint-class support

The preregistered audit classifies occupied households jointly on nine dimensions that matter to continuity operations and are present or constructible in public PUMS: household size, public structure class, tenure, vehicles, limited-English status, presence of a person under eighteen, count of older adults, any disability and ambulatory difficulty. The citywide file contains 2,123 observed joint classes among 123,463 occupied donor households representing 3,334,093 weighted households.

The support distribution is sharply unequal:

| Raw donors per class | Classes | Raw households | Weighted households | Weighted share |
| --- | ---: | ---: | ---: | ---: |
| 1 | 346 | 346 | 8,252 | 0.25% |
| 2–4 | 452 | 1,243 | 30,308 | 0.91% |
| 5–19 | 620 | 6,331 | 160,380 | 4.81% |
| 20 or more | 705 | 115,543 | 3,135,153 | 94.03% |

Classes with fewer than five donors account for 37.59 percent of observed classes but only 1.16 percent of weighted households. That combination is easy to mishandle. The small aggregate mass could tempt an operator to drop or generalize rare classes; the large share of the class surface means doing so would disproportionately erase unusual household combinations, weaken tail fidelity and conceal privacy and convergence failures.

Rare cells therefore remain explicit. The later compiler must diagnose donor monopoly, effective sample size, maximum weight share, split-half stability, target conflict and disclosure risk. Generalization rules, if any are admitted by the privacy and statistical authorities, must be declared before architecture outcomes and must preserve an auditable path back to the unsupported class.

## Local support is not uniform

Raw occupied-household counts in the twelve local pools range from 1,446 to 4,643. More consequentially, the local pool represents as little as 71.36 percent of citywide weighted class mass when support is measured against classes available in that pool. Adding touching PUMAs raises the worst catchment to 89.66 percent but still leaves some classes supported only by the citywide remainder.

The two limiting cases make the design consequence visible:

| Catchment | Local occupied donors | Local class-mass support | Local plus adjacent support |
| --- | ---: | ---: | ---: |
| `NYC-V1-R03` | 2,966 | 71.36% | 93.88% |
| `NYC-V1-R02` | 2,667 | 73.82% | 89.66% |

These percentages are support diagnostics, not goodness-of-fit measures and not estimates of how much a catchment resembles its PUMA. A class is counted as supported when at least one donor with that joint signature exists in the tier; the calculation weights classes by their citywide PUMS household mass. Target fitting may reveal stricter or different gaps.

The evidence rejects two simple implementations. A local-only solver would manufacture structural zeros where relevant household classes are absent by sample chance. An unconstrained citywide solver could converge numerically while disguising how much nonlocal information generated the catchment. The admissible approach is hierarchical: begin with local evidence, expand visibly to adjacent and citywide support, regularize sparse cells, report tier use and reject any solution whose donor concentration, fit or stability exceeds preregistered limits. Partial pooling is a model choice; it does not turn the borrowed household into a tract observation.

## Privacy and controlled custody

PUMS is public-use microdata, but the constructed linkage and class diagnostics still create governance obligations. Raw person and housing records, `SERIALNO`, `SPORDER` and record-level derived classes remain in controlled processing. The repository releases only source commitments, aggregate counts, class bands, support metrics, linkage anomalies and zero-output confirmations. No donor row, reconstructed household or row-level synthetic state is included.

The presence of 346 singleton joint classes also reinforces the compiler registration's privacy boundary. “Synthetic” is not a disclosure control. The privacy authority must evaluate membership inference, attribute inference, nearest-neighbor similarity, rare-household uniqueness, query leakage and the utility cost of any formal mechanism before public relational release. The correct response to rare support is not silent deletion after seeing an architecture result.

## Institutional consequence

This audit changes the Department of Resilience concept in a small but fundamental way. Civil-state production is not a dashboard function. It is a standing national capability for reconciling statistical evidence, protected local records, building and utility state and field observations under disconnection—while preserving provenance, uncertainty, household relationships, purpose limits and rights.

That capability needs its own profession, secure computation environments, local custody agreements, interoperable schemas, disconnected reconciliation, independent statistical reproduction, privacy red teams and field-operable interfaces. The military analogy is mission-data infrastructure, not centralized omniscience. The civil objective is the minimum trustworthy state required to deliver water, cooling, medical power, access, movement and lawful household disposition. The force must be able to say what it knows, what it modeled, where it borrowed support and what remains unknown.

## What this pass closes

- official source acquisition and cryptographic custody for the New York PUMS donor surface;
- exact reproduction of two unweighted record counts and three weighted population controls;
- household–person relational integrity for occupied households, vacancies and group quarters;
- the tract-to-PUMA mapping and a reproducible local–adjacent–citywide support ladder;
- empirical size and sparsity of the registered nine-dimensional household-class surface; and
- aggregate-only release with all target, synthesis, building-assignment and architecture outputs preserved at zero.

## What remains open

The coherent target engine has not drawn a target. No continuous weights or integer household counts exist. The compiler has not been subjected to the eighteen registered failure injections, privacy attacks, ensemble-convergence tests or independent reproduction. Public building-class capacity assignment remains unimplemented. Medical-power need, caregiver relation, exact household–building binding, floor, elevator and water-pump operability, indoor thermal state and live service status remain `UNKNOWN`. Borough remains an unapproved service-territory proxy, alternate dependence cases and causal-feasibility rules remain open, and external salted holdout custody does not exist.

The next admissible pass is therefore the target engine and hierarchical donor fit—not an architecture run. It must preserve the registered zero-output boundary until target coherence, tier-labeled support, sparse-cell behavior, privacy and reproduction gates have been evaluated. No `NCAC` evidence gate advances and no rendering is authorized.
