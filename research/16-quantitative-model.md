# Quantitative model: force, capital, workforce, and operating scale

## Purpose

The initial workbook converts the qualitative Department of Resilience architecture into an auditable numerical hypothesis. It is designed to answer five questions:

1. What owned inventory follows from the `3C + 5M + 2G + 20R` concurrency standard?
2. What might a broad purpose-built program portfolio cost under explicit concept-study assumptions?
3. How large a workforce and annual operating establishment would be required to keep that inventory ready?
4. How would a 25-year build distribute capital and operating obligations through time?
5. Which conclusions remain robust when capital, operating, demand, cost, and benefit assumptions change?

The model is not an independent cost estimate, budget request, forecast, or benefit-cost analysis. It is a transparent research instrument that makes implicit scale choices visible and replaceable.

The editable workbook is [`disaster-force-model.xlsx`](../models/disaster-force-model.xlsx).

## Model structure

| Sheet | Role |
|---|---|
| Summary | Selected case, force and resource scale, material warning, and annual capital/operating trajectory |
| Assumptions | Low, reference and high cases; concurrency; operating controls; annual capital weights; force ramp |
| Mission Demand | Ten design reference missions expressed as affected population, support share, duration, access, water, energy, clinical, and debris demand |
| Force Sizing | Campaign-package coefficients, simultaneous demand, residual reserve, availability, and owned inventory |
| Portfolio | Program quantities, average unit costs, non-recurring engineering, bases/tooling, risk allowance, and capital reconciliation |
| Workforce | Active and reserve structure, personnel burden, career length, attrition, accessions, and annual personnel cost |
| 25-Year Plan | Capital deployment, force growth, personnel, asset support, training, deployments, and cumulative resource requirement |
| Operating Cost | Mature annual cost by service and institutional component |
| Industrial Base | Production years, assumed dedicated capacity, capacity multiple, learning rate, and a diagnostic learned-cost calculation |
| Benefits | Illustrative event probability, severity, addressable share, effectiveness, avoided loss, and present value |
| Sensitivity | Formula-driven operating-cost and avoided-loss matrices |
| Checks | Reconciliations, bounds, inventory coverage, source count, and model status |
| Sources | Official references, project assumptions, scope notes, and version history |

Blue-on-tan cells are editable inputs. Green cells are cross-sheet formulas. Black cells are same-sheet calculations. One selector changes the low, reference, and high cases.

## Core equations

### Ready force and owned inventory

For capability family (i):

```text
simultaneous demand_i = 3 × catastrophic package_i
                      + 5 × major package_i
                      + 2 × global package_i

ready requirement_i = simultaneous demand_i × (1 + 20%)

owned inventory_i = round up(ready requirement_i / availability_i)
```

This makes the inventory consequence of concurrency and mission availability explicit. It does not yet derive each package coefficient from the full population-service-time demand table; that is the most important unresolved link.

### Program capital

For program family (i):

```text
gross program_i = quantity_i × average unit cost_i × selected cost multiplier
                + non-recurring engineering and test_i
                + bases and tooling_i

total program_i = gross program_i × (1 + risk allowance_i)
```

Average unit cost is an editable concept-study input. It is not a bid, analogous-platform estimate, or validated cost-estimating relationship. Non-recurring engineering, bases, tooling, spares, mission modules, and program risk are visible rather than hidden inside one unit-cost number.

### Mature annual operations

```text
annual operating requirement = active and reserve personnel
                             + installed asset base × asset O&M rate
                             + training and stock rotation
                             + average deployment allowance
                             + other institutional cost
```

The capital tranche and recurring operating establishment remain separate. Treating the user-specified $1 trillion as though it also purchased 25 years of people, maintenance, training, deployments, stock rotation, schools, depots, and science would materially understate the institution.

### Illustrative avoided loss

```text
expected gross annual loss_j = annual probability_j × loss if event_j

annual avoided loss_j = expected gross annual loss_j
                      × addressable share_j
                      × selected effectiveness_j
```

The calculation is deliberately narrow. It excludes unpriced strategic access, humanitarian obligations, public confidence, distributional outcomes, ecosystem preservation, industrial learning, export capacity, and deterrence-like value. Probability, severity, addressability, and causal effectiveness are design assumptions rather than official estimates.

## Reference-case outputs

The reference case currently produces:

| Output | Reference result | Interpretation |
|---|---:|---|
| Top-down capital tranche | $1.00 trillion | User-specified 25-year reference envelope in real 2026 dollars |
| Bottom-up concept portfolio | $2.24 trillion | Full concurrency inventory under current illustrative quantities and costs |
| Capital reconciliation gap | $1.24 trillion | Unfunded difference; model status remains `REVIEW` |
| Mature active workforce | 302,000 FTE | Seven service/institutional components |
| Mature reserve workforce | 396,500 people | Different reserve ratios by component |
| Annual accessions at maturity | about 29,700 | Career-length and attrition replacement requirement |
| Mature personnel cost | about $99.1 billion/year | Active plus paid reserve assumptions |
| Mature annual operating requirement | about $187.9 billion/year | Personnel, O&M, training, deployment, and institutions |
| 25-year capital plus operating resources | about $4.44 trillion | Undiscounted real-dollar build-period total |
| Monetized avoided loss | about $30.8 billion/year | Partial scenario value, not a comprehensive benefit estimate |
| 25-year present value of modeled avoided loss | about $535.5 billion | Three-percent real discount rate; assumption-driven |

The most important output is the gap, not a false point estimate. The initial $1 trillion tranche does not buy the complete force implied by the current concurrency packages and cost assumptions. Closing the gap requires one or more of four explicit choices:

1. increase the capital envelope;
2. reduce the concurrency promise;
3. reduce owned inventory through higher availability, allied pools, or assured industrial/commercial capacity;
4. lower program cost through different concepts, common platforms, modularity, learning, or reduced requirements.

The model does not choose among them. It makes the trade visible.

## What the current numbers do and do not mean

The output does not establish that the mature Department “costs $2.24 trillion.” The number is a consistency test across a large provisional portfolio. It is especially sensitive to:

- carrier, sealift, medical ship, airlift, and nuclear water–energy concepts;
- per-campaign aircraft and mission-package coefficients;
- mission availability, which converts ready demand into owned inventory;
- whether strategic lift, bases, and stocks are sovereign, assured, reserve, commercial, or allied;
- whether the Department buys complete formations or counts equipment without people and sustainment; and
- concept unit costs that have not passed engineering definition or independent estimation.

The workforce result is also a force-design hypothesis. It indicates the institutional order of magnitude created by complete crews, shifts, maintenance, engineering, healthcare, community stabilization, acquisition, science, schools, depots, and logistics. It is not derived from current agency staffing and should not be used as a transition headcount.

The operating result demonstrates a structural fact even if its point estimate changes: a serious standing force creates an annual readiness obligation larger than the average annual capital tranche. The mature institution cannot be financed as a temporary construction program.

## Scenario behavior

The workbook's control test verifies that the case selector changes capital, demand, unit-cost, workforce, and benefit-effectiveness multipliers:

| Case | Capital envelope | Active FTE | Bottom-up portfolio |
|---|---:|---:|---:|
| Low | $750 billion | 256,700 | about $1.97 trillion |
| Reference | $1.00 trillion | 302,000 | about $2.24 trillion |
| High | $1.50 trillion | 377,500 | about $2.60 trillion |

This is not a conventional low/base/high cost confidence interval. Each case represents a different force ambition and cost environment. A future model should separate demand uncertainty, technical cost risk, policy scope, schedule, and inflation into independent dimensions.

## Industrial interpretation

The industrial sheet turns quantities into required average production rates and compares them with editable assumptions about dedicated annual capacity. It also applies a simple learning-rate diagnostic. The result is intended to identify where the program would require new yards, factories, suppliers, schools, test facilities, certification capacity, and skilled trades.

The learning calculation is not used as the controlling portfolio cost because a first-to-nth-unit curve cannot represent configuration change, block upgrades, spares, facilities, program delay, concurrency, material constraints, or contracting strategy. Later passes should build cost-estimating relationships at the subsystem level and separate development, tooling, procurement, initial spares, military construction equivalents, and recapitalization.

## Verification state

The saved workbook contains no detected spreadsheet error values. Twelve of thirteen model-integrity checks pass. The remaining check correctly reports `REVIEW` because the bottom-up portfolio exceeds the selected top-down envelope by more than the stated tolerance. Low, high, and reference control cases were exercised after export and restored to reference.

## Next model work

1. Derive campaign package coefficients directly from population-service-time demand, throughput, cycle time, setup, distribution, and duration.
2. Replace concept unit costs with sourced parametric ranges, reference-class forecasts, and independent risk distributions after requirements mature.
3. Separate sovereign core, assured industrial, mobilization reserve, commercial, and allied inventory in the force-sizing equation.
4. Add platform age, maintenance, depot, attrition, overhaul, block upgrade, and recapitalization schedules.
5. Build occupation-level workforce, school capacity, qualification time, shift, rotation, and reserve activation models.
6. Model geographic posture and lift as a damaged-network problem rather than a national aggregate.
7. Replace the avoided-loss scenario with service-specific mortality, morbidity, displacement, downtime, productivity, and distributional benefit functions, with explicit double-counting controls.
8. Use probabilistic ranges only after each uncertainty has a defensible distribution or structured expert-judgment protocol.

These steps should precede the first vehicle rendering. The model should determine which system concepts advance to physics closure, not rationalize concepts already selected for visual appeal.
