# New York `L0` world-generator registration

**Generator:** `DF-NYC-L0-PR43-GEN-v1`

**Parent registration:** `DF-NYC-L0-PR42-EMPTY-v1`

**Protocol:** `DF-NYC-HB-PR38-v1`

**State:** design factors frozen; demographic and operational input snapshot still open

**Decision:** close the operator generator-and-dependence obligation; continue to prohibit both architecture executions

## Executive judgment

The New York campaign now has a reproducible answer to a question that had remained dangerously informal: **what does one of the campaign's 1,000 “broad uncertainty worlds” actually mean?**

Generator `DF-NYC-L0-PR43-GEN-v1` creates 12,000 catchment–world factor vectors while preserving the 12,000 pair identities registered in Pass 42. Each of the twelve factors occupies every one of 1,000 equal-width strata exactly once within each catchment. The factors are coupled through citywide, borough and catchment latent drivers so grid loss, communications, building backup, vertical access, water pumps, cooling, field labor, streets, utility output and illness do not behave like independent dice.

The first deterministic attempt passes every registered diagnostic:

| Diagnostic | Result | Limit |
| --- | ---: | ---: |
| mean within-catchment maximum absolute Spearman deviation | 0.0244 | 0.0550 |
| mean within-catchment Spearman RMSE | 0.0091 | 0.0200 |
| worst individual-catchment maximum absolute deviation | 0.1030 | 0.1200 |
| same-borough cross-catchment maximum absolute deviation | 0.0316 | 0.0700 |
| different-borough cross-catchment maximum absolute deviation | 0.0232 | 0.0500 |

All 144 catchment–factor margins contain exactly 1,000 unique strata and no out-of-range value. The target within-catchment Pearson correlation matrix has a minimum eigenvalue of 0.3449, so the registered loading construction is positive definite rather than a hand-edited correlation table repaired after generation.

This is **not an event forecast**. The factor margins are deliberately uniform design coverage over the ranges registered in Pass 42. The dependence loadings are transparent stress hypotheses, not estimates fitted to observed disasters. A world index does not carry an annual probability, recurrence interval or climate scenario weight. The design can compare two architectures across the same declared stress surface; it cannot estimate how often either architecture would succeed in New York.

No `A2` or `S3` model has been called. No demand population, building state, service outcome, failure code, hypothesis result or campaign aggregate has been produced. The outcome tables registered in Pass 42 remain empty.

## Why independent ranges would be false precision

A conventional Latin hypercube can cover each input range well and still manufacture an implausibly easy world. If grid outage duration, elevator availability, pump availability, communications, cooling and workforce are permuted independently, long grid loss is just as likely to coincide with strong supporting systems as with weak ones. The resulting “diversity” comes from the sampling method, not the physical system.

The NIST Community Resilience Planning Guide treats infrastructure dependencies as physical, functional, spatial, temporal and source relationships, and emphasizes that disruptions propagate through external systems and internal critical components ([NIST SP 1190, Volume II](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.1190v2.pdf)). The guide does not supply coefficients for this campaign. It establishes why dependence cannot be ignored.

The original Latin-hypercube paper showed why stratified input coverage can improve computer experiments relative to simple random sampling for important estimator classes ([McKay, Beckman and Conover, 1979](https://doi.org/10.1080/00401706.1979.10489755)). The [NIST/SEMATECH Engineering Statistics Handbook](https://doi.org/10.18434/M32189) likewise identifies Latin-hypercube designs as especially useful for computer experiments. Neither source turns a chosen input range into an observed probability distribution or validates the dependence hypotheses below.

The design therefore separates two obligations:

1. **marginal coverage:** every catchment must cover every registered factor range evenly; and
2. **joint stress:** factors must move together through explicit, reviewable common-mode mechanisms.

## Hierarchical dependence model

For replicate `r`, catchment `c`, primary borough `b(c)` and factor `f`, the latent score is

```text
Z[r,c,f] = A_city[f] · G[r]
         + A_borough[f] · B[r,b(c)]
         + A_local[f] · L[r,c]
         + a_residual[f] ε[r,c,f]
```

where all latent driver components begin as independent standard-normal draws. The loading rows satisfy

```text
||A_city[f]||² + ||A_borough[f]||² + ||A_local[f]||² + a_residual[f]² = 1
```

for every factor. This makes the full latent covariance matrix positive semidefinite by construction. It also gives every correlation an explanation:

- `G[r]` creates common citywide stress across all twelve catchments;
- `B[r,b(c)]` creates additional dependence among catchments assigned to the same primary borough;
- `L[r,c]` creates joint conditions within one catchment; and
- `ε[r,c,f]` preserves factor-specific variation rather than forcing all behavior through a few common modes.

### Citywide drivers

| Driver | Positive direction | Principal role |
| --- | --- | --- |
| regional heat severity | more severe heat | raises indoor heat and illness demand; reduces labor, street and cooling performance |
| regional grid failure | deeper common electrical disruption | lengthens grid loss and reduces communications, access, cooling and utility realization |
| regional operational capacity | stronger field system | raises workforce, street, communications, cooling and utility performance |
| cell common-mode capacity | stronger shared cell technology and sustainment | primarily raises realized cell-utility output, with smaller effects on cooling and communications |

### Borough drivers

The borough layer represents sub-city infrastructure and operating conditions that can affect several catchments without becoming citywide. `borough_infrastructure_capacity` couples grid duration, building backup, elevators, pumps, communications, cooling and cell utilities. `borough_operational_access` couples streets, workforce, communications and cooling.

Primary borough is a registered approximation, not a claim that utility, labor or communications service areas follow borough boundaries. It is used because the current catchment registry carries a defensible borough classification but does not yet contain validated feeder, pressure-zone, carrier, depot, labor-shed or transportation-control territories. Replacing borough with observed service territories will require a new generator version, not a silent edit.

### Catchment drivers

| Driver | Positive direction | Principal role |
| --- | --- | --- |
| building resilience | stronger building-level continuity | raises backup, elevator, pump and cooling availability; reduces indoor heat accumulation |
| neighborhood heat burden | greater local heat and vulnerability | raises demand, indoor heat and illness; reduces labor and cooling |
| local access capacity | stronger block and street operations | raises street productivity and field workforce, with smaller communications effects |
| local utility capacity | stronger local utility and communications support | raises cell utility, communications, cooling, backup, elevator and pump availability |

The model does not reject an unusual combination merely because it is rare under the loading structure. A high-grid-loss world with relatively strong elevators, for example, may represent unusually capable building backup. Such tail combinations are useful adversarial cases. Rejection is reserved for failures of the registered mathematical and coverage diagnostics, not for worlds that make a preferred narrative uncomfortable.

## Registered variance allocation

The loading squares allocate latent variance by hierarchy. They are scenario-design parameters, not fitted variance components.

| Factor | Citywide | Borough | Catchment | Residual |
| --- | ---: | ---: | ---: | ---: |
| design demand multiplier | 0.073 | 0.010 | 0.125 | 0.792 |
| indoor heat accumulation | 0.368 | 0.043 | 0.305 | 0.285 |
| grid outage hours | 0.502 | 0.125 | 0.025 | 0.348 |
| building backup availability | 0.043 | 0.043 | 0.385 | 0.530 |
| elevator availability | 0.085 | 0.065 | 0.338 | 0.512 |
| domestic water-pump availability | 0.085 | 0.065 | 0.385 | 0.465 |
| commercial communications through hour 36 | 0.378 | 0.073 | 0.165 | 0.385 |
| field workforce availability | 0.255 | 0.025 | 0.175 | 0.545 |
| street-operability productivity | 0.238 | 0.092 | 0.335 | 0.335 |
| prepared cooling-service availability | 0.165 | 0.050 | 0.335 | 0.450 |
| cell-utility realized output | 0.375 | 0.050 | 0.190 | 0.385 |
| heat-sensitive illness arrival | 0.328 | 0.013 | 0.238 | 0.422 |

Three choices are visible in this allocation.

First, grid duration carries the largest citywide share because a metropolitan blackout is the campaign's initiating common mode. Second, building backup, elevators, domestic pumps and prepared cooling retain large catchment shares because building condition and local interfaces vary sharply inside one outage. Third, residual variance remains material for every factor. The generator is not allowed to imply that four citywide narratives explain every local future.

The lowest residual share is 0.285, for indoor heat accumulation. No factor is deterministically recoverable from the shared drivers.

## From latent score to centered Latin hypercube

The generator does not use a volatile spreadsheet random function. It applies this fixed sequence:

1. Construct a label from the protocol ID, generator ID, attempt number, replicate ID, hierarchy, spatial unit and driver or factor name.
2. Hash the UTF-8 label with SHA-256.
3. Interpret the first 64 digest bits as an unsigned integer and map it to the open unit interval with `(integer + 0.5) / 2^64`.
4. Convert two separately labeled uniforms to one normal draw with the Box–Muller transform.
5. Combine the normal drivers with the frozen loading vectors.
6. Rank the 1,000 latent scores within each catchment–factor column; an exact tie is resolved by ascending replicate index.
7. Place rank `k` at the center of its stratum, `u = (k − 0.5) / 1000`.
8. Map `u` linearly to the registered low and high values.

NIST FIPS 180-4 defines SHA-256 and the integrity properties of its digests ([Secure Hash Standard](https://doi.org/10.6028/NIST.FIPS.180-4)). Here SHA-256 serves two narrower purposes: a portable labeled numerical stream and an integrity commitment. The stream is public and deterministic. It is not secret randomization, a security control or a substitute for external holdout custody.

Centered strata remove within-bin jitter. This makes the design exactly reproducible and gives every catchment–factor the same marginal mean and evenly spaced levels. The tradeoff is intentional: the campaign studies architecture behavior over a declared rectangular design space, not uncertainty inside each one-thousandth interval.

## Dependence targets and acceptance

Because the latent model is Gaussian before ranking, a latent Pearson correlation `ρ` has target Spearman correlation

```text
ρ_s = (6 / π) asin(ρ / 2)
```

The registered target matrices follow directly:

```text
within one catchment:
    R_city + R_borough + R_local + residual diagonal

different catchments, same primary borough:
    R_city + R_borough

different catchments, different primary boroughs:
    R_city
```

The generator accepts the first attempt numbered `0` through `99` that meets all five diagnostics shown in the executive table. This rule is fixed before either architecture runs. Attempt zero passes, so no redraw occurs.

The tolerance does not claim that the loadings are true to four decimals. It prevents an implementation from declaring one dependence structure and accidentally producing another. Scientific review must separately decide whether the target itself is plausible.

## Factor ranges and marginal result

| Factor | Range | Unit | Design interpretation |
| --- | ---: | --- | --- |
| design demand multiplier | 0.80–1.30 | ratio | population and service-demand stress |
| indoor heat accumulation | 0.70–1.40 | ratio | building thermal burden |
| grid outage | 24–168 | hours | common electrical disruption |
| building backup availability | 0.20–0.80 | share | building continuity state |
| elevator availability | 0.05–0.60 | share | vertical-access condition |
| domestic water-pump availability | 0.20–0.80 | share | pressurized domestic-water condition |
| commercial communications through hour 36 | 0.00–0.50 | share | surviving commercial communications |
| field workforce availability | 0.65–0.95 | share | usable field labor |
| street-operability productivity | 0.60–1.00 | ratio | combined street and curb productivity |
| prepared cooling-service availability | 0.50–0.90 | share | prepared receiver availability |
| cell-utility realized output | 0.70–0.95 | share | output after shared cell failures |
| heat-sensitive illness arrival | 0.80–1.50 | ratio | clinical demand stress |

Every factor uses all 1,000 centered levels in every catchment. For example, grid outage begins at 24.072 hours and ends at 167.928 hours; its mean is exactly 96 hours. These are design levels, not asserted measurement precision.

## Adversarial-tail coverage

The following combinations remain in the accepted matrix. They are diagnostics of coverage, not empirical frequencies.

| Code | Declared combination | Catchment–world rows | Minimum per catchment | Maximum per catchment |
| --- | --- | ---: | ---: | ---: |
| `T01` | grid loss at least 144 h and commercial communications no more than 0.10 | 938 | 72 | 86 |
| `T02` | indoor heat at least 1.25 and prepared cooling no more than 0.60 | 1,240 | 98 | 110 |
| `T03` | building backup no more than 0.30 and elevator availability no more than 0.20 | 1,071 | 84 | 98 |
| `T04` | street productivity no more than 0.70 and workforce no more than 0.75 | 1,806 | 143 | 158 |
| `T05` | grid loss at least 120 h and cell-utility output no more than 0.80 | 2,100 | 168 | 188 |
| `T06` | indoor heat at least 1.25, grid loss at least 120 h and communications no more than 0.15 | 813 | 65 | 79 |

These counts should not be compared to historical event counts. They show that every disclosed catchment receives meaningful compound stress rather than only one-variable extremes.

## Integrity commitments

| Object | SHA-256 |
| --- | --- |
| generator specification | `2c774e7c2e29b5971eafe7d16e665cb445738c1a105a3e7890200da93bb47836` |
| algorithm text | `d8169a6497ac777a32315ebbad709cd2affbd32e959d6d6b0e6f97e1f0e9d164` |
| ordered parent world keys | `01acbda9db5a642edd304c847a5d4aa077bcaaa8f650ce7c63a310cff190d326` |
| ordered world factor values | `7ef09ee18a97cdb0d7ded2677c23f924611fb8815d1ca5893df33a31768fe45d` |

The world-value digest serializes each ordered pair ID followed by the twelve factor values at eight decimal places. Changing one identity, order or registered value changes the commitment.

These repository hashes establish internal integrity, not independent custody. The operator controls both the method and the artifact. An external custodian must still countersign the accepted design, retain the salted holdouts and govern unsealing.

## What the generator does not yet contain

The design is intentionally incomplete in six important ways.

1. **No fitted occurrence distribution.** Uniform margins and loadings cover a stress space; they do not estimate New York event likelihood.
2. **No time series.** Each factor summarizes a declared campaign condition. It does not yet resolve hour-by-hour grid restoration, indoor temperature, staffing, transport or utility dynamics.
3. **No observed service territories.** Borough effects stand in for validated feeder, carrier, water-pressure, labor, depot and control geographies.
4. **No synthetic population or building demand.** Age, disability, medical power, household composition, occupancy, elevator inventory, accessibility and building thermal state remain open inputs.
5. **No causal feasibility solver.** Dependence makes combinations more or less common on the design surface but does not hard-code, for example, that every elevator must be bounded by one backup-power share. Those physical constraints belong in the building-state generator and architecture interface model.
6. **No architecture response.** The accepted worlds have never been passed to `A2` or `S3`.

Alternative dependence strengths must be registered before analysis. At minimum, the future package should include weaker citywide coupling, stronger grid/common-mode coupling and service-territory replacements for borough effects. Those sensitivity cases are structural challenges to the conclusion, not opportunities to select the case that favors one architecture.

## Institutional implication

A mature Department of Resilience needs an **experimental-world authority** between intelligence and operational test. Its job is not to predict a single disaster. It maintains adversarial, reproducible stress spaces; registers which dependencies are treated as citywide, regional, local or independent; preserves common worlds across rivals; and prevents program offices from purchasing synthetic diversity through unjustified independence assumptions.

That function is as consequential as a test range. A force can appear robust because its pumps, aircraft, communications, crews, routes and destinations are counted separately while they share power, fuel, software, labor, authority or repair. The generator is therefore part of force design: it determines whether common modes are visible before acquisition scale makes them expensive to discover.

## Remaining `L0` gates

The operator generator-and-dependence obligation is complete. Architecture execution remains prohibited until:

1. an independent implementation reproduces topology, catchments, row identities, generator values and all four hashes;
2. governed age, disability, medical-power, household, accessibility, occupancy and building-condition inputs are acquired;
3. service territories replace or explicitly retain the borough proxy under independent review;
4. the building/population generator, missingness propagation and causal feasibility rules are registered;
5. alternate dependence-strength cases are frozen;
6. an external custodian controls salted holdouts, countersignature and unsealing; and
7. disability-led, rights, safety, statistical, privacy, labor and technical authorities approve the complete `L0` package.

No `NCAC` evidence gate advances. No campaign performance result exists. No rendering is authorized.

## Registered artifact

The companion [world-generator workbook](../../../../models/proving/campaigns/new-york/nyc-l0-world-generator-registration.xlsx) contains the algorithm, factor ranges, complete loading registry, variance allocation, target and achieved within-/cross-catchment matrices, 12,000 world vectors, all Latin-hypercube strata, marginal checks, dependence diagnostics, tail coverage, sources and formula-backed integrity checks.
