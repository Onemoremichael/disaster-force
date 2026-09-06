# Quantitative model library

The workbooks are executable design arguments. They connect public demand to capacity, configuration, mass, energy, workforce, readiness, industrial scale, cost, uncertainty, and evidence gates. They are built for inspection and sensitivity analysis; they are not independent cost estimates, acquisition baselines, forecasts, or proof that a proposed system will work.

The library now mirrors the research proof architecture instead of placing every workbook in one flat directory:

```text
models/
├── mandate/                 national system requirements
├── force/                   generation, projection, reception, and mobility
├── systems/                 complete civil-service and technical chains
├── proving/                 campaigns and the test enterprise
└── programmatics/           Department-scale resource consequences
```

This is more than file organization. It identifies the decision each workbook is allowed to influence. A campaign model cannot certify component physics; a force-allocation model cannot validate a field rate; a reconciled budget cannot reduce a public-service requirement simply because the resulting institution is large.

The complete [model catalog](CATALOG.md) links every workbook to its owning paper, current use, maturity, and supersession status.

## How to inspect a model

Begin on the `Executive`, `Read Me`, or control sheet. Identify the service promise and the decision the model owns before examining the top-line result. Then distinguish four kinds of information inside the workbook: source-backed observations, declared design assumptions, calculated quantities, and evidence gates.

Change only designated inputs, inspect the linked balances and scenarios, and read the checks and sources alongside the result. A plausible top line is insufficient. Configuration must also close deployment time, distribution, interfaces, workforce, maintenance, degraded modes, safety, waste, civil transfer, and the complete public-effect chain.

An intentional `OPEN` check identifies a research contradiction or missing proof; it is not a spreadsheet defect. All monetary values are real 2026 U.S. dollars unless a workbook states otherwise.

## What the lineage means

Later models often break or supersede one conclusion while preserving the earlier workbook as a lower bound, sensitivity surface, or historical control. The central lineage runs from Department scale through force allocation and deployment; from service-entry mass through occupied population systems and civil mobility; and finally into the neighborhood formation now being tested in New York.

```text
DEPARTMENT SCALE
      ↓
FORCE ALLOCATION → DEPLOYMENT ENTERPRISE
      ↓                    ↓
CASCADIA CLOSURE → COVARIANCE FAILURE
      ↓
SERVICE-ENTRY FORCE → INDIVISIBLE POD
      ↓
OCCUPIED DISTRICT → RECEIVING GEOGRAPHY → CIVIL MOBILITY
      ↓                                      ↓
LOCAL PROTECTION ───────────────────────→ NCAC-35
                                             ↓
                        NEW YORK PREREGISTRATION AND L0 CONTROLS
```

Budgets are not automatically additive. Several workbooks allocate, deepen, or stress capacity already carried by a parent force. The original $1 trillion force-capital constraint, the domain-specific $1 trillion fire and flood experiments, the $130 billion flood research program, the selected $2 trillion technology case, and the $320 billion proving-network cross-classification are distinct analytical frames.

Most configurations remain at `R2+`: more detailed than a bounded concept, but still awaiting representative hardware, solved site cases, verified rates, reliability evidence, and independent full-mission trials. Platform renderings remain blocked until physics and evidence close at `R3`.
