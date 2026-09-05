# New York `L0` population and building input registration

**Registration:** `DF-NYC-L0-PR44-INPUTS-v1`

**Parent generator:** `DF-NYC-L0-PR43-GEN-v1`

**Protocol:** `DF-NYC-HB-PR38-v1`

**State:** official demographic margins and inherited building-administrative proxies registered; synthetic people, households, building states and architecture outcomes remain empty

**Decision:** close the operator observation-acquisition obligation; continue to prohibit population synthesis and both architecture executions

## Executive judgment

The New York campaign now knows substantially more about the people and built form inside its twelve reference catchments. It still does not know enough to create twelve operational populations.

Registration `DF-NYC-L0-PR44-INPUTS-v1` binds 87 official census tracts to 156 selected 2020–2024 American Community Survey estimate cells and their published 90-percent margins of error. It derives 3,306 tract-metric records and 456 catchment-metric records across age, disability, household composition, vehicle access, language access, occupancy, housing structure, heating fuel and group-quarters population. Eight ACS tables include eighty variance replicates, allowing covariance-aware uncertainty propagation through component sums, tract aggregation and ratios. Nine tables lack published tract-level replicates; their derived margins of error are explicitly weaker root-sum-of-squares approximations. No suppressed or sentinel value occurs in the selected records.

The observation surface is joined to the already frozen New York administrative building evidence: tax lots, residential units, floor counts, roof heights, elevator-device records, Heat Vulnerability Index strata and facility proximity. Those fields can distinguish reference built forms. They cannot establish who is home, who lives on which floor, whether an elevator bank has power and control, whether domestic-water pumps operate, whether emergency generation serves resident loads, or how fast an occupied zone heats after grid loss.

The resulting evidence rejects a tempting shortcut. A 35,000-person catchment cannot be represented by multiplying its population by independent “elderly,” “disabled,” “no vehicle,” “limited English,” “high-rise” and “medical power” shares. Those conditions bind within people, households, units, floors, buildings and caregiver networks. The public tables disclose margins, not those joint records. Treating the margins as independent would manufacture synthetic people who are unusually easy to contact, serve and move.

The twelve references demonstrate why the joint state matters. Their point estimates span:

| Registered condition | Lowest reference | Highest reference |
| --- | ---: | ---: |
| population age 65 and over | 10.5% | 26.3% |
| any disability among the civilian noninstitutionalized population | 5.6% | 19.7% |
| ambulatory difficulty | 2.8% | 12.0% |
| households with no vehicle available | 29.9% | 85.9% |
| limited-English-speaking households | 1.2% | 50.4% |
| one-person households | 25.2% | 57.2% |
| occupied units in structures with 50 or more units | 12.4% | 67.8% |
| inherited high-rise residential-unit proxy | 0.1% | 75.8% |

These are design inputs, not claims about all New York City neighborhoods. The references were selected to exercise three built-form archetypes; they are not a probability sample of the city. Several small categories also carry wide uncertainty. Of 456 catchment metrics, 264 meet the campaign's screening convention of a relative margin of error no greater than 20 percent, 154 are moderate-precision screens and 38 exceed 50 percent or pair a zero estimate with a positive margin. The convention is a campaign control, not a Census Bureau quality rating.

This pass therefore changes the campaign in a more important way than simply filling blank columns. It defines a new force-design object: a **governed population–household–building state compiler**. That compiler must become part of the Department of Resilience's permanent intelligence, science and operating infrastructure. It is not an incidental analyst task and cannot be assembled after a disaster from unrelated public tables.

No `A2` or `S3` function has been called. The 24,000 architecture rows and 2,000 campaign aggregates registered in Pass 42 remain empty. No rendering is authorized.

## Why the force requires this state

The campaign's public-effect unit is a person who either receives a verified safe local service bundle or is admitted to a named destination that provides the required bundle. That rule cannot be computed from a tract population alone.

For a vertical heat blackout, the service path begins inside an occupied building. A resident's outcome can depend jointly on floor, indoor thermal response, elevator and stair access, domestic-water pressure, medical electricity, mobility, communication method, language access, caregiver relationship, household vehicle access, collection availability and destination admission. Some attributes increase demand; others determine which service path remains lawful and physically possible. A caregiver and dependent person may be indivisible even if two seats exist. An operable elevator may be useless if its emergency circuit does not serve the relevant bank. A cooled site may be irrelevant if it cannot admit the person's household or clinical condition.

The needed state is therefore relational:

```text
PERSON
age · disability vector · medical-power need · communication · mobility
        │
        ▼
HOUSEHOLD
composition · caregiver binding · vehicle access · lawful disposition
        │
        ▼
UNIT / FLOOR / BUILDING
occupancy · vertical route · power topology · pumps · cooling · thermal response
        │
        ▼
SERVICE PATH
contact · local protection · vertical access · collection · admission · return
```

An additive vulnerability index can help select where to study. It cannot replace that graph. Force size follows the workload on the graph: doors that must be verified, floors that must be reached, household units that must remain together, equipment that must stay powered, litres and kilowatt-hours that must reach occupied zones, and people who must be admitted elsewhere by a clock.

## Registered evidence surface

### Exact population anchor and survey margins

The catchment registry retains the exact 2020 Census population used for outcome-blind selection: 414,234 people across 87 non-overlapping reference tracts. It now adds the Census Bureau's 2020–2024 ACS five-year release, which covers data collected from January 2020 through December 2024 and publishes tract estimates ([ACS 2024 release](https://www.census.gov/programs-surveys/acs/news/data-releases/2024/release.html)). The selected tract estimates sum to 403,320 people.

That 10,914-person difference is not labeled growth, decline or error. One value is an exact decennial count at a point in time; the other is a multiyear survey estimate with sampling and nonsampling error. Catchment differences range from −17.4 percent to +9.4 percent of the 2020 count. The architecture model cannot quietly select whichever denominator gives a preferred result. A later campaign control must choose the population authority and propagate its uncertainty into demand.

The same discipline applies to buildings. The inherited PLUTO surface contains 186,699 residential-unit records across the references, while the ACS housing-unit estimates sum to a different concept and vintage. Individual catchment differences range from −15.0 percent to +25.2 percent of the PLUTO count. The discrepancy is an audit signal, not a trend estimate.

### Covariance-aware and approximate uncertainty

The Census Bureau states that ACS estimates are subject to sampling and nonsampling error and provides variance replicate estimates for exact variance calculation when derived estimates combine published cells or geographies ([2020–2024 Accuracy of the Data](https://www2.census.gov/programs-surveys/acs/tech_docs/accuracy/MultiyearACSAccuracyofData2024.pdf); [2024 variance tables](https://www.census.gov/programs-surveys/acs/data/variance-tables/2024.html)).

For the eight available tables, this registration applies the published eighty replicate values. If `θ` is a derived full-sample estimate and `θᵣ` is replicate `r`, the standard error is:

```text
SE(θ) = sqrt[(4 / 80) × Σᵣ(θᵣ − θ)²]
MOE90 = 1.645 × SE(θ)
```

The same transformation is applied after summing components and tracts, so covariance is retained rather than assumed away. Ratio replicates divide the replicate numerator by its corresponding replicate denominator before calculating variance.

Detailed difficulty, household-vehicle, limited-English and occupied-structure tables do not have tract variance-replicate files in the 2024 publication. Their published component and tract margins are combined by root-sum-of-squares. This is visible as `RSS_MOE_APPROXIMATION` in every affected row. It omits covariance and is not represented as exact. The point estimate remains useful for adversarial configuration, but the model must not use an absent share margin of error as if it were zero.

### Medical-power context is a lower bound, not a catchment input

The current HHS emPOWER county layer reports 1,462,021 Medicare beneficiaries across New York City's five counties, including 36,295 beneficiaries associated with power-dependent devices or durable medical equipment and 12,382 associated with both an included health service and any DME. The public service is refreshed monthly and publishes de-identified counts at national, state, county and ZIP levels ([HHS emPOWER REST service](https://empowerprogram.hhs.gov/empower-rest.html)). Its own public guidance warns that the counts may underestimate the total at-risk Medicare population ([HHS emPOWER Map](https://empowerprogram.hhs.gov/empowermap)).

The figures are registered as county context only. They cover Medicare fee-for-service and Medicare Advantage claims under program definitions. They do not enumerate every electricity-dependent person, do not reveal joint household and building state, and do not match the tract geography. No proportional county-to-catchment allocation is performed. Such a downscale would convert administrative coverage into false local precision.

Closing the medical-power input requires either governed protected data with coverage accounting or a representative measurement program that estimates the uncovered population. Even then, the force needs an operational classification: device energy, permissible interruption, batteries, replacement consumables, clinical escalation, caregiver support and the building circuit or local service interface. A count alone does not define the service.

## The synthetic contract—and why it remains empty

The workbook registers the fields required for three linked synthetic entities without generating a record.

The person layer requires age, a multi-valued disability state, medical-power class, communication and language access, mobility and transfer need, and clinical continuity. The household layer requires size and composition, caregiver binding, vehicle access, lawful disposition and indivisible-movement rules. The building layer requires unit and floor occupancy, elevator-bank state, emergency-power topology, domestic-water pressure zones and pumps, resident-serving cooling, access-control state and a calibrated thermal-response class.

PUMS can supply donor relationships that published marginal tables do not. It cannot be treated as a tract microfile. The Census Bureau identifies PUMA as the most detailed PUMS geography, and the 2020–2024 file uses 2020 PUMA definitions ([ACS PUMS documentation](https://www.census.gov/programs-surveys/acs/microdata/documentation.html); [2020–2024 PUMS User Guide](https://www2.census.gov/programs-surveys/acs/tech_docs/pums/2020_2024ACS_PUMS_User_Guide.pdf)). A household drawn from a PUMA may constrain plausible joint composition. It does not establish that the household exists in a selected tract, occupies a particular building, or shares the campaign's unmeasured medical and vertical-access state.

The future compiler must therefore pass more than marginal-fit checks:

1. Person totals, household totals and housing occupancy must reconcile under one declared denominator authority.
2. Every synthetic person must belong to exactly one household; every household must bind to at most one occupied unit and one building state at a time.
3. Household and person margins must fall within registered tolerances that reflect sampling uncertainty rather than arbitrary decimal targets.
4. PUMA-level donor relationships must be reported as donor constraints, with sensitivity to alternate donor pools and methods.
5. Difficulty types must remain nonexclusive; their component counts cannot be summed as unique disabled people.
6. Caregiver, medical-power, accessible-transport and building-operability fields must remain unknown until authorized evidence exists. They may not be filled by convenient independence assumptions.
7. Disclosed validation must not release actionable household or medical microdata. Independent reviewers need method, marginal, joint, residual and stress diagnostics—not a public address-level registry of vulnerable residents.
8. The compiler must be rebuilt by a second team from the frozen sources and specification before architecture execution.

Until those conditions are approved, “synthetic population” means an empty governed schema.

## Building records are not building state

The inherited NYC evidence distinguishes demanding built forms. One reference has a unit-weighted mean of 19.3 floors, 75.8 percent high-rise proxy exposure and 497 active elevator-device records; another has a 3.8-floor mean, a 0.1-percent high-rise share and 101 active-device records. Population-weighted HVI spans 2.0 to 5.0. These contrasts validate the campaign's decision to test multiple archetypes.

They do not close the vertical service path. MapPLUTO and footprints are administrative and geometric records. Elevator compliance data describes records and status, not incident availability. Annual energy benchmarking is not emergency load, internal-zone temperature or backup runtime. Building-code applicability does not prove installed, maintained and fueled resident-serving capacity.

The minimum operational building state should instead be generated from a causal graph whose nodes include utility service, transfer switches, fuel, emergency buses, elevator banks, domestic-water pumps, cooling zones, access control, communications and occupied floors. Hard feasibility must bound the world generator: an elevator cannot operate without a surviving drive, controls, doors, route and eligible source of power. Dependence loadings alone cannot enforce that physics.

This yields four representative evidence programs before the architecture contest:

- **building continuity census:** a governed inventory of electrical one-lines, emergency loads, vertical transport, water-pressure zones, cooling capability, fuel, inspection and maintenance;
- **instrumented heat-blackout archetype trials:** occupied-equivalent thermal, water, elevator and communications behavior under controlled loss and restoration sequences;
- **vertical access workload trials:** household verification, mobility assistance, mechanical handling, stair and elevator throughput under dark-building conditions;
- **building-state inference validation:** tests of how well public and protected records predict actual incident state, including false-safe and false-unsafe errors.

These are Department-scale scientific capabilities. They imply laboratories, secure data enclaves, municipal and utility instrumentation, standing field teams, calibration standards and an independent safety and civil-rights authority.

## Technology programs implied by the evidence gap

The campaign does not yet justify a vehicle form. It does justify an ambitious technology portfolio.

### Resilience population compiler

A national compiler should generate privacy-preserving operational populations from heterogeneous evidence while carrying uncertainty and provenance into every derived state. Its outputs would be ensembles rather than one “best” population. It would preserve households and caregivers, distinguish unknown from negative, prohibit unsupported cross-geography allocation, and allow red-team reconstruction without publishing sensitive records.

### Civil continuity ledger

The `S3` architecture assumes faster disconnected household verification. That requires more than an offline database. A civil continuity ledger must support lawful enrollment, minimal necessary attributes, rapidly changing location and service status, consent and emergency authority, disconnected field reconciliation, duplicate resolution, household binding, multilingual and accessible interaction, audit, deletion, cyber compromise and deliberate nonparticipation. Its unit of performance is a verified service disposition under network loss—not records synchronized per second.

### Building systems observatory

A standing building observatory would make the interior civil network measurable. It should combine authenticated static topology with local sensing of grid service, emergency buses, elevator availability, water pressure, cooling-zone condition, indoor temperature and occupied-service requests. It must operate through commercial-network loss and degrade safely under sensor failure or cyber attack. The observatory is not a universal surveillance system; data minimization and local/public accountability are part of the architecture.

### Prepared-building adapter and autonomous vertical logistics

The evidence also defines the interface that future equipment must meet. A prepared-building adapter would accept temporary power, water, communications, cooling and logistics from multiple Department formations and expose known connection, protection, load-shed and safety states. Autonomous or highly assisted vertical logistics may carry water, batteries, medical equipment and small payloads through stairs, shafts or façades, but only representative trials can establish where such machines outperform human teams without creating egress, fire, structural or dignity hazards.

These programs are analogous to military investments in sensing, logistics, command networks and digital mission engineering: they create the information and interfaces that make physical force usable. They should be funded and tested as first-order mission systems, not left as software accessories to a platform acquisition.

## What closes, what remains binding

This pass closes one bounded operator obligation: official public demographic and housing margins are acquired, hashed, mapped to the frozen tracts, aggregated with declared uncertainty, joined to the inherited building proxy surface and registered before architecture execution. The companion workbook passes twelve formula-backed integrity checks. Its six record commitments are:

| Object | SHA-256 |
| --- | --- |
| input specification | `a073ad784d6d02963a1b1676989482cad90ce7ffe9e00849ed50deb53d11da73` |
| source manifest | `b6a917a93d7f81ea8c8b4bb1ff691d1f0c6dcbf68ecdbadbffb3e40ac3044bb0` |
| tract metric records | `23898c91d5a4886984bad6f54872e2c17700d3b9108ca6323f91cb42500e1595` |
| catchment metric records | `909d79e8f9e6893c1a3456df48f0cf79ef469d25b67f8ab76c802bd2b4db03cb` |
| building administrative records | `cec74f339febb7daf9a3bd7b9485234ecff7e2fd4f20bb748ef36e6e152b6dea` |
| HHS emPOWER county context | `84884cc7a2a1791d3fcff7f6f32c1e5948341fd694ef90f6998a51c6c3554785` |

Repository custody remains operator-controlled, not independent. The workbook binary has SHA-256 `c6326024d523169a53f912cf0a62ed57e9c8cb30e0a7e7b14a3a1cac3353c268`.

Eight gates still prevent population synthesis or architecture execution:

1. choose and propagate a campaign population and housing denominator authority;
2. approve the tract-constrained PUMS donor method and joint-distribution diagnostics;
3. acquire governed person–household–unit–floor–building bindings or a defensible uncertainty model;
4. measure medical-power need with explicit program coverage and no proportional geographic invention;
5. build the operational building-state graph and causal feasibility solver;
6. replace or independently defend borough as a service-territory proxy;
7. complete independent reconstruction and alternative dependence cases; and
8. establish privacy, civil-rights and salted external custody before unsealing any holdout.

The next useful pass should not synthesize records immediately. It should register the compiler algorithm, permissible evidence, privacy architecture, marginal and joint diagnostics, feasibility rules, ensemble size, rejection criteria and empty output surface first. Only then should a generator be allowed to create synthetic persons, households and building states.

The [companion workbook](../../../../models/nyc-l0-population-building-input-registration.xlsx) contains the full tract and catchment surfaces, source manifest, variable dictionary, building proxies, medical-power context, synthetic schema, gate stack, missingness ledger, reliability classifications and integrity commitments.

No vehicle, formation or site rendering is authorized.
