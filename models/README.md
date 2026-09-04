# Models

Quantitative work is delivered in the editable [`disaster-force-model.xlsx`](disaster-force-model.xlsx) workbook. The model is a design-study instrument, not an independent cost estimate, budget request, forecast, or official benefit-cost analysis.

Version 0.1 includes:

1. Assumptions and scenario control
2. Mission demand and concurrency
3. Concurrency-driven force inventory and availability
4. Bottom-up program portfolio and capital reconciliation
5. Workforce, reserve structure, attrition, and accessions
6. A 25-year capital and operating-resource plan
7. Mature annual operating cost by service/component
8. Industrial capacity and learning-curve diagnostics
9. Benefits and avoided-loss scenarios
10. Sensitivities, integrity checks, sources, and version history

The reference case keeps the user-specified $1 trillion capital tranche separate from personnel and operations. Current full-force assumptions produce a roughly $2.24 trillion bottom-up portfolio and therefore leave the workbook in `REVIEW`; the mismatch is visible rather than hidden by a plug.

See [`research/16-quantitative-model.md`](../research/16-quantitative-model.md) for equations, output interpretation, verification state, and the next research requirements. No model output should be treated as evidence unless its inputs are sourced or explicitly marked as design-study assumptions.

## WRG-50 engineering model

[`water-restoration-engineering.xlsx`](water-restoration-engineering.xlsx) converts the Regional Water Works and Rapid Water Grid into a 13-sheet configuration study. It links delivered demand, three source-treatment cases, Darcy–Weisbach hydraulics, four reference pressure zones, pipe geometry and mass, storage and access nodes, wastewater and residuals, construction modes, lift, workforce, failure cases, sources, and the R3 rendering gate.

The default seawater case produces approximately 23,500 tonnes of preliminary deployment mass before stored water, 14.75 MW of installed treatment-plus-conveyance capacity after reserve, 47,900 m³ of storage, 2,720 deployed people, and a 19.7-day rapid-surface construction target. Most equipment masses and all construction rates remain explicit assumptions. The workbook remains `R2+`; passing model checks is not physics verification.

See [`research/18-water-configuration-model.md`](../research/18-water-configuration-model.md) for equations, output interpretation, verification and open engineering evidence.

## PRG-100 engineering model

[`power-restoration-engineering.xlsx`](power-restoration-engineering.xlsx) converts the Power Restoration Group into a 17-sheet deployable-utility configuration study. It links an illustrative 100 MW critical-load registry, reuse/bypass/rebuild network states, three source cases, generation reserve, battery duties, feeder current and loss, mobile transformation, rapid distribution, fuel, thermal protection, deployment mass, workforce, failures, sources and the R3 gate.

The default bypass/liquid-fuel-dominant case produces 103.89 MW of average gross dispatch, 140 MW of owned generation, 140 MW / 140 MWh of storage, eight 25 MVA mobile substations, 60 circuit-km of temporary network, 18,332 tonnes of preliminary dry deployment mass, 2,796 deployed people and 152,461 gallons/day of liquid fuel. Reuse lowers modeled dry mass to 13,932 tonnes and 6.3 setup days; rebuild raises it to 30,757 tonnes and 39.3 days. A gas-hybrid case lowers liquid demand to 47,644 gallons/day while creating a 12,343 MMBtu/day gas dependency.

All equipment masses, construction rates, staffing coefficients and thermal intensities remain explicit design-study assumptions. The workbook is `R2+`; it is not an electrical construction design, transport plan, cost estimate or verified performance claim.

See [`research/21-power-configuration-model.md`](../research/21-power-configuration-model.md) for equations, scenario interpretation, verification and open evidence.

## Fire response force engineering model

[`fire-response-force-engineering.xlsx`](fire-response-force-engineering.xlsx) converts the Ignition Intercept Network and Integrated Fire Control Group into a 23-sheet configuration study. It links three formation states, four fire cases, complete intercept clocks, fire-growth screens, aircraft cycles, airspace and base capacity, water and agent constraints, aerial and ground control line, robotics, structure defense, smoke/thermal protection, deployment mass, workforce, national readiness, technology campaigns, capital, failure modes and 18 R3 evidence gates.

In the default WUI campaign case, the IFCG produces 798.28 effective sorties and 411.80 km/day of effective line, giving a +4.77 km/h closure margin and a 10.64-hour screening closure time after a P90 arrival of 135.4 minutes. Its preliminary dry deployment is 42,339 tonnes, with 12,330 deployed people and a 46,237.5-billet service establishment. The same case shows why the Department needs a separate distributed force: an intercept cell reaches an 81.2% modeled probability of action before the 50-minute escape threshold, while the campaign formation reaches 33.4%.

The model is assumption-driven. Its fire growth, arrival distribution, aircraft yield, robot productivity, line hold, public protection, readiness and cost relationships are test requirements, not performance claims. `IIN` and `IFCG` are `R2+`; no vehicle or system is authorized for rendering.

See [`research/23-fire-configuration-model.md`](../research/23-fire-configuration-model.md) for equations, results, scenario interpretation, technology priorities, verification and open evidence.

## Flood hydraulic-control engineering model

[`flood-hydraulic-control-engineering.xlsx`](flood-hydraulic-control-engineering.xlsx) converts the Flood Intercept Network and inland/coastal Hydraulic Control Groups into a 29-sheet configuration study. It links three formation states, five flood cases, complete forecast-to-effective-action clocks, basin zones, a 45-day storage balance, four pump families, intake and debris derating, power, the Rapid Drainage Spine, receiving-water constraints, barriers, interior drainage, breach arrest, rescue demand, five amphibious classes, wet-gap logistics, earthworks, contamination, infrastructure protection, deployment mass, workforce, readiness, works carriers, technology campaigns, capital, failure modes and twenty R3 gates.

In the default trapped-urban-basin case, the Inland HCG-100's 100 m³/s nominal portfolio becomes 36.551 m³/s effective flow after unit availability, head, intake/debris and 75% formation operating utilization. It produces +16.051 m³/s day-zero net removal and drains the assumed 75 million m³ basin in 28 modeled days. The same configuration has a −14.01 m³/s protected-side drainage margin, demonstrating that barrier interior drainage is a separate requirement. Its preliminary dry deployment is 79,391 tonnes, approximately 66,844 tonnes require external lift, and its workforce screen is 7,039 deployed people / 26,394 service billets.

Across all 15 formation–case combinations, pump/intake and formation utilization bind before route, receiving-water or power capacity under the selected assumptions. FIN frequently acts before the hazard threshold while lacking positive hydraulic reversal; the HCG can reverse the trapped-basin case but does not beat flash or breach thresholds. The 12 m × 3 m breach screen produces 165.7 m³/s initial flow, 9.2–9.7 times degraded HCG pumping, preserving breach arrest as an upstream mission rather than treating pumping as a universal answer.

All hydraulic cases, equipment values, readiness, staffing, cost and technology coefficients are explicit design-study assumptions. The workbook is not a civil-works design, incident forecast, environmental authorization, navigation plan, acquisition estimate or verified performance claim. `FIN` and `HCG-100` are `R2+`; all twenty evidence gates remain open and no flood system is authorized for rendering.

See [`research/25-flood-configuration-model.md`](../research/25-flood-configuration-model.md) for equations, results, scenario interpretation, technology priorities, verification and open evidence.

## Flood research, test and evaluation model

[`flood-research-test-evaluation.xlsx`](flood-research-test-evaluation.xlsx) converts the flood force's technological ambition into a 17-sheet, 25-year invention and proof campaign. It links editable controls, ten `ARPA-R` technology campaigns, an independent integration/test line, 46 experiment packages, twenty R3 evidence gates, ten purpose-built range families, annual funding, facility throughput, competing prototype cohorts, TRL/MRL transitions, four detailed protocol families, eight complete mission-thread trials, decision rights and cost/schedule failure sensitivity.

The baseline reconciles to the existing $130B flood RDT&E allocation: $24B for the National Hydraulic Proving Network and $106B for science, prototypes, field trials, data, standards and transition. Protected independent integration and T&E is $13B, exactly 10% of the envelope. The annual profile peaks at approximately $11.32B in year 8. The modeled cohort begins with 54 rival technical paths and narrows to 43 at TRL 5, 30 at TRL 6 and 20 entering TRL 7. Parallel/distributed ranges hold average planned peak utilization to 75.82% under an 80% planning ceiling.

A compound 25% facility, 15% redesign, two-year delay and 15% integration shock raises calculated need to $156.25B, $26.25B above the RDT&E envelope; the separate $25B program reserve is short by $1.25B. This is a sensitivity, not a forecast or estimate. It demonstrates why `ARPA-R` needs genuine cancellation authority and why `RTEA` evidence cannot be negotiated away by sunk cost.

All 46 performance thresholds are research hypotheses. The workbook is not a statistical power analysis, range design, safety case, environmental authorization, independent cost estimate or acquisition baseline. All twenty flood evidence gates remain open, `FIN` and `HCG-100` remain `R2+`, and no flood system is authorized for rendering.

See [`research/26-flood-research-test-and-evaluation.md`](../research/26-flood-research-test-and-evaluation.md) for the institutional doctrine, test philosophy, facility architecture, experiment design, mission-thread logic, portfolio interpretation and source notes.

## Department-wide technology frontier model

[`resilience-technology-frontier.xlsx`](resilience-technology-frontier.xlsx) generalizes the invention-and-proof architecture across the Department of Resilience. Its 16 sheets link three alternative 25-year funding cases, twelve mission-science directorates, eight institutional channels, sixty measured technology campaigns, ten common technological primitives, a 240-to-20 maturity funnel, ten proving-range families, annual funding, independent stage gates, decision rights, industrial clusters, export pathways and cost/schedule sensitivity.

The workbook distinguishes a $750B catalytic case, selected $2T strategic case and rounded $4.5T peer-intensity case. Peer intensity is contextualized by the FY2026 defense RDT&E request of $179.1B, not asserted as a resilience cost estimate. In the selected case, `ARPA-R` receives $480B, National Resilience Laboratories $440B, the 58-site National Resilience Proving Network $320B, protected independent `RTEA` $200B, Service Technology Commands $240B, the Manufacturing and Mobilization Administration $200B, university consortia $80B and standards/data/public assurance $40B. These are two classifications of one envelope, not additive budgets.

The funding profile averages $80B/year and peaks at approximately $139.81B in years 9 and 10. A compound facility, redesign, integration, two-year delay and supply-chain shock raises calculated need to $2.494T; the 15% / $300B reserve is short by $194B. Seventeen arithmetic and architecture checks pass and one informational line intentionally flags that shortfall. All future performance values remain design hypotheses, no campaign receives R3 operational credit and no vehicle or platform is authorized for rendering.

See [`research/27-resilience-technology-frontier.md`](../research/27-resilience-technology-frontier.md) for the institution, technology taxonomy, proving doctrine, civil constraints, industrial implications and source notes.
