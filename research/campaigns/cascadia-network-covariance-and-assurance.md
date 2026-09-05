# Cascadia network covariance and campaign assurance

## Executive judgment

The Pass 25 Cascadia campaign proved that a complete response force could be *arithmetically arranged* to close four deployment waves across nine temporarily disconnected service islands. It did not prove that the twelve named paths were operationally independent. This paper introduces shared hazard, fuel, communications, workforce, authority, repair and inspection failure into that architecture.

The finding is severe. Under the declared screening assumptions, the deterministic reference architecture closes only **5.8 percent** of 500 fixed-seed trials. Hardening the same one-path-per-group topology raises closure to **21.4 percent**. Duplicating critical paths and permitting air-path substitution reaches **48.0 percent**. A three-cell campaign mesh reaches **84.2 percent**, with a simple 95-percent binomial half-width of about 3.2 percentage points. None clears the deliberately demanding 95-percent design-assurance target.

These values are not forecasts. The marginal failure rates and correlations are research assumptions, not fitted Cascadia distributions. The result is a design discriminator: it demonstrates that nominal path diversity can disappear when physically different assets share the same fuel terminal, data service, labor pool, technical release chain, inspection system or repair parts.

The institutional conclusion is more important than the percentage. The Department of Resilience should not organize theater opening around fleets and modes. It should organize around **independently supportable campaign cells**: origin-to-effect formations with their own command, energy, communications, crews, repair, safety authority, inventories and substitution rights. Platforms belong inside those cells. The cell—not the ship, aircraft, convoy or port—is the minimum unit of resilience force projection.

The accompanying [covariance and assurance workbook](../../models/cascadia-covariance-model.xlsx) exposes all assumptions, fixed random draws, latent states, closure formulas, finance deltas, sources and open evidence gates.

## The contradiction exposed by Pass 25

Pass 25 divided the Cascadia theater into nine service islands, eight origin hubs and twelve operating paths assigned to eleven correlation groups. In its selected deterministic stress case, sixty-four formation loads, 1.763 million tonnes, forty-four public-service tests, responder bases, sustainment and return flow all closed. That was a major advance over a national model that treated lift as an aggregate pool.

Yet the word *independent* was doing more work than the model could support.

Two routes can be geographically separate and still depend on:

- the same fuel refinery, pipeline, dispatch system or charging supply;
- the same satellite or terrestrial communications provider;
- the same airspace, port, rail or bridge inspection authority;
- the same scarce pilots, linemen, clinicians, reactor operators or maintainers;
- the same depot, diagnostic software, cyber service or replacement component;
- the same safe-zone base, transfer yard or utility interconnection;
- the same regional weather system or aftershock sequence; and
- the same civil decision that establishes priorities and accepts residual risk.

NIST's community-resilience method makes time to recovery of function a primary metric and requires planners to identify internal and external dependencies. Its worked infrastructure examples are operationally direct: rail depends on power; repair crews depend on roads, fuel, cellular service and material supply. The implication is that recovery cannot be represented as a list of sector availabilities. It is a dependency graph whose topology changes after damage. See the [NIST Community Resilience Planning Guide, Volume I](https://www.nist.gov/system/files/community-resilience-planning-guide-volume-1.pdf) and [Volume II](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.1190v2.pdf).

The Department therefore needs two different definitions:

> **Path diversity** is the number of nominal ways to move an effect from origin to destination.

> **Assured independence** is the number of origin-to-effect chains that can lose any declared common dependency without losing the public service promise.

The first can be counted on a map. The second must be engineered, exercised and statistically demonstrated.

## The unit of design: an independently supportable campaign cell

A campaign cell is not a small task force assembled from a common rear area. It is a bounded sovereign operating system able to perform a declared public effect while adjacent cells are unavailable.

Every cell contains eight inseparable layers:

1. **Effect module** — the water, power, medical, communications, access, shelter, sanitation or hazard-control capability.
2. **Origin package** — protected inventory, loading, staging, workforce, energy and command outside the damaged theater.
3. **Strategic movement** — one or more modes with configuration-controlled loads and crews.
4. **Reception and onward movement** — mobile handling, no-pier or austere-air interfaces, route opening and local transfer.
5. **Zero-host-utility base** — power, water, food, sanitation, lodging, health protection and waste handling for responders.
6. **Sovereign information plane** — local sensing, allocation, identity, data provenance, spectrum management and offline mission command.
7. **Repair and technical authority** — diagnostics, spares, inspection, safety release, degraded-mode limits and independent reachback.
8. **Civil interface** — a predelegated mechanism for public priorities, consent, equity, property access, environmental constraints and transfer to legitimate local control.

If two cells share a non-substitutable instance of any of these layers, their independence credit must be discounted. Duplication of vehicles without duplication of enabling layers is inventory redundancy, not campaign redundancy.

This yields a stricter accounting rule:

```text
credited independent cells
  = minimum of
      effect-module independence
      origin independence
      movement independence
      reception independence
      host-utility independence
      information independence
      repair/authority independence
      civil-decision independence
```

The rule is intentionally unforgiving. Catastrophe exploits the weakest shared dependency, not the average quality of the fleet.

## Method

### Purpose and model boundary

The model asks a narrow question: under a common set of stochastic shocks, which of four rival architectures preserves the Pass 25 day-3, day-14 and sustainment promises?

It does not estimate earthquake occurrence, casualties, economic loss or infrastructure restoration. It does not use FEMA default fragilities as if they described the future Department's assets. FEMA's current [Hazus Earthquake Model Technical Manual](https://www.fema.gov/sites/default/files/documents/fema_hazus-earthquake-model-technical-manual-6-1.pdf) is used only as a methodological precedent for component fragility and utility/transport loss modeling.

### Common-random-number experiment

The workbook stores 500 fixed-seed standard-normal draw sets and applies the same draws to every architecture. This common-random-number design makes architecture comparisons less sensitive to chance differences between samples and allows every result to be reproduced cell by cell.

Each path-copy state is generated from a simple latent normal factor model:

```text
latent state
  = √ρsystem × Zsystem
  + √ρfamily × Zfamily
  + √(1 − ρsystem − ρfamily) × Zidiosyncratic
```

The latent state is compared with precomputed normal thresholds for three outcomes:

- failed: zero capacity;
- degraded: architecture-specific capacity fraction; or
- intact: full capacity.

There are distinct system and family shocks for day 3 and day 14. Families are distributed, air, maritime and surface. Eleven group-level correlation domains follow Pass 25: local distributed resources; north air; south air; vertical lift; Puget maritime; coastal maritime; inland water; Washington surface; Oregon surface; rail; and offshore support.

Five shared enablers receive their own three-state draws: energy, communications, qualified workforce, civil and technical authority, and repair/inspection. A path's delivered capacity is limited by the weakest of these enablers. This is a conservative screening representation; later network models should map each path to specific enabler instances rather than apply one common minimum.

### Closure standard

Campaign closure is the minimum of three tests:

**Day 3 force closure.** Local distributed supply meets its requirement. The reference and hardening cases also require each north-air, south-air and vertical path to meet its assigned demand. The duplicated and cellular cases can pool air capacity, but at least two air groups must remain usable.

**Day 14 service-island independence.** Every one of the nine zones must retain its Pass 25 minimum number of qualifying path groups. A group qualifies when effective capacity is at least 50 percent of its nominal day-14 capacity.

**Sustainment.** The capacity-weighted surviving network must clear the architecture's declared sustainment threshold.

The 95-percent campaign target is a normative design choice. It expresses the proposition that a coequal national instrument should be held to an explicit residual-risk standard. It is not drawn from statute or historical frequency and remains open to civil decision.

### Aftershocks are operational state, not background uncertainty

USGS operational aftershock forecasts estimate expected aftershock counts and the probability of damaging magnitude bands, and they update as a sequence evolves. A Department campaign model should therefore ingest a living forecast into inspection holds, route release, crew exposure, staging and redundancy decisions rather than bury aftershocks in one fixed derating factor. See the [USGS Operational Aftershock Forecasting overview](https://earthquake.usgs.gov/data/oaf/overview.php) and [update schedule](https://earthquake.usgs.gov/data/oaf/schedule.php).

Cascadia requires local calibration. USGS research on [Cascadia aftershock-sequence productivity](https://www.usgs.gov/publications/productivity-cascadia-aftershock-sequences) cautions that generalized global models can misrepresent local sequences. The workbook therefore does not claim a calibrated aftershock distribution; it identifies the data and operational interface that must be built.

## Rival architectures

| Architecture | Topology | Common-risk treatment | Day-3 substitution | Attributable capital delta |
| --- | --- | --- | --- | ---: |
| A — Pass 25 reference | One copy per group | Nominal path labels; concentrated support | No | $0B |
| B — hardened nodes | One stronger copy per group | Lower marginal failure and degradation | No | $74.5B |
| C — duplicated critical paths | Two smaller copies per group | More separate origin and enabler packages | Pooled air, two-group minimum | $141B |
| D — cellular campaign mesh | Three independently supported cells per group | Lower common-factor exposure, deliberate overcapacity and substitution | Pooled air, two-group minimum | $228B |

The costs are attributable planning hypotheses, not estimates. They are nested within the Pass 23 Department and Pass 24 deployment-enterprise lines. They should not be added to those totals.

## Results

| Architecture | Day 3 | All zones by day 14 | Sustainment | End-to-end closure | Approx. 95% half-width |
| --- | ---: | ---: | ---: | ---: | ---: |
| Pass 25 reference | 9.6% | 51.0% | 16.6% | **5.8%** | ±2.0 pp |
| Hardened nodes | 23.8% | 81.4% | 60.0% | **21.4%** | ±3.6 pp |
| Duplicated critical paths | 50.6% | 83.2% | 75.4% | **48.0%** | ±4.4 pp |
| Cellular campaign mesh | 85.0% | 93.6% | 92.2% | **84.2%** | ±3.2 pp |

The sequence matters.

First, **hardening is not independence**. Better nodes sharply improve the day-14 geographic screen, but a single instance of each path still leaves the campaign exposed to common enablers and day-3 threshold effects.

Second, **duplication changes the slope but not the endpoint**. Two smaller copies create useful substitution, yet campaign closure remains below one-half under the declared joint shocks. A second platform is not enough if both copies inherit the same systemic and family factors.

Third, **cellular architecture is qualitatively different**. The strongest case cuts system and family correlation, gives each group three smaller copies, carries overcapacity and pools day-3 air delivery. It closes 421 of 500 trials. Among the 79 failures, 75 are assigned first to day-3 force closure, none to the day-14 zone-diversity gate and four to sustainment.

That decomposition points to the next design problem. The regional network is no longer primarily constrained by the number of paths after day 14. It is constrained by the first 72 hours, when high demand, limited prepared handling capacity and shared enabler degradation coincide.

The cellular case adds a provisional $228B to the $373.44B Pass 25 regional attribution, yielding a $601.44B attributable architecture, and adds $14.7B per year to the earlier $34.2B mature operating slice. Relative to the reference case, its 78.4-percentage-point modeled improvement costs about $2.91B per percentage point. That ratio is descriptive, not an optimization result; no avoided-loss function is claimed.

## What the mature force should become

### From functional services to cell-generating services

The Department's seven operating services should still maintain professional depth, but readiness reporting should shift from platform or formation counts to certified cells. A service would be responsible not merely for producing aircraft, ships, power modules, protected-movement systems or hospitals, but for contributing complete cell layers with declared independence pedigrees.

A cell readiness record should include:

- its effect and time-to-service envelope;
- exact origin and alternate origin;
- movement and reception configurations;
- energy and communications sources;
- named crew pools and relief pools;
- repair parts, diagnostic authorities and depot relationships;
- civil and technical decision rights;
- common components and software dependencies shared with other cells;
- last full-mission trial and seeded losses survived; and
- the campaigns for which the cell can receive independent credit.

This becomes a national **campaign assurance ledger**. Joint planners allocate cells by covariance budget as well as capacity. Two units with identical nominal performance may receive different credit because one shares a software baseline, fuel terminal, workforce catchment or supplier with units already assigned.

### A Joint Campaign Assurance Command

The Department requires a functional command responsible for the reliability of the whole operating graph. This command should not own all assets. It should own the cross-service methods and decision rights that prevent false independence.

Its standing functions would be:

- maintain dependency and common-mode registers across every certified formation;
- allocate correlation budgets in campaign plans;
- run fixed and adaptive stochastic closure models;
- integrate current hazard forecasts into route, exposure and inspection policy;
- certify cell substitution and graceful-degradation rules;
- direct blind loss-of-node and loss-of-enabler exercises;
- recommend reserve release based on remaining independence, not inventory count; and
- publish a civilly understandable statement of residual service risk.

The independent technical authorities retain safety release. The Civil Resilience Authority retains public priority and risk-acceptance decisions. Campaign Assurance Command provides the joint evidence neither function can produce alone.

## Technology agenda for genuine independence

The new doctrine creates technology requirements that a conventional equipment catalogue would miss.

### 1. Containerized sovereign micro-utilities

Each cell needs modular power, water, sanitation, thermal management and energy storage that can start without the host grid or fuel network. The frontier is not a better generator. It is a certified black-start utility fabric with automated protection, common physical interfaces, safe islanding and machine-readable resource contracts.

### 2. Multi-fuel and fuel-light mobility

Common fuel dependence is a campaign-level vulnerability. Research should pursue multi-fuel turbines and engines where physically defensible, battery and hybrid ground systems for short-haul work, locally producible energy carriers, safe mobile charging, and allocation software that can move energy among mobility and public-service loads. The goal is not universal electrification; it is multiple substitutable energy chains.

### 3. Sovereign offline mission command

Cells require communications that can operate without commercial identity, cloud, timing or backhaul. The technology program includes delay-tolerant networking, local compute, multi-provider radios, portable spectrum coordination, trusted offline data packages, degraded positioning and human-readable manual fallback.

### 4. Configuration-aware autonomous logistics

Autonomous aircraft, surface craft and ground vehicles should be developed as a means of multiplying handling and last-mile capacity while reducing crew exposure. They must carry configuration provenance, operate under bounded authority, negotiate damaged networks and degrade safely when data links or navigation are lost. Autonomy credit is earned only through seeded-fault mission trials.

### 5. Rapid inspection and release systems

The 72-hour constraint is partly an epistemic problem: the force does not know which runway, channel, bridge, slope, pipeline or utility segment can safely carry load. Distributed sensing, robotic inspection, portable nondestructive evaluation, structural digital twins and probabilistic release tools can convert uncertainty into usable capacity. They also need an explicit technical authority willing and able to issue bounded releases.

### 6. Common-function, diverse-implementation components

Interoperability and correlated risk pull in opposite directions. A universal component can simplify logistics while grounding the entire force. The Department should standardize interfaces, data contracts and performance envelopes while funding diverse implementations for critical components. Two cells may interoperate without sharing the same vulnerable controller, firmware, pump seal or power electronic module.

### 7. Mobile micro-depots and additive repair

Cells need diagnostic, fabrication and repair depth close to the theater. Research should test mobile metrology, additive repair, certified substitute parts, automated inventory sensing and remote technical support under disconnected conditions. The relevant metric is time to return a complete public-service chain to operation, not the number of parts printed.

### 8. Dynamic covariance-aware allocation

Campaign software should continuously update which cells still count as independent as aftershocks, weather, congestion, cyber incidents, crew availability and repair status change. This requires explicit dependency data, causal rather than merely correlational failure models, interpretable recommendations and a human authority model for reallocating scarce public service.

## Industrial architecture

A cellular force should not be delivered by one vertically integrated prime whose common subsystems become national single points of failure. The industrial model should deliberately combine:

- multiple cell integrators with common government-owned interfaces;
- second-source requirements for critical components;
- regional production and depot capacity outside shared hazard footprints;
- government reference implementations and conformance test harnesses;
- continuous production at readiness-sustaining rates;
- competitive upgrade lanes that preserve interchangeability; and
- an independent common-mode review before any design becomes ubiquitous.

This is a different use of industrial policy from buying more inventory. It creates **productive diversity**: enough commonality to combine forces, enough implementation diversity to prevent one defect, supplier, cyber compromise or industrial accident from disabling the national response instrument.

The export proposition also changes. The valuable product is not a giant U.S.-specific platform. It is a family of sovereign, modular campaign cells; open interface standards; training and assurance methods; and regionally manufacturable subsystems that partner nations can adapt without accepting permanent dependence on U.S. cloud, fuel or depot infrastructure.

## Research and test campaign

The next evidence program should proceed in six linked stages.

### Stage 1: build the dependency census

Inventory every Pass 25 path, node, formation and service chain at asset level. Record physical location, suppliers, energy, data, labor catchment, licenses, repair relationships, software, common components and alternate modes. The output is a directed dependency graph with explicit ownership and uncertainty.

### Stage 2: fit joint damage and recovery distributions

Use route and node surveys, Hazus-compatible component methods, utility records, exercises and geographically resolved hazard fields to replace workbook priors. Recovery distributions must include inspection queues, repair resources and aftershock holds—not only initial physical damage.

### Stage 3: build representative cells

Construct at least three rival origin-to-effect cells for the binding day-3 air mission and two for no-pier/shallow-draft reception. Give them deliberately different energy, communications, control and repair implementations.

### Stage 4: seed common-mode losses

Exercise loss of a fuel terminal, data provider, identity service, airspace system, supplier part, crew pool, technical authority and safe-zone base. Evaluators should withhold some failures from operators and modelers until execution.

### Stage 5: run the complete Cascadia thread

Combine current USGS forecast injects, winter weather, multiple service islands, public-priority changes, responder sustainment, patient movement, waste and reconstitution. Measure population-service-time delivered, not sorties or tonnes alone.

### Stage 6: replicate on unfamiliar terrain

Repeat the method for an invited overseas campaign with different law, port geometry, disease burden, power standards, language, industrial capacity and host-state authority. A design that works only because it quietly assumes U.S. institutions has not demonstrated strategic force projection.

Fourteen workbook gates remain open. No platform or vehicle rendering is authorized by this pass.

## Limits and falsification

This model should be rejected or materially revised if:

- measured marginal failure or degradation distributions differ enough to reverse architecture ranking;
- path-to-enabler mapping shows the common-minimum treatment is materially too conservative or not conservative enough;
- capacity loss is continuous or state-dependent in a way the three-state representation cannot approximate;
- cell copies cannot be made operationally separate because of workforce, supplier, airspace or authority constraints;
- pooling creates congestion, unsafe control burdens or incompatible mission packages;
- the 95-percent assurance target is replaced through legitimate civil decision;
- full-mission trials show that day-3 demand, handling or service thresholds are wrongly specified; or
- independent replication cannot reproduce the architecture result.

The 500-trial run is adequate for screening large differences, not tail certification. The half-width calculation assumes independent Bernoulli trials and does not capture parameter uncertainty. The Gaussian factor structure captures common movement but not every tail dependence, cascading failure or adaptive decision. The model therefore remains `R2+` arithmetic inside an `R2` campaign architecture.

## Strategic consequence

The mature Department of Resilience should project not a collection of benevolent platforms but a network of sovereign service cells that can be composed, separated, substituted and regenerated under continuing hazard.

That is a more ambitious institution than a national emergency agency and a more demanding engineering project than a fleet procurement. It requires a standing science of civil campaign assurance; government-owned interface standards; multiple industrial lineages; distributed origins and depots; new professions in dependency engineering and public-service mission command; and repeated destructive proof.

Pass 25 showed what must arrive. Pass 26 shows that the force is not ready merely because a plan contains many arrows. It is ready only when the arrows remain valid after the systems behind them begin to fail.
