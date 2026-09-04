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
