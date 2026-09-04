# WRG-50 configuration model

## Purpose

Pass 7 converts the Water Restoration Group 50 (`WRG-50`) from a bounded architecture into an editable configuration model. The model links delivered service, source treatment, pipe hydraulics, pressure zones, pipe mass, storage, point-of-use access, wastewater, residuals, installation tempo, deployment lift, workforce, failure cases, and the rendering gate.

The model is an engineering-research instrument, not a construction design. It distinguishes externally anchored values, formula-derived values, design choices, and assumptions requiring tests. A value does not become evidence because the spreadsheet can calculate it.

The editable workbook is [`models/water-restoration-engineering.xlsx`](../models/water-restoration-engineering.xlsx).

## Reference configuration

The default case represents a difficult but legible coastal campaign:

| Control | Reference value | Status |
|---|---:|---|
| Product water | 50,000 m³/day | force-design target |
| Supported population | 1,000,000 | mission reference |
| Selected service | 50 L/person/day | expanded emergency service |
| Source case | seawater | selected treatment case |
| Route | 50 km; 50 m net rise | design assumption |
| Trunks | two parallel lines | degraded-service design choice |
| Internal diameter | 0.5 m | design assumption |
| Darcy friction factor | 0.015 | reference inside 0.012–0.020 study band |
| Pump efficiency | 75% | engineering assumption |
| Minor loss | 10% of friction head | engineering assumption |
| Pipe geometry | illustrative PE4710 DR17 | industry-bounded assumption |
| Maximum operating pressure | 100 psi | selected ceiling below 125-psi reference class |
| Product buffer | 12 hours | design assumption |
| Community return flow | 75% of delivered volume | midpoint assumption in the 60–90% planning band |
| Construction mode | surface rapid; five work fronts | untested design assumption |
| Force-generation depth | three operational echelons | force-design assumption |

PPI identifies PE4710 DR17 water pipe as a 125-psi reference pressure class at standard temperature and requires sustained pressure, recurring/occasional surge, temperature and application conditions to be evaluated together.[^ppi-tn27][^ppi-handbook] The model therefore uses 100 psi as a selected operating ceiling, not as a universal allowable pressure.

## Model structure

The workbook has thirteen sheets:

1. **Summary** — decision outputs, findings, power and mass comparisons;
2. **Controls** — editable mission, hydraulic, storage, force and scenario inputs;
3. **Service Demand** — water levels, population demand and WRG-50 coverage;
4. **Treatment Cases** — fresh surface, brackish and seawater feed, reject, energy and train effects;
5. **Hydraulic Reaches** — Darcy–Weisbach balance and uniform pressure-zone reference;
6. **Pipe & Lift** — pipe geometry, mass and preliminary equipment manifest;
7. **Storage & Access** — raw/product/break/district storage and distribution channels;
8. **Return Flows** — community wastewater, treatment reject and cleaning residuals;
9. **Deployment Plan** — construction modes, primary lift and layered arrival;
10. **Workforce** — continuous positions, shifts, relief, day staff and force generation;
11. **Failure Modes** — degraded capacity and safe operating responses;
12. **R3 Gate** — technical closure evidence and model-integrity checks; and
13. **Sources** — primary references and an assumption-validation register.

Yellow cells are inputs. Calculated cells remain formula-driven. Source URLs and assumption status are visible inside the workbook.

## Hydraulic closure

Total flow is:

\[
Q_{total}=\frac{50{,}000}{86{,}400}=0.579\ \text{m}^3/\text{s}.
\]

With two equal trunks:

\[
Q_{line}=0.289\ \text{m}^3/\text{s}
\]

and velocity in each 0.5-meter-ID line is:

\[
v=\frac{Q_{line}}{\pi D^2/4}=1.474\ \text{m/s}.
\]

For 50 kilometers and `f = 0.015`, Darcy–Weisbach friction head is 166.0 meters. The model adds 16.6 meters of minor losses and 50 meters of static rise, producing 232.6 meters of total dynamic head.

Average hydraulic power for both lines is:

\[
P=\frac{\rho gQH}{\eta}=1.761\ \text{MW}.
\]

With a 30-percent installed-power reserve, the hydraulic plant is 2.289 MW.

The model divides the uniform reference route into four pressure zones. Each zone represents 12.5 km, 58.16 meters of head, 82.72 psi operating pressure, and approximately 0.57 MW of installed pumping power. This closes a steady-state arithmetic reference only. It does not close:

- actual high and low points;
- zero-flow static pressure;
- pump start, stop and trip transients;
- rapid valve closure;
- air admission and release;
- vacuum and column separation;
- temperature derating;
- recurring and occasional surge;
- fittings, anchor blocks, crossings and local structures; or
- failure propagation between reaches.

EPA describes pressure monitoring and management as integral to distribution-system operation because pressure affects quality, intrusion, water loss and break risk.[^epa-distribution] A surveyed route and transient model remain an R3 prerequisite.

## Pipe and lift mass

For an internal diameter of 0.5 meters and DR17 geometry, the model derives:

| Geometry result | Value |
|---|---:|
| Outer diameter | 0.567 m |
| Wall thickness | 0.033 m |
| Material area | 0.056 m² |
| Linear mass | 53.1 kg/m, numerically 53.1 t/km |
| Two-line base pipe mass | 5,305.8 t |
| Ten-percent route and damage reserve | 530.6 t |
| Total pipe mass | 5,836.4 t |

The preliminary full manifest produces 20,449 tonnes before contingency and 23,516 tonnes with a 15-percent configuration allowance. Stored water, excavated or fill material, local construction aggregate, fuel, recurring consumables after the initial stock, and personnel effects are excluded.

The principal manifest masses are:

| Category | Base mass |
|---|---:|
| Conveyance | 6,961 t |
| Mobility fleet | 3,960 t |
| Treatment | 2,580 t |
| Construction machinery | 1,920 t |
| Sanitation | 1,620 t |
| Support modules | 1,440 t |
| Quality, storage, distribution, power, spares and initial consumables | 1,968 t |
| Configuration contingency | 3,067 t |

Only the pipe mass is geometry-derived. Equipment quantities, unit masses and volumes remain explicit preliminary assumptions. Their purpose is to reveal lift and reception questions, not manufacture an appearance of design maturity.

After contingency, the manifest assigns approximately 11,040 tonnes to sealift, 9,161 tonnes to rail, 3,085 tonnes to road and 230 tonnes to air as primary modes. These assignments do not represent an origin–destination network or claim that the group can arrive in 2.3 days. They show that airlift is an edge capability while port, railhead, road, handling and receiving-site throughput dominate the main deployment.

## Treatment and power

The model carries three treatment cases:

| Case | Recovery | Process energy | Feed for 50,000 m³/day | Reject | Plant power including assumed auxiliaries |
|---|---:|---:|---:|---:|---:|
| Fresh surface | 90% | 0.6 kWh/m³ | 55,556 m³/day | 5,556 m³/day | 1.50 MW |
| Brackish | 75% | 1.5 kWh/m³ | 66,667 m³/day | 16,667 m³/day | 3.69 MW |
| Seawater | 50% | 4.0 kWh/m³ | 100,000 m³/day | 50,000 m³/day | 9.58 MW |

The seawater process-energy and recovery reference is grounded in the DOE desalination bandwidth study.[^doe-desal] Fresh-surface and brackish energy, auxiliary fractions, source recovery, train mass and consumable rates are model assumptions requiring feed-matrix tests and vendor guarantees.

Under the default seawater case:

- average treatment plus hydraulic power is 11.34 MW;
- the 30-percent reserve adds 3.40 MW;
- reference installed capacity is therefore approximately **14.75 MW**; and
- treatment energy is materially larger than trunk pumping energy.

This does not diminish the distribution problem. The plant is about one-third of the preliminary manifest mass, while the pipe, mobility, construction, storage interfaces and sanitation system carry the rest.

## Storage, access and quality

The default storage system holds 47,917 m³ and therefore 47,917 tonnes of water:

| Storage function | Volume |
|---|---:|
| Four-hour raw-water buffer | 16,667 m³ |
| Two-hour plant clearwell | 4,167 m³ |
| Three one-hour inter-zone break stores | 6,250 m³ |
| Six-hour district reserve | 12,500 m³ |
| Four-hour isolated contingency reserve | 8,333 m³ |

At 2.5 meters usable depth and a gross-to-net site factor of 2.0, the simplified storage footprint is 38,333 m², or 3.83 hectares. This is a land and sanitary-protection requirement in addition to a transport requirement.

The point-of-use architecture allocates the default output across:

- safe utility sectors: 50 percent;
- direct critical facilities: 10 percent;
- district loops and service islands: 25 percent;
- tanker delivery: 10 percent; and
- packaged-water interfaces: 5 percent.

With provisional node capacities, the model produces 111 distribution interfaces and 154 sampling actions per day. Those counts are staffing and laboratory demand signals. They are not regulatory sampling schedules. EPA emergency guidance requires planners to consider partially usable and completely unusable networks, multiple distribution methods, operators, power, storage and security.[^epa-edws]

## Return flows and sanitation

At the 75-percent community return-flow assumption, the default mission creates 37,500 m³/day of wastewater. If surviving local systems accept 40 percent, the temporary treatment gap is 22,500 m³/day. The model provisionally represents this as nine 2,500-m³/day wastewater trains; both capacity and unit mass remain open assumptions.

The selected seawater case simultaneously produces:

- 50,000 m³/day of concentrate; and
- 1,000 m³/day of backwash and clean-in-place residuals.

The total managed liquid flow is therefore 88,500 m³/day before any double-counting corrections or source-specific reuse. The significant result is architectural: the potable plant can be smaller than the combined system required to receive, convey, store, distribute, recollect and safely discharge its flows.

## Construction tempo

Three installation cases make the trade visible:

| Mode | Rate | Work fronts | Commissioning | Total to reference service |
|---|---:|---:|---:|---:|
| Surface rapid | 0.60 route-km/front-day | 5 | 3 days | 19.7 days |
| Shallow protected | 0.30 route-km/front-day | 6 | 5 days | 32.8 days |
| Enduring | 0.12 route-km/front-day | 8 | 10 days | 62.1 days |

Every rate is an assumption. The values exist so the research program can define the required trials: flat road shoulder, dense urban corridor, rubble, flooded ground, steep grade, river crossing, freezing conditions, extreme heat and wildfire exposure. Until repeated tests establish joint rate, rework, crossing delay, inspection, cleaning, disinfection and recovery time, 19.7 days is a test target rather than a promise.

## Workforce and force generation

The position model produces 2,720 deployed people:

| Workforce block | Deployed people |
|---|---:|
| Command and civil integration | 120 |
| Source, network and route assessment | 200 |
| Treatment and quality | 425 |
| Conveyance construction and operations | 750 |
| Storage and distribution | 475 |
| Sanitation and residuals | 375 |
| Maintenance, logistics and internal support | 375 |

Three operational echelons require 8,160 people. A provisional 25-percent training, depot and institutional overhead raises the service establishment to 10,200 billets. At an eight-percent annual replacement assumption, the pipeline requires 816 accessions annually.

This is more than a construction crew. The formation contains continuing utility operation, quality release, public-health, wastewater, maintenance, distribution, civil authority and transfer functions. The workbook exposes the position and shift arithmetic, but it does not yet establish occupational specialties, qualification duration, school capacity, reserve mix or fatigue limits.

## Failure cases

The model includes ten degraded cases. Capacity is limited by the weakest treatment, trunk, source, power, distribution or wastewater factor. Important consequences include:

- losing one trunk reduces output to 25,000 m³/day—enough arithmetically for 1.67 million people at 15 L/day but only 500,000 at 50 L/day;
- losing both grid and prime power leaves a provisional 12,500 m³/day black-start service;
- a source outside the validated treatment envelope stops release rather than producing an unsafe plausible output;
- loss of local wastewater acceptance restricts potable output to the sanitation pathway; and
- telemetry loss moves the system to local manual control and reduced pressure.

The capacity factors and recovery times are hypotheses. Their value is to define fault-injection and operational tests, not to predict reliability.

## Gate decision

All twelve spreadsheet integrity and design-consistency checks pass in the reference case. The workbook was re-imported after export, scanned for formula errors, rendered on all thirteen sheets, and tested under alternate treatment and construction selectors. Independent calculations reproduce its velocity, hydraulic power and pipe mass.

Those checks prove that the model behaves as designed. They do **not** prove the system is ready to build.

The R3 gate contains twelve evidence domains. None is marked verified. Mass, energy, flow and storage close only at model level; treatment, waste, crew and lift are bounded; pressure/surge and maintenance remain open; construction tempo and degraded modes require tests. The visualization state therefore remains **R2+**.

No rendering is authorized. The next water-specific work should be a route/transient prototype study, source-feed guarantee matrix, configuration-controlled vendor manifest, multi-front construction trial plan, reliability/maintenance model, and full-scale degraded-mode test program.

## Industrial implication

The model makes the “Lockheed Martin scale” proposition concrete. A serious water force would create industrial programs for:

- high-rate potable pressure pipe, valves, fittings, fusion and repair systems;
- standardized modular intakes and source-specific treatment trains;
- mobile laboratories and national quality-control systems;
- pumps, drives, switchgear, break tanks, surge control and black-start power;
- purpose-built autonomous route, pipe-handling, trenching, inspection and repair machinery;
- deployable reservoirs and district water interfaces;
- modular wastewater and residual-management systems;
- rail, sealift and receiving-site packages;
- professional schools, proving grounds, depots and reserve production lines; and
- exportable standards for complete deployable utilities.

The procurement object is the assured restoration of a water service under damaged-network conditions. Individual vehicles and platforms follow from that operating system.

[^ppi-tn27]: Plastics Pipe Institute, [*Frequently Asked Questions: HDPE Pipe for Water Distribution and Transmission Applications*](https://www.plasticpipe.org/common/Uploaded%20files/Technical/TN-27.pdf), TN-27, 2009.
[^ppi-handbook]: Plastics Pipe Institute, [*Handbook of PE Pipe*](https://www.plasticpipe.org/common/Uploaded%20files/Technical/PPI%20PEHandbook2022.pdf), 2022 edition, Chapter 6.
[^epa-distribution]: U.S. Environmental Protection Agency, [*Drinking Water Distribution System Tools and Resources*](https://www.epa.gov/dwreginfo/drinking-water-distribution-system-tools-and-resources), accessed September 4, 2026.
[^doe-desal]: U.S. Department of Energy, [*Bandwidth Study on Energy Use and Potential Energy Savings Opportunities in U.S. Seawater Desalination Systems*](https://www.energy.gov/sites/default/files/2017/12/f46/Seawater_desalination_bandwidth_study_2017.pdf), 2017.
[^epa-edws]: U.S. Environmental Protection Agency, [*Planning for an Emergency Drinking Water Supply*](https://www.epa.gov/sites/default/files/2015-03/documents/planning_for_an_emergency_drinking_water_supply.pdf), EPA 600-R-11-054, June 2011.
