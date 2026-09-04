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
