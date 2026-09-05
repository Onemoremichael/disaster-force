# New York `L0` catchment rehearsal and evidence-surface audit

**Run:** `DF-NYC-L0-PR39-v1`

**Parent protocol:** `DF-NYC-HB-PR38-v1`

**Status:** outcome-blind operator rehearsal; formal `L0` remains open

**Decision:** retain twelve provisional references and three rehearsal commitments for independent reproduction; do not generate `A2` or `S3` outcomes

## Executive judgment

The first New York selection run demonstrates that a serious resilience force cannot begin a metropolitan test by pointing to twelve convenient neighborhoods. It must first build a governed evidence surface, define the population unit, turn built form into falsifiable strata, expose every exclusion and missing join, and commit to a selection order before either architecture produces a result.

That operator run is now complete. Seven official source extracts produce 2,325 land-tract records, 2,222 candidate-eligible residential tracts and 844 unique contiguous catchments within the protocol's 32,000–38,000-person envelope. The frozen covariate rules yield 80 tower-intensive candidates, 170 mid-rise heat-burden candidates and 25 campus/service-friction candidates. Deterministic hash ordering, cross-archetype non-overlap and a two-borough minimum produce twelve disclosed provisional references containing 87 distinct tracts and 414,234 people. Three additional compositions are withheld behind published SHA-256 commitments.

Those results are not a closed `L0`. The run found four reasons to refuse formal freeze.

First, the protocol required a connected local-street component, while this run can establish only polygon adjacency among census tracts. Second, the public holdout universe and deterministic unsalted procedure make each withheld composition inferable; a hash proves later consistency but does not create secrecy. Third, the 2024 ACS API required a key at retrieval, so age and disability remain explicitly unmeasured rather than being replaced with zeros. Fourth, independent reproduction—including a separately implemented candidate builder and an empty outcome-table audit—has not occurred.

The correct result is therefore neither “selection failed” nor “the catchments are final.” The result is a useful pre-outcome rehearsal that fixes the operator's implementation, reveals the evidence cliffs and hands an independent team a complete candidate universe to challenge. No `A2` or `S3` performance outcome should be generated until that challenge is complete.

## What `L0` is for

`L0` is not a clerical preface to the interesting experiment. It is the control against geographic overfit.

A resilience formation can appear successful because a study boundary omits difficult buildings, counts nominal facilities as working destinations, treats administrative device records as installed capacity, assumes a road connection from polygon proximity, or defines the test population after seeing where the architecture performs well. Each error is capable of moving more apparent performance than the technology being evaluated. Catchment construction is therefore part of the experiment's causal design.

The parent [vertical heat-blackout protocol](new-york-vertical-heat-blackout-replication-protocol.md) required source freezing, outcome-blind selection, three mechanistic built-form strata, four non-overlapping references per stratum and one sealed holdout. The [full-mission test program](../test-enterprise/ncac-full-mission-test-program.md) further required an independent team to reproduce the catchments, design matrix and empty outcome tables before `L0` closes. This pass performs the first operator build and audits the distance between that build and the registered requirement.

The governing prohibition is simple: **architecture outcomes cannot repair a selection defect**. A defect found now can be corrected under a public amendment. The same correction after `A2` and `S3` results exist would create an opportunity to select a more favorable city.

## Frozen evidence surface

The run uses official public records retrieved on September 5, 2026. The workbook preserves the exact row count, byte count, source-file SHA-256, available metadata hash, retrieval timestamp, reconstructable query and inferential boundary for every extract.

| Evidence layer | Role in the rehearsal | Boundary that remains |
| --- | --- | --- |
| [NYC DCP 2020 Census Tracts 26b](https://data.cityofnewyork.us/City-Government/2020-Census-Tracts/63ge-mke6) | land-tract geometry, borough and neighborhood labels | geometry is modified for the city base map; polygon contact is not a street route |
| [2020 Census TIGERweb tract layer](https://tigerweb.geo.census.gov/arcgis/rest/services/TIGERweb/tigerWMS_Census2020/MapServer/6) | exact `POP100` population and `HU100` housing-unit denominator | 2020 count is not 2026 population or incident occupancy |
| [NYC PLUTO](https://data.cityofnewyork.us/City-Government/Primary-Land-Use-Tax-Lot-Output-Map-MapPLUTO-/64uk-42ks) | residential units, floors, lot and building count, postcode | tax-lot administration is not occupancy, access or operability |
| [NYC Building Footprints](https://data.cityofnewyork.us/City-Government/BUILDING/5zhs-2jue/about_data) | constructed footprint count and roof-height join by BBL | exterior geometry does not describe interior circulation or usable refuge |
| [NYC Heat Vulnerability Index](https://data.cityofnewyork.us/Health/Heat-Vulnerability-Index-Rankings/4mhf-duep) | pre-outcome heat-burden stratum transferred through postcode | ZCTA planning index is not person-level risk or a thermal dose model |
| [NYC elevator safety compliance](https://data.cityofnewyork.us/Housing-Development/DOB-NOW-Elevator-Safety-Compliance/e5aq-a4j2) | latest administrative status for elevator and accessibility-lift devices, joined by BBL | record status is not incident availability; the join is incomplete |
| [NYC Facilities Database](https://data.cityofnewyork.us/City-Government/Facilities-Database/ji82-xba5/data) | straight-line distance to selected public education, health and human-service facility groups | presence is not opening, cooling, accessibility, capacity or admission |

The data discipline matters most where acquisition failed. The requested 2024 ACS tract calls returned a missing-key response. The run did not substitute a modeled demographic profile, infer disability from building type or equate a missing count with zero. It instead uses exact decennial population for catchment size and leaves civilian noninstitutionalized population, disability and age 65+ blank. None affects eligibility, ordering or selection. They remain required enrichments before synthetic household generation.

Coverage is high for some joins and weak for others. Of 3,734,341 PLUTO residential units, 99.97 percent receive an HVI postcode match and 98.05 percent receive a positive joined roof height. Only 62,982 of 120,187 latest elevator records—52.4 percent—join through a PLUTO BBL to the tract surface. That device measure remains useful for broad stratification, but it cannot support a claim that a catchment contains a known number of working elevators.

## Canonical operator implementation

The operator method is now stated at enough precision to reproduce or reject it.

1. Start with the 2,325 DCP land tracts. Join 2020 `POP100` by eleven-digit GEOID.
2. Retain a tract as candidate-eligible only when population is positive, PLUTO reports positive residential units and the tract polygon touches at least one other eligible polygon. This last condition is a rehearsal proxy, not the protocol's street-component test.
3. Project centroids to New York Long Island State Plane feet (`EPSG:2263`). For each eligible seed tract, repeatedly add the frontier tract whose centroid is nearest to the current population-weighted centroid. An exact-distance tie breaks by ascending GEOID.
4. Stop when population first reaches 32,000. Retain the group only if it does not exceed 38,000. Canonicalize the group as ascending GEOIDs joined by the ASCII pipe character and deduplicate identical sets.
5. Compute candidate-level population-weighted and residential-unit-weighted covariates. Do not impute missing disability, age, roof or HVI values.
6. Compute the selection hash as SHA-256 of `canonical_GEOID_set|DF-NYC-HB-PR38-v1`. Order ascending by that hash.
7. Apply the three archetype rules. Process `V1`, then `V2`, then `V3`; within each, take the first five candidates that share no tract with an earlier selection, prevent any primary borough from supplying more than three of five and require the second selection to introduce a second borough. The first four are disclosed references and the fifth is a rehearsal holdout.

This implementation resolves ambiguities that the parent prose did not fully specify: how the frontier grows, how equal distances break, how a GEOID set is serialized, how candidates eligible for two archetypes are assigned and how borough balance interacts with hash order. Because these choices can change the named catchments, they must be independently reviewed and incorporated into a registered protocol amendment before formal freeze.

The implementation uses Python 3.10.12, NumPy 1.26.4, pandas 1.5.3, Shapely 2.1.2 and pyproj 3.7.1. Exact versions and lineage appear in the workbook. The repository remains Markdown-only except for models, so formal `L0` also requires either a permitted sealed code escrow or a second implementation against this canonical specification.

## Candidate universe and archetype rules

The 2,222 eligible tracts produce 844 unique groups, or 38.0 percent as many groups as seeds after invalid overshoots and duplicate sets are removed. Candidate construction itself therefore has substantial selection power: most seeds do not create a distinct retained catchment.

The thresholds are computed from the complete 844-candidate universe.

| Archetype | Frozen rehearsal rule | Threshold | Eligible candidates |
| --- | --- | ---: | ---: |
| `V1` tower-intensive | mean floors at or above P80; active relevant device records per 1,000 people at or above P80; density at or above P75 | 8.519 floors; 7.685 records/1,000; 75,883 people/sq mi | 80 |
| `V2` mid-rise heat burden | at least 50 percent of residential units in three-to-eight-floor lots; HVI 4–5 unit share at or above P75 | 50 percent; 100 percent HVI 4–5 share | 170 |
| `V3` campus/service friction | units on lots with at least three buildings at or above P75; device records at or above P60; public-facility distance at or above median | 14.29 percent; 4.936 records/1,000; 0.159 straight-line mi | 25 |

The pools are not citywide categories. Of the 844 groups, 578 satisfy no rule, 257 satisfy exactly one and nine satisfy two. None satisfies all three. Overlap is desirable evidence: Parkchester can be both vertically demanding and campus-like, while an East Harlem group can be tower-intensive and high-HVI. The test should preserve those mechanisms rather than force every place into a single descriptive label.

The geography is uneven. Seventy-five of the 80 `V1` candidates have Manhattan as their primary borough, with three in Queens and two in Brooklyn. The `V2` pool is concentrated in Brooklyn and the Bronx but includes Manhattan and Queens. The `V3` pool is small—thirteen Queens, five Brooklyn, four Bronx and three Manhattan candidates. The balance constraint prevents a five-site single-borough result; it does not manufacture representativeness where the frozen covariates do not provide it.

## Provisional reference set

The hash-order rehearsal yields the following disclosed set. Population is the 2020 Census denominator; values are selection covariates, not post-event measurements.

| ID | Primary geography | Pop. | Tracts | Mean floors | Device records/1k | HVI 4–5 unit share | Campus unit share |
| --- | --- | ---: | ---: | ---: | ---: | ---: | ---: |
| `NYC-V1-R01` | Flushing–Willets Point, Queens | 34,306 | 6 | 8.59 | 8.22 | 100.0% | 6.6% |
| `NYC-V1-R02` | Upper West Side–Manhattan Valley | 32,165 | 4 | 13.45 | 13.59 | 0.0% | 0.8% |
| `NYC-V1-R03` | Murray Hill–Kips Bay, Manhattan | 33,788 | 5 | 19.28 | 14.71 | 0.0% | 7.1% |
| `NYC-V1-R04` | East Harlem North, Manhattan | 33,788 | 6 | 12.48 | 7.81 | 100.0% | 36.3% |
| `NYC-V2-R01` | University Heights North–Fordham, Bronx | 33,433 | 5 | 5.49 | 3.83 | 100.0% | 0.0% |
| `NYC-V2-R02` | East Flatbush–Farragut, Brooklyn | 32,813 | 10 | 3.98 | 3.57 | 100.0% | 19.8% |
| `NYC-V2-R03` | Bedford-Stuyvesant East, Brooklyn | 35,451 | 10 | 3.76 | 2.85 | 100.0% | 7.3% |
| `NYC-V2-R04` | East New York–City Line, Brooklyn | 33,190 | 9 | 4.95 | 2.05 | 100.0% | 34.8% |
| `NYC-V3-R01` | Astoria Central, Queens | 36,648 | 9 | 5.33 | 7.26 | 0.2% | 18.2% |
| `NYC-V3-R02` | Parkchester, Bronx | 36,560 | 7 | 8.22 | 5.69 | 100.0% | 68.1% |
| `NYC-V3-R03` | Rockaway Beach–Arverne–Edgemere, Queens | 37,606 | 9 | 5.58 | 5.48 | 100.0% | 27.0% |
| `NYC-V3-R04` | Forest Hills, Queens | 34,486 | 7 | 8.91 | 8.55 | 0.0% | 22.1% |

The set is mutually disjoint at tract level. It spans Queens, Manhattan, the Bronx and Brooklyn but not Staten Island. That absence is not evidence that Staten Island lacks need; it is a consequence of the three declared vertical-city mechanisms and the current thresholds. A later citywide doctrine cannot generalize from this test to low-density, coastal-isolation or detached-building missions without a separate stratum.

Threshold sensitivity is orderly rather than knife-edge. Tightening `V1` floor and device cutoffs from P80 to P85 reduces its pool from 80 to 65 and retains two of four provisional references; P90 also retains two. Tightening `V2` from HVI P75/mid-rise 50 percent to P80/55 percent reduces 170 to 146 and retains three. Tightening `V3` from campus P75/device P60 to P80/P65 reduces 25 to 18 and retains all four; P85/P70 leaves eleven and retains one. The sensitivity surface shows that the set samples the declared boundary rather than only its extreme tail—which is appropriate for falsification, but it increases the importance of a frozen rule.

## Holdout commitments are not yet seals

The operator run publishes three commitments:

| Holdout | SHA-256 commitment | State |
| --- | --- | --- |
| `NYC-V1-H01` | `2a5fbcafb3f8c6a3a673021cf7ac54c817131e9384d38c3886566bd118011d39` | rehearsal only |
| `NYC-V2-H01` | `2f1b5528a53efb9288f3c9e70f3a3f592ef2f10bebf7f6366858f8fcf529ecc6` | rehearsal only |
| `NYC-V3-H01` | `284f1a756375147329171dc38e34e45899f75cbf67492bf2e0c9fcc09b602315` | rehearsal only |

The workbook withholds their GEOIDs and covariates. That protects against casual exposure, but the full candidate universe, rules and ordering are public and the commitment is unsalted. A determined analyst can reconstruct the composition. Formal holdouts require an independent custodian to select or receive the compositions, apply a secret random salt, publish salted commitments and control unsealing under a dated protocol. The operator should not retain access to the salt or sealed records.

This distinction is institutional, not cryptographic trivia. A Department of Resilience will face the same pressure as a weapons program to test on familiar ranges, tune to visible cases and explain away failure. Independent holdout custody is part of the acquisition system's separation of powers.

## What the rehearsal teaches about the force

### The city is a system of vertical service paths

The three strata do not merely create sampling variety. They imply different `NCAC` workload generators.

`V1` concentrates elevator, stair, domestic-water-pressure, medical-power and high-rise household-accounting burden. `V2` distributes contact and thermal demand across more buildings and blocks, with fewer device records per person and no single tower core to organize the mission. `V3` creates common-mode building or campus dependencies while increasing the friction between a resident and a public-service proxy. The same 35,000-person formation can encounter four tracts in one reference and ten in another; equal population does not imply equal doors, vertical metres, service interfaces or command spans.

This strengthens the case for configuring the force around measured work accounts rather than population alone. A future `NCAC` model must translate each catchment into households requiring disposition, floors and vertical trips, powered-device dependencies, water-pressure zones, candidate safe-service spaces, accessible movement cases, utility-island interfaces and field-team-hours. Population remains the denominator, not the workload model.

### Administrative abundance can conceal operational ignorance

New York supplies unusually rich public records, yet the variables that govern a heat-blackout mission remain largely unobserved: which elevators serve accessible egress, what loads backup power carries, how long fuel lasts, where domestic pumps fail, which residents need powered equipment, how indoor temperature evolves by building, which facilities will open and admit people, and what a field team can lawfully verify without commercial communications.

The proper response is not to wait for a perfect city database. It is to design the `L1` and field-reconnaissance program around these unknowns. But the workbook must never convert record volume into confidence. The 52.4 percent elevator-to-tract join and the tiny 0.159-mile facility-distance threshold are warnings: the first may reflect identifier coverage rather than device scarcity; the second measures geometric proximity in a facility-rich city, not an accessible service path.

### The HVI boundary is too coarse for building claims

Residential units inherit HVI through postcode. This creates a discrete distribution in which the candidate P75 for HVI 4–5 share is 100 percent. It separates high-burden ZCTA fabrics effectively, but it cannot identify high-risk residents or variation among buildings inside the same catchment. `V2` is therefore a neighborhood heat-burden stratum, not a clinical cohort.

Synthetic population work must add separately governed household vulnerability and building thermal-response layers. Those layers may shape the design worlds and field sample; they may not be used to replace the already selected catchments after outcomes appear.

### A purpose-built evidence force is itself national infrastructure

The source work required spatial joins across planning, tax-lot, footprint, elevator, facility, public-health and census systems that were not designed as one operational record. A mature Department cannot rebuild this lineage ad hoc during every catastrophe. It needs a standing civilian mission-data service with legal authority, privacy protection, offline continuity, versioned schemas, local stewardship and independent audit.

That is not an argument for a single omniscient federal database. It is an argument for a common continuity architecture: household and facility facts remain under appropriate custody, while the force can prove coverage, request lawful minimum data, operate through communications loss and reconcile dispositions without inventing people or losing them between systems. The New York rehearsal turns Pass 37's disconnected continuity ledger from an abstract technology program into a concrete institutional requirement.

## Required work before formal freeze

`L0` closes only after the following actions are complete:

1. **Street-topology audit.** Replace polygon touch with a versioned pedestrian/local-street graph that handles grade separation, bridges, restricted land, waterways and island components. Publish every tract-group change relative to this rehearsal.
2. **Independent reproduction.** A separate team re-downloads the declared sources, verifies hashes or documents source drift, reimplements the canonical method and reconciles all 844 candidates, twelve provisional references and three custodian records.
3. **Salted custody.** Transfer holdout compositions to an independent authority, publish salted commitments and destroy operator access to the salts.
4. **Demographic enrichment.** Acquire a reproducible official age, disability and household denominator with uncertainty; keep it outside selection and use it only for synthetic-population construction and sample design.
5. **Field-validity sample.** Before mission modeling, draw a blinded building and facility sample in every reference catchment to estimate BBL/device linkage, elevator function classes, backup load coverage, domestic-water dependencies, accessible egress and facility admission readiness.
6. **Empty outcome tables.** Publish the complete 24,000-row architecture-world key structure with all outcome cells empty, along with the correlation targets, rejection rules and software environment.
7. **Data-governance review.** Independent privacy, accessibility, civil-rights and local-authority reviewers approve the household-disposition data path before any representative contact experiment.

If the topology audit changes a catchment, the rejected composition and reason remain public. If the independent implementation disagrees because the canonical method is ambiguous, the protocol is amended while outcomes remain nonexistent. No result is grandfathered through a material lineage change.

## Decision and handoff

The provisional catchments are good enough to focus the next evidence work and not good enough to begin the architecture contest. They should be used to prepare source-specific field-validation plans, utility and building sampling frames, privacy cases, empty data structures and the independent reproduction package. They should not yet be used to simulate `A2` versus `S3`, tune formation parameters, select equipment or authorize visual renderings.

The companion [selection workbook](../../../models/nyc-l0-catchment-selection.xlsx) exposes the complete candidate universe, tract evidence surface, thresholds, reference compositions, commitments, sensitivity analysis, source hashes and formula-backed checks. It intentionally marks salted custody as open even while its internal arithmetic passes.

This is the larger institutional lesson. A coequal Department of Resilience does not prove seriousness by moving quickly from a compelling vehicle concept to acquisition. It proves seriousness by funding an evidence system capable of delaying its preferred design, discovering that its registered method is underspecified and repairing the defect before anyone can know which correction produces the better result.

No `NCAC` architecture advances. No campaign outcome exists. No rendering is authorized.
