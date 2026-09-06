# New York `L0` empty outcome registration

**Registration:** `DF-NYC-L0-PR42-EMPTY-v1`

**Protocol:** `DF-NYC-HB-PR38-v1`

**Pre-outcome amendment:** `DF-NYC-HB-PR42-A1`

**Status:** identity and schema registered; world factors and all architecture outcomes remain empty

**Decision:** close the operator empty-table obligation; prohibit execution until the remaining `L0` gates close

## Executive judgment

The New York campaign now has a complete place for failure to appear before either architecture is allowed to produce a result.

This registration creates 12,000 catchment–world identities, each with one `A2` and one `S3` row, for exactly 24,000 paired architecture–world rows. It also creates 2,000 campaign-aggregate identities: 1,000 twelve-catchment replicate blocks for each architecture. Every execution field, world factor, raw outcome, adjudication, derived result and campaign result is blank. The only populated values are frozen identity, architecture version, seed commitment and registration state.

The work found and repairs a logical ambiguity in the parent protocol while outcomes remain nonexistent. The protocol named a catchment–world pair as its primary unit, yet one complete-rule condition referred to the “worst reference catchment,” an object that exists only across a twelve-catchment campaign. It also required 95 percent safe service in every catchment while separately imposing a 90 percent worst-catchment floor, making the latter redundant.

Amendment `DF-NYC-HB-PR42-A1` separates the levels:

- each catchment–world must reach a 90 percent safe-service floor and pass household, contact, movement, exposure, readiness and sentinel gates;
- each twelve-catchment campaign replicate must reach 95 percent population-weighted safe service, 95 percent aggregate mandatory-movement admission and no catchment below 90 percent; and
- `H1` and `H2` operate on paired catchment–world results, while `H4` operates on the campaign replicate.

This is not a result-generating model. No Latin-hypercube factor value, simulated demand, performance measure or architecture comparison appears in the artifact. The target dependence matrix, generator implementation, demographic enrichment, independent topology reproduction and salted holdout custody remain open. The registration makes those absences visible and prevents a future analyst from silently changing row identity, denominator, failure precedence or missing-data treatment after seeing outcomes.

## Why an empty table is a research instrument

Preregistration is often treated as a promise in prose. A computational campaign needs a more demanding object: a table whose row universe, field names, types, units, allowable null states, architecture versions, hypotheses and decision rules already exist.

Without that object, apparently minor implementation choices can change the answer:

- generating different input worlds for the two architectures destroys pairing;
- dropping a simulator nonconvergence can favor the more fragile architecture;
- representing zero mandatory-movement demand as 100 percent admission hides the denominator;
- imputing an absent outcome can convert measurement failure into service;
- treating a pending rights adjudication as zero sentinels converts uncertainty into permission;
- changing the first-failure hierarchy after inspection can change the causal explanation; and
- aggregating twelve catchments without a registered replicate key can manufacture or erase covariance.

The National Academies distinguishes computational reproducibility from broader replication and emphasizes the need to supply the data, code and methods required to obtain the same result ([Reproducibility and Replicability in Science](https://doi.org/10.17226/25303)). The [NIST/SEMATECH Engineering Statistics Handbook](https://doi.org/10.18434/M32189) treats a computer experiment as an experiment in which factors are deliberately varied and outputs observed, and identifies Latin-hypercube designs as useful for that setting. Neither source validates this campaign. They support the discipline of fixing the experimental object and exposing the method before interpreting a response surface.

## Registered units

### Catchment–world pair

The primary unit is one frozen reference catchment under one design-space world. Both architectures receive the same future input snapshot.

```text
PAIR ID
  ├── same catchment
  ├── same replicate block
  ├── same world factors
  ├── same source and generator hashes
  ├── A2-PR37-v1 row
  └── S3-PR37-v1 row
```

There are twelve reference catchments and 1,000 world indices per catchment, producing 12,000 pair IDs. Each pair produces two architecture rows, yielding 24,000 registered outcome rows.

The pairing rule is exact, not statistical. A result row cannot substitute a different input snapshot merely because it has the same factor ranges. If one architecture experiences an external execution defect, both rows are quarantined and rerun together under the same frozen inputs before unblinding.

### Campaign replicate

World index `0001` through `1000` also defines a citywide replicate block. Each block contains twelve catchment worlds and two architecture aggregate rows.

The common index does not assert that catchments are independent. Later world generation must include shared citywide latent draws and local residuals. Heat, grid loss, commercial communications, workforce stress and cell utility common modes require cross-catchment dependence; building backup, vertical access, domestic pumps, prepared sites and street friction require catchment-specific structure. Until the target cross-catchment and within-catchment dependence matrices are registered, all factor cells remain blank.

The campaign table has 2,000 rows: 1,000 replicate blocks for `A2` and 1,000 for `S3`. It is derived only after all twelve required catchment rows reach an admissible locked state.

## Deterministic identity and custody

The registration uses four layers of identity:

| Object | Count | Construction |
| --- | ---: | --- |
| reference catchment | 12 | preserved candidate ID and composition hash from the street-topology audit |
| catchment–world pair | 12,000 | SHA-256 commitment over protocol, catchment and four-digit world index |
| architecture outcome row | 24,000 | SHA-256 commitment over pair ID, architecture ID and frozen architecture version |
| campaign aggregate row | 2,000 | SHA-256 commitment over replicate ID, architecture ID and version |

Global and local seed commitments are also registered as sixteen hexadecimal characters derived from the protocol, registration, replicate and catchment identities. They are inputs to the future generator specification; they are not permission to choose a pseudorandom generator later without amendment.

The canonical registration object includes the architecture versions, catchments, factor ranges, success rules, hypotheses, failure codes, missingness rules, state machine and ninety-two registered fields. Its SHA-256 is:

`8124258f13574d1fd03243a49067e6e592e16dbda757ca4e2a219c1eb5d6ae94`

Three additional ledgers bind the ordered row identities:

| Ledger | SHA-256 |
| --- | --- |
| 12,000 world/pair keys | `01acbda9db5a642edd304c847a5d4aa077bcaaa8f650ce7c63a310cff190d326` |
| 24,000 outcome-row keys | `79f029f3d3b6b99dafadd17513fbaa1f683739407e78811bb1360f732137af5f` |
| 2,000 campaign-row keys | `677ae43ca4f62fadabfda6c066c6ed97647c3f016978fadc659d7bab606c99e0` |

These hashes can show that the registered object or row sequence changed. They do not establish independent custody. The repository operator currently controls the artifact, so an external registration service or independent custodian must countersign the final `L0` package before execution.

## Amendment `DF-NYC-HB-PR42-A1`

### The ambiguity

The parent protocol made the paired catchment–world difference the main estimand and asked whether `S3` succeeded within each archetype. Those are row-level questions. Its complete rule also included 95 percent total safe-service closure and a 90 percent worst-reference-catchment floor. A single catchment row cannot contain a worst-of-twelve result.

The accompanying `H4` text required every reference catchment to reach 95 percent safe service. Under that interpretation, the worst-catchment 90 percent requirement could never be the binding constraint: if every catchment is at least 95 percent, the minimum is also at least 95 percent.

### The correction

The amendment defines two connected rules.

The **catchment complete rule** uses the following gates:

1. 100 percent authoritative household disposition by hour 36;
2. at least 95 percent high-risk household contact by hour 18;
3. at least 90 percent safe-service closure by hour 72;
4. at least 95 percent mandatory-movement destination admission by hour 72, or `PASS_NO_DEMAND` when the registered denominator is exactly zero;
5. no more than eighteen mean unsafe indoor hours per demand person;
6. at least 80 percent next-mission capacity at hour 168, measured as the minimum of qualified people, mission-capable equipment, utility capability, stocks and reconcilable records; and
7. zero attributable rights and safety sentinels with adjudication complete.

The **campaign complete rule** requires:

1. all twelve catchment rows present and admissible;
2. at least 95 percent population-weighted safe service across the twelve catchments;
3. at least 95 percent aggregate mandatory-movement admission, or `PASS_NO_DEMAND` only when the total registered denominator is zero;
4. no catchment below 90 percent safe service; and
5. every non-aggregate catchment gate passed.

`H1` compares the paired catchment complete-rule indicator. `H2` measures `S3` catchment complete-rule coverage within each archetype. `H3`, `H5` and `H6` remain catchment-level constraints. `H4` becomes the campaign-level aggregate and worst-catchment test.

The amendment does not weaken a service obligation. It makes the original 95/90 structure mathematically coherent: a 95 percent total standard prevents the force from serving every catchment at only 90 percent, while the 90 percent floor prevents the total from being achieved by sacrificing one place.

## Raw outcomes and denominators

The outcome register stores counts before shares. It reserves separate fields for:

- total households and households authoritatively disposed by hour 36;
- high-risk households and those contacted by hour 18;
- design-demand people and people in verified safe service by hour 72;
- people requiring mandatory movement and people admitted by hour 72;
- unsafe indoor person-hours;
- five separate next-mission capacity shares;
- five separate attributable sentinel counts;
- unresolved accessibility, consent and household-continuity queues;
- adjudication, first failure, terminal state and amendment lineage; and
- run, input, code and execution hashes.

The raw table does not prepopulate derived ratios or success flags. Those are produced only after raw lock under separately hashed analysis code. This preserves numerator and denominator, prevents a blank from looking like zero and allows the independent evaluator to recompute every gate.

The campaign aggregate table follows the same rule. It reserves total demand, total safe service, mandatory movement and admission counts; derived aggregate shares; the worst catchment; all-catchment gate flags; sentinel and unresolved-rights totals; complete-rule result; first failure; and adjudication state. Every field is blank.

## Missingness and execution defects

The registration distinguishes absence before execution from missing evidence after execution.

| State | Primary treatment |
| --- | --- |
| registered empty | expected blank before authorization; not missing data |
| source missing | retain flag and source; use only a registered imputation and missing-not-at-random sensitivity |
| structural zero mandatory demand | record numerator `0`, denominator `0` and `PASS_NO_DEMAND`; never encode a 100 percent share |
| architecture-caused nonconvergence or impossible state | architecture failure; no favorable rerun |
| external execution defect | quarantine both paired rows and rerun both once under identical frozen inputs before unblinding |
| adjudication pending at lock | not a pass; count pending and treat conservatively in the primary result |
| measurement missing | not a pass; no primary outcome imputation |
| post-terminal unobserved field | remain blank with stop reason; row remains a failure |

This distinction prevents two opposite errors. It does not punish an architecture for a demonstrably external corrupt file while allowing its paired rival to keep a clean run. It also does not excuse an architecture because its own complexity caused the model or system to fail to produce an answer.

## Failure ordering

The register assigns first-failure precedence before results exist:

1. hour-18 high-risk contact precedes hour-36 household disposition, preserving temporal order in both the summary code and the raw failure hour;
2. attributable rights and safety sentinels stop advancement regardless of throughput;
3. catchment safe-service, mandatory admission and unsafe exposure follow at the hour-72 boundary;
4. next-mission readiness follows at hour 168;
5. campaign aggregate safe service, aggregate admission and worst-catchment floors are evaluated after all twelve rows lock; and
6. incomplete data and external execution defects retain distinct codes rather than being mixed with capability failure.

The summary `first_failure_code` cannot replace the full gate vector. It is a causal index for secondary analysis, not a compensating score.

## State and authority

Each row moves through a registered state machine:

```text
REGISTERED_EMPTY
      ↓ registration custodian
INPUTS_FROZEN
      ↓ independent data board
AUTHORIZED
      ↓ independent test director
RUNNING
      ├── QUARANTINED → governed paired rerun or locked failure
      └── RAW_LOCKED
                ↓ rights, safety and measurement authorities
          ADJUDICATED
                ↓ independent analysis board
          ANALYSIS_LOCKED
                ↓ holdout custodian
             UNSEALED → PUBLIC
```

No operating sponsor can promote its own row. Raw measurements are append-only. Architecture labels may be masked from rights and safety adjudicators where operationally possible. A pending sentinel or lawful-inaccessibility decision cannot be silently replaced by zero.

## Statistical interpretation

The 1,000 worlds per catchment cover a declared multidimensional design space. They are not 1,000 observed disasters and do not estimate annual probability.

`H1` reports the mean paired difference in catchment complete-rule success overall and within archetype. The registered interval uses 10,000 resamples of the twelve catchment clusters. With only twelve clusters, that interval is a descriptive sensitivity to the selected geography, not a source of false precision or a replacement for the raw catchment results.

`H2` reports raw `S3` coverage of the design space within each archetype and a catchment-resampled lower interval. `H4` reports campaign-replicate coverage under the cross-catchment dependence structure eventually registered. No result may be translated into event reliability without externally warranted occurrence distributions.

The Latin-hypercube generator remains deliberately unbuilt. Before `INPUTS_FROZEN`, the program must register:

- the generator and pseudorandom algorithm;
- factor transforms and truncation;
- target within-catchment and cross-catchment dependence matrices;
- the method for enforcing conditional dependencies;
- rejection criteria and maximum redraw count;
- achieved-correlation tolerances;
- alternate dependence-strength cases;
- demographic and building-demand generation;
- source and code hashes; and
- a blind diagnostic that does not execute either architecture.

## Integrity result

The registered artifact contains:

| Object | Count | Blank integrity |
| --- | ---: | --- |
| reference catchments | 12 | identity only |
| world/pair rows | 12,000 | twenty reserved fields blank per row |
| architecture outcome rows | 24,000 | thirty-one reserved fields blank per row |
| campaign aggregate rows | 2,000 | seventeen reserved fields blank per row |
| schema fields | 92 | roles and blank-at-registration rules explicit |

Each pair has exactly two architecture rows. Each replicate has exactly twelve world rows and twenty-four architecture rows. Each architecture has 12,000 outcome rows. All 744,000 reserved outcome cells, 240,000 reserved world cells and 34,000 reserved campaign cells are blank. Seventeen independent build checks and workbook formulas reconcile the counts and detect any populated reserved range.

## Institutional implication

A mature Department of Resilience needs a **campaign registration and evidence-custody authority** whose power is organizational, not ceremonial. It should own identity ledgers, protocol hashes, source freezes, randomization commitments, access control, blinded adjudication, missingness decisions, unsealing and public deviation records. Program managers may propose architectures and explanations; they may not redefine the rows on which their success is judged.

This is the rescue-and-stabilization analogue of investing in test ranges, operational evaluation, configuration control and intelligence custody. It is easy to fund a dramatic vehicle and leave the evidence system informal. A coequal national instrument does the opposite: it builds enough institutional machinery to discover that a favored platform, software system or formation fails before public dependence makes that failure catastrophic.

## Remaining `L0` gates

The empty-table obligation is complete at operator level. Architecture execution remains prohibited until:

1. an independent team reproduces the topology, catchments, row identities and schema hashes;
2. governed age, disability, medical-power, accessibility and household inputs are acquired and their missingness rules registered;
3. the world generator and target/achieved dependence matrices are registered without executing either architecture;
4. an external custodian creates salted holdout commitments and controls unsealing;
5. disability-led, rights, safety, statistical and privacy authorities approve the design; and
6. the complete registration receives an immutable external timestamp or countersignature.

No `NCAC` evidence gate advances. No architecture result exists. No rendering is authorized.

## Registered artifact

The companion [empty outcome registry workbook](../../../../models/proving/campaigns/new-york/nyc-l0-empty-outcome-registry.xlsx) contains the registration control, catchment and architecture lineage, hypotheses, factor ranges, success rules, missingness, failure codes, state machine, ninety-two-field schema, all 12,000 world identities, all 24,000 empty architecture rows, all 2,000 empty campaign rows, sources and formula-backed integrity checks.
