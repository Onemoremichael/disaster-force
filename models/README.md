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

The [National Formation Registry](force/generation/national-formation-registry.xlsx) governs force identity and evidence state. The [Canonical Force Allocation](force/generation/canonical-force-allocation-model.xlsx) is its first national quantitative successor: it sizes all forty-eight families, disaggregates the legacy utility line, exposes shared-system credits, reproduces the predecessor baseline and reruns workforce, capital, movement, reception and sustainment screens. Its $15.179T capital and 10.484M affiliated-billet results are planning contradictions, not estimates. The [Household Collection Group model](force/generation/household-collection-group-model.xlsx) then attacks the dominant line from workload upward. It separates a 5,076-person, seven-company mobile origin formation from prepared district and heavy support contracts, showing why mobile mass can fall 71 percent while complete assigned mass and capital do not. The [Shared Capacity Allocation Ledger](force/generation/shared-capacity-allocation-ledger.xlsx) expands all forty-eight families across ten campaigns and enforces conservation against quantified pools. It shows why accounting credits cannot remove 2.011 million gross responders from the basing demand or 6.677 million early tonnes from the movement demand. The [Canonical Cargo and Transport model](force/projection/canonical-cargo-and-transport-model.xlsx) then turns that mass into ten external position classes and deadline-mode claims. Its 25.5-percent physical delivery becomes only 13.0-percent complete-formation closure, and every receiver remains unquantified. The [Carrier–Node Requirement and Program model](force/projection/carrier-node-requirement-and-program-model.xlsx) converts the same demand into three rival strategic-mobility envelopes. The smallest declared case still requires 10.048 million tonnes of gross 72-hour potential, 517 carrier groups, 296 transfer nodes and a $5.222T 25-year carrier-and-node program. Its inputs are clean-sheet design hypotheses and its receiver admission remains zero. The [`WRG-50` Serial Manifest and Admission model](force/projection/wrg50-serial-manifest-and-admission-model.xlsx) then expands one water formation into 690 planning objects. A 120-tonne surface target fits 686 after density floors and closes five of six complements, but all dispatch and receiver admissions remain zero under the twenty-eight-field release protocol. The [First-Reach Water Competition model](force/projection/wrg-fr10-first-reach-technology-competition.xlsx) converts its invalid pipe-volume claim into four live rival configurations. The complete-system dry range is 3,862–4,228 tonnes, the declared line schedule is 78–152 hours, the program base is $110.4 billion over twenty-five years, and all strict service and rendering admissions remain zero. The [First-Reach Degraded-Service Architecture model](force/projection/wrg-fr10-degraded-service-architecture.xlsx) then separates zero trunk inflow from accessible service, represents storage charge state, and tests centralized, parallel, bypass and route-separated topologies. The declared leader passes six of seven worlds but fails a receiver-wide hold. The [Federated Receiver Architecture model](force/projection/wrg-fr10-federated-receiver-architecture.xlsx) decomposes that hold into independent distribution, branch, power, quality, storage, source, access and authority boundaries. Its four rivals pass one, three, eight and nine of ten declared worlds. The [Unknown-Agent Water Assurance model](force/projection/wrg-fr10-unknown-agent-water-assurance.xlsx) distinguishes nondetection from qualified provenance. Its centralized, field-negative, reserve-backed and dual-continuous rivals safely sustain the floor in two, three, ten and eleven of twelve declared worlds respectively; the field-negative rival also exposes seven unsafe issue worlds. All strict admissions remain zero.

The [Assurance-Source Family Competition](force/projection/wrg-fr10-assurance-source-family-competition.xlsx) replaces generic provenance with four complete source chains. Coastal, groundwater, inland-treatment and sealed-transfer families pass two, four, one and nine of twelve worlds; the national quartet covers ten and retains two eligible sources in six. The mixed twenty-four-chain comparator is $208.75 billion over twenty-five years. Thirty-five integrity checks pass, four sensitivities react, all strict admissions remain zero and rendering stays blocked.

The [Closed-Loop Water Endurance model](force/projection/wrg-fr10-closed-loop-water-endurance.xlsx) converts that portfolio's two common failures into four competing endurance architectures. Carry-and-contain, regeneration/dewatering, quality-segmented service and a circular source cell all close the original fourteen-day residual and thirty-day consumable cases. Only `E2` and `E4` close both denials together; both fail at 75 percent of the inherited 2 MW power allocation. Incremental twenty-four-chain comparators span $46.88–145.0 billion over twenty-five years. Fifty integrity checks pass, four sensitivities react, all strict admissions remain zero and rendering stays blocked.

The [End-to-End Service-Chain Independence model](force/projection/wrg-fr10-end-to-end-independence.xlsx) registers twelve failure domains across source, treatment, carrier, node, power, quality, receiver, process materials, crew, depot, control and mobilization. Source-only, split-deployment and paired-chain architectures pass four, six and eleven of sixteen service worlds. A three-cell upper comparator passes all sixteen and the universal stop, but no architecture is admitted. The declared twenty-five-year range is $283.52–599.76 billion; sixty integrity checks pass, four sensitivities react and twenty evidence gates remain open.

The [Cellular Power and Thermal Independence model](force/projection/wrg-fr10-cellular-power-and-thermal-independence.xlsx) replaces that upper comparator's three power placeholders with central, isolated, hybrid and multi-vector utility architectures. The first three pass seven, ten and twelve of sixteen service worlds but qualify no complete cells. `P4` qualifies all three, passes all service worlds and the lawful stop, and reconstructs the formation at 11,250 dry tonnes, 12,960 chargeable tonnes and 598 crew. Its $232.80 billion replacement power program raises the whole comparator to $796.88 billion. Eleven sheets, four live stress changes, sixty integrity checks and a zero-error scan reconcile; twenty evidence gates and the campaign-energy wet load remain open, so admission and rendering stay blocked.

## How to inspect a model

Begin on the `Executive`, `Read Me`, or control sheet. Identify the service promise and the decision the model owns before examining the top-line result. Then distinguish four kinds of information inside the workbook: source-backed observations, declared design assumptions, calculated quantities, and evidence gates.

Change only designated inputs, inspect the linked balances and scenarios, and read the checks and sources alongside the result. A plausible top line is insufficient. Configuration must also close deployment time, distribution, interfaces, workforce, maintenance, degraded modes, safety, waste, civil transfer, and the complete public-effect chain.

An intentional `OPEN` check identifies a research contradiction or missing proof; it is not a spreadsheet defect. All monetary values are real 2026 U.S. dollars unless a workbook states otherwise.

## What the lineage means

Later models often break or supersede one conclusion while preserving the earlier workbook as a lower bound, sensitivity surface, or historical control. The central lineage runs from Department scale through force allocation and deployment; from service-entry mass through occupied population systems and civil mobility; and finally into the neighborhood formation now being tested in New York.

```text
DEPARTMENT SCALE
      ↓
FORMATION REGISTRY → FORCE ALLOCATION → SHARED-CAPACITY LEDGER → CANONICAL CARGO → CARRIER–NODE ENTERPRISE → WRG-50 SERIAL ADMISSION → FIRST-REACH COMPETITION → DEGRADED-SERVICE ARCHITECTURE → FEDERATED RECEIVERS → UNKNOWN-AGENT ASSURANCE → ASSURANCE-SOURCE FAMILIES → CLOSED-LOOP ENDURANCE → END-TO-END INDEPENDENCE
      ↓                    ↓                    ↑
                         HCG-35B ───────────────┘
CASCADIA CLOSURE → COVARIANCE FAILURE
      ↓
SERVICE-ENTRY FORCE → INDIVISIBLE POD
      ↓
OCCUPIED DISTRICT → RECEIVING GEOGRAPHY → CIVIL MOBILITY
      ↓                                      ↓
LOCAL PROTECTION ───────────────────────→ NCAC-35
                                             ↓
                        NEW YORK PREREGISTRATION AND L0 CONTROLS
                                             ↓
                                TARGET ENGINE v1 REPAIR FAILURE
                                             ↓
                              STRUCTURAL ENGINE v2 CALIBRATION FAILURE
                                             ↓
                           MOMENT ENGINE v3A: LINEAR FEASIBILITY,
                              NONLINEAR CIVIL-STATE FAILURE
                                             ↓
                           ATOMIC BASIS v3B0: POINT FEASIBILITY,
                              EXTREME NONIDENTIFICATION
                                             ↓
                         ATOMIC MOMENT-CONE AUDIT v3B1A:
                           EXACT MOMENT CLONING IMPOSSIBLE
                                             ↓
                       ATOMIC POSTERIOR PREREGISTRATION v3C0:
                       12 CASES · 25 GATES · ZERO POSTERIOR STATES
                                             ↓
                         POSTERIOR PREFLIGHT v3C0 → v3C0A:
                         37/48 PATHS PASS · STOP BEFORE CHAINS
                         CALIBRATED SUCCESSOR FROZEN, NOT RERUN
```

Budgets are not automatically additive. Several workbooks allocate, deepen, or stress capacity already carried by a parent force. The original $1 trillion force-capital constraint, the domain-specific $1 trillion fire and flood experiments, the $130 billion flood research program, the selected $2 trillion technology case, and the $320 billion proving-network cross-classification are distinct analytical frames.

Most configurations remain at `R2+`: more detailed than a bounded concept, but still awaiting representative hardware, solved site cases, verified rates, reliability evidence, and independent full-mission trials. Platform renderings remain blocked until physics and evidence close at `R3`.
