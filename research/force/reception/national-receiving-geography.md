# National Receiving Geography

## From national inventory to population continuity under concurrent damage

> **Pass 32 decision:** a receiving force is not national because its inventory is nationally owned. It is national only when surviving capacity is reachable from the people who need it, by a lawful and accessible path, inside the service deadline.

> **Mobility note — Pass 33:** this paper remains authoritative for the population-weighted receiving geography and the aggregate capacity deficit. [The National Civil Mobility and Continuity Force](../mobility/national-civil-mobility-and-continuity-force.md) supersedes its abstract corridor rates with federal network gates, population cohorts, fleet and transfer-node classes, and joint route-receiver trials.

The [National Receiving Lattice](national-receiving-lattice.md) established that land, buildings, utility interfaces, stocks, inspectors, records, activation labor and civil release are operational force capacity. Its synthetic sixteen-region screen exposed a geographic shortfall but could not say whether the failure came from population distribution, concurrent hazard exposure, receiving-site loss or insufficient movement.

This paper replaces that abstraction with a population-weighted national allocation model. It is not a siting study. It does not recommend a city, parcel, port, airport or rail terminal. It creates thirty-two reproducible **Service Catchment Areas** (`SCA`) so that capacity, damage, demand, movement, reception and rights can be tested in the same argument.

The result is more severe than the earlier regional stress test:

- the 7,200 nominal domestic district-equivalents become 3,707.30 after the prior readiness, N-2 and common-mode screen;
- concurrent geographic damage reduces usable scenario capacity to **2,355.80 CDE**, below the **2,500-CDE** domestic campaign demand;
- local capacity serves **1,525.92 CDE**, or **61.0 percent** of demand;
- the declared baseline multimodal corridor plan raises service to **2,066.42 CDE**, or **82.7 percent**;
- **433.58 CDE**—about 433,600 people—remain without complete service;
- even frictionless redistribution has an upper bound of **2,355.80 CDE**, leaving **144.20 CDE** uncovered; and
- among the limited architectures tested, closure first appears with a **1.50× receiving lattice and a 1.732× corridor enterprise**, at a planning-screen burden of about **$2.311 trillion over twenty-five years**.

The critical discovery is therefore not that transportation is useful. It is that the baseline receiving force is simultaneously **capacity-limited and geography-limited**. No amount of routing can move people into capacity that did not survive.

## 1. The force-design correction

Pass 31 treated receiving capacity as a coequal force. Pass 32 adds the missing operational grammar.

> surviving local receiver → accessible population movement → transfer node → destination intake → complete service → return or durable continuity

Every arrow is a possible campaign failure. A nominal bed or district slot at a distant receiver does not serve an affected person. It receives credit only when all of the following are true:

1. the receiving system survives the same event that creates demand;
2. the person can leave the affected area;
3. a road, rail, air or water path can accept the person and any essential equipment;
4. mode changes preserve identification, family, caregiver and clinical continuity;
5. the destination can admit the arriving flow without exceeding its utilities, staff or civil-release capacity;
6. movement is voluntary or rests on explicit lawful authority and review;
7. the person can communicate, obtain care and exercise rights at the destination; and
8. the system has a funded path for return or durable settlement.

This changes the meaning of interregional capacity. **Receiver capacity does not move. People do.** A corridor force is therefore not merely a logistics formation. It is a civil-mobility, public-health, custody, data, accessibility and receiving enterprise.

## 2. What is observed, constructed, assumed and computed

The model separates four epistemic layers.

| Layer | Content | Permitted use | Prohibited inference |
| --- | --- | --- | --- |
| Observed | 2025 county and state population estimates | population denominators and weights | event evacuation counts |
| Observed | 2025 county internal points, area and adjacency | reproducible spatial screening and connected catchments | facility locations or proved corridors |
| Observed | FEMA National Risk Index v1.20 county scores | relative multi-hazard salience with reported coverage | receiver failure probabilities |
| Constructed | thirty-two Service Catchment Areas | national allocation units | jurisdictions, commands, sites or investment decisions |
| Assumed | campaign demand, damage loss, mode rates and intake limits | transparent adverse architecture screen | forecasts or validated performance |
| Computed | deterministic shortest-time greedy dispatch | one auditable feasible-flow witness | optimal, equitable or robust allocation |
| Computed | common-rule cost and workforce scaling | order-of-magnitude architecture comparison | budget estimate or acquisition baseline |

The source discipline matters. FEMA NRI scores combine hazard, exposure, vulnerability and resilience information for relative risk comparison. They are not fragility curves and are never converted into scenario survival. Receiver damage is modeled separately as an explicit stress assumption. Missing or non-applicable hazard scores remain missing rather than becoming zero risk.

## 3. The national planning geography

### 3.1 Construction

The model joins:

- U.S. Census Bureau Vintage 2025 county population estimates for the fifty states and District of Columbia;
- the Census Bureau's 2025 state estimate for Puerto Rico;
- FEMA NRI municipio population shares to distribute that Puerto Rico total for catchment arithmetic;
- 2025 Census Gazetteer county and municipio representative coordinates and land/water area; and
- the 2025 Census county-adjacency file.

The thirty-two catchments comprise twenty-nine connected CONUS graph partitions plus separate Alaska, Hawaii and Puerto Rico cells. Seeds are selected with a deterministic population-weighted farthest-point rule. Counties are then assigned by multi-source traversal of the adjacency graph. The process creates a reproducible screen with more cells where population is dense while preserving continental coverage.

The result represents **344,969,692 people**: the 2025 states-and-DC estimate plus Puerto Rico. Catchment populations range widely because these are geographic screening units rather than equal legislative districts. That variation is intentional and visible.

### 3.2 What the reference place means

Each SCA carries the name of its largest county or municipio as a human-readable reference. “Kings County, NY” or “Harris County, TX” means only that the named county is the largest population component of the planning cluster. It does not identify a preferred receiver, hub or corridor.

The model must not be used to rank parcels or preempt state, local, territorial or Tribal decisions. Its job is to reveal where a national architecture needs more evidence.

### 3.3 Capacity allocation

The 7,200 nominal domestic CDE are allocated in two parts:

\[
C_i = 35 + (7{,}200 - 32 \times 35)\frac{P_i}{\sum P_i}
\]

Every catchment receives a thirty-five-CDE planning floor; remaining capacity follows population. The floor prevents low-population and non-contiguous areas from disappearing inside a purely proportional national average. It is a design hypothesis, not a siting quantity.

The Pass 31 assurance factor is preserved:

\[
A = \frac{5{,}203.2236544}{7{,}200}\times\frac{6}{8}\times0.95 = 0.51490234
\]

Baseline assured capacity in catchment (i) is (C_i A). This preserves the earlier readiness, N-2 cell-loss and common-mode assumptions while changing only the geography.

## 4. The concurrent domestic campaign

The stress set retains the Department's three-catastrophic and five-major concurrency standard. Demand is allocated to catchments by the 2025 population of target states falling inside each SCA.

| Campaign | Class | Target states | Demand CDE | Receiver loss stress | Hazard thread |
| --- | --- | --- | ---: | ---: | --- |
| California cascade | Catastrophic | CA | 500 | 50% | earthquake, wildfire, heat |
| Gulf hurricane | Catastrophic | TX, LA, MS, AL | 500 | 50% | hurricane, coastal and inland flood |
| Northeast compound | Catastrophic | NY, NJ, PA, CT, RI, MA | 500 | 50% | heat, wind and inland flood |
| Cascadia | Major | WA, OR | 200 | 30% | earthquake, tsunami and landslide |
| New Madrid | Major | MO, AR, TN, KY, IL, MS | 200 | 30% | earthquake and inland flood |
| Great Lakes winter | Major | MI, OH, IN, WI, MN | 200 | 30% | winter weather, cold and ice |
| Southeast Atlantic | Major | FL, GA, SC, NC, VA | 200 | 30% | hurricane, coastal and inland flood |
| Southwest heat and drought | Major | AZ, NM, NV, UT, TX, CA | 200 | 30% | heat, drought and wildfire |

Within each catchment, the campaign exposure share is the fraction of its population located in the campaign's target states. Survival factors multiply across overlapping campaigns:

\[
S_i = \max\left(0.25, \prod_k (1 - d_k e_{ik})\right)
\]

where (d_k) is the declared receiver-loss stress and (e_{ik}) is catchment exposure. The twenty-five-percent floor prevents an early planning screen from asserting total receiver annihilation without site-level fragility evidence. It is deliberately conservative in one direction and optimistic in another; both require later testing.

California and Texas illustrate compound exposure. Their catchments can lose capacity in both a catastrophic regional campaign and the major Southwest heat-and-drought campaign. This is the correct conceptual behavior: hazards and campaigns are not independent simply because they appear on different planning lines.

## 5. The local-capacity result

After applying concurrent damage, national scenario capacity is **2,355.80 CDE**. Local matching serves **1,525.92 CDE** and leaves **974.08 CDE** of geographically stranded demand.

This 61.0-percent local closure is not a forecast. It is the first screen that simultaneously includes:

- unequal population distribution;
- overlapping campaign geography;
- receiver damage inside affected catchments;
- nationally distributed spare capacity; and
- a complete-service demand denominator.

The result rejects two tempting simplifications.

First, national assured capacity cannot be compared directly with national demand. The 3,707.30-CDE Pass 31 assurance total exists before event geography. It does not survive intact inside the scenario.

Second, local self-sufficiency cannot be assumed from a population-proportional allocation. High-demand catchments are also where receiver damage is concentrated. Proportional inventory without anti-correlated siting remains correlated with the population it protects.

## 6. The corridor force

### 6.1 Four planning modes

The first corridor screen uses four mode envelopes.

| Mode | Speed | Mobilization | Reception | Arc cap | Origin-mode cap | Availability rule |
| --- | ---: | ---: | ---: | ---: | ---: | --- |
| Road | 55 km/h | 8 h | 6 h | 40 CDE | 80 CDE | connected CONUS SCA path |
| Rail | 70 km/h | 12 h | 8 h | 60 CDE | 120 CDE | connected CONUS SCA path |
| Air | 650 km/h | 6 h | 6 h | 15 CDE | 30 CDE | all SCA pairs |
| Water | 35 km/h | 18 h | 10 h | 25 CDE | 50 CDE | both SCAs pass a planning water-access flag |

Surface path distance is a centroid-to-centroid graph screen across adjacent SCAs. Air uses great-circle distance. Water uses great-circle distance with a 1.25 detour factor. These are not route measurements. The water-access flag is a broad coastal, Great Lakes or major-waterway planning assumption, not evidence of a functioning port.

A route receives credit only if mobilization, travel and reception fit inside seventy-two hours. The path matrix records all 992 ordered SCA pairs and keeps unavailable or late modes visible.

### 6.2 Destination intake

Spare receiver capacity is not the same as arrival throughput. Each destination therefore receives a separate intake ceiling:

\[
I_j = \min\left(\text{spare}_j, \max(20, 0.35\times\text{scenario capacity}_j)\right)
\]

The thirty-five-percent and twenty-CDE values are hypotheses. They stand in for registration, screening, triage, sanitation, shelter assignment, utility connection, records, safeguarding and civil release. Later receiver-class trials must replace them.

### 6.3 Dispatch rule

The baseline flow is a deterministic heuristic:

1. rank origins by remaining local shortfall;
2. rank timely origin-destination-mode options by completion time;
3. allocate continuous CDE until origin demand, destination spare, destination intake, arc capacity or origin-mode capacity binds; and
4. continue until no eligible allocation remains.

The resulting thirty-four-flow plan is a **witness** that the declared capacities can be reconciled. It is not an optimum. It does not yet minimize mortality, family separation, travel burden, cost, inequity or uncertainty.

### 6.4 Baseline result

The baseline corridor enterprise relocates **540.50 CDE** into surviving receiver capacity. Total service rises to **2,066.42 CDE**, or **82.66 percent**. The remaining shortfall is **433.58 CDE**.

Increasing only corridor throughput cannot close the baseline architecture. Even if every unit of spare capacity could be transferred without time, mode, intake or rights friction, total service would stop at **2,355.80 CDE**. The **144.20-CDE** residual is an aggregate capacity deficit.

This is the pass's governing falsification:

> A mobility program can reduce geographic mismatch, but it cannot repair a receiver force whose surviving capacity is smaller than the service promise.

## 7. Architecture choices

Five common-rule screens expose the principal design space.

| Architecture | Lattice scale | Corridor scale | Service | Closure | Shortfall | 25-year planning burden |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| Local-only balanced lattice | 1.000× | 0 | 1,525.92 CDE | 61.0% | 974.08 | $1.138T |
| Balanced lattice + baseline corridors | 1.000× | 1.000× | 2,066.42 CDE | 82.7% | 433.58 | $1.639T |
| Frictionless-transfer upper bound | 1.000× | not purchasable | 2,355.80 CDE | 94.2% | 144.20 | not an architecture |
| Dense local lattice, no relocation | 4.196× | 0 | 2,500.00 CDE | 100.0% | numerical only | $3.092T |
| Closing hybrid | 1.500× | 1.732× | 2,500.00 CDE | 100.0% | numerical only | $2.311T |

The dense-local solution is expensive because it sizes every damaged geography to serve its own coincident peak after receiver loss. It minimizes dependence on interregional movement but multiplies standing site capacity.

The closing hybrid is the least-cost closing candidate in this deliberately small set. It carries a different risk: **631.44 CDE** of service depends on relocation. Its apparent economic advantage exists only if the Department can build and lawfully operate the corridor system assumed by the model.

No claim of optimality is made. A later equity-constrained stochastic model could favor additional local capacity because corridor failure harms particular populations disproportionately, or favor a different spatial mix because site-level hazards are less correlated than state-level exposure implies.

## 8. The institutional consequence

The Department of Resilience requires a fourth force-design machine alongside generation, projection and reception: a **National Civil Mobility and Continuity Command**.

Its mission is not “evacuation.” Evacuation ends when a person leaves danger. Continuity ends when a person safely enters complete service and retains a credible future.

The command requires at least five standing professions:

1. **Accessible movement crews** for road, rail, air and water passenger chains, including mobility devices, caregivers and service animals.
2. **Transfer-node operators** for registration, triage, health, food, sanitation, power, safeguarding, data and onward assignment.
3. **Network recovery engineers** for route clearance, bridge and track inspection, signaling, temporary power and communications.
4. **Dispatch and rights officers** for consent, priority, destination matching, records, family unity, appeals, reunification and return.
5. **Fleet sustainment forces** for operators, maintainers, energy, spares, depots, crew rest and regeneration.

The corridor force must share the receiving lattice's readiness cycle. A bus, train, aircraft or vessel without a destination assignment and intake slot is not employable capacity. A receiver without an accessible incoming path is not assured capacity.

## 9. Rights and legitimacy are capacity

The model does not award quantitative credit for the following requirements because evidence is open. It records them because future models must reduce throughput when they fail.

### Voluntary movement and due process

Movement must be voluntary or rest on explicit lawful emergency authority with review, refusal handling and appeal. A throughput plan that depends on unexamined coercion is not a resilience capability.

### Disability access

Accessibility must be door-to-berth, not vehicle-level. The chain includes origin pickup, boarding, restraints, toilets, communication, mode changes, destination transport and receiver use. A nominal seat unavailable to a person with functional needs is zero capacity for that person.

### Medical continuity

Medicines, oxygen, devices, records, staff and referral arrangements must move with the patient. Transport that creates a clinical interruption transfers risk rather than reducing it.

### Family, caregiver and property custody

Households, caregivers, service animals, mobility devices and essential property require persistent identity and custody. Separation changes willingness to move and the safety of arrival.

### Tribal and territorial sovereignty

Invitation, compact, liaison and sovereign authority govern access and custody. Federal throughput cannot be assumed to override Tribal or territorial decision rights. Puerto Rico is retained as a separate planning cell precisely because a CONUS adjacency model cannot absorb its geography or authority.

### Return or durable settlement

Every outbound flow needs a funded reverse or continuity path. Temporary protection without return, compensation or durable settlement can become indefinite displacement. The force must measure time to an informed return offer, not only time to departure.

## 10. Technology programs pulled by the failure

Military-scale innovation is appropriate here, but the mission thread—not the vehicle silhouette—must pull it.

### 10.1 Autonomous emergency corridor

The objective is not an autonomous truck. It is a mixed human-machine corridor that continuously senses route condition, proves safe passage, reallocates vehicles, maintains disconnected operation and doubles or quadruples usable passenger throughput without increasing fatalities.

### 10.2 Universal accessible lift

A common passenger module, restraint system and data interface should move across road, rail, air and water modes while preserving mobility devices, caregiver position, medical equipment and identity. The kill criterion is any design that gains nominal density by separating people from what makes independent survival possible.

### 10.3 Resilience transfer node

A purpose-built node must operate without intact grid, cloud, water or sewer; register and triage arrivals; sustain sanitation and health; and assign onward movement. The threshold is 10,000 people per day for seven days. The objective is 50,000 per day with thirty-minute dwell.

### 10.4 Damage-tolerant rail bridge

The program combines rapid bridge and track inspection, temporary signaling, modular passenger loading and pre-negotiated railroad access. Its unit of merit is restored 1,000-person train paths per day after network damage.

### 10.5 Austere passenger air bridge

The program joins aircraft, accessible embarkation, ground equipment, airspace, medical custody and destination release. Airport queueing must appear inside the service clock rather than outside the model.

### 10.6 Waterborne civil bridge

The program seeks shallow-draft, high-throughput passenger and utility reception that does not require an intact deepwater port. Weather, berth, health and customs constraints are part of the platform requirement.

### 10.7 National capacity digital twin

The system must report verified receiver state, route state, passenger needs and destination intake under disconnected conditions. Its failure mode is dangerous: stale data can create fictitious capacity. Provenance, local validation and red-team resistance are operational requirements.

These programs remain at `R1/R2`. None supports a platform rendering. Their first useful visual will be a complete service-chain diagram after the requirements close.

## 11. Economic and workforce consequence

The cost screen carries forward the Pass 31 lattice structure:

- $349.84B scalable lattice capital before reserve;
- $120B common lattice capital before reserve;
- 20-percent capital reserve;
- $12.12B/year scalable site operations;
- $24.20B/year common operations; and
- a 15.81 mature-year operations factor across the twenty-five-year build.

Pass 32 adds a baseline corridor hypothesis of $180B pre-reserve capital and $18B/year mature operations. Each corridor multiple adds 40,000 permanent personnel and 200,000 affiliated billets; the baseline lattice retains 59,832 permanent and 163,020 affiliated positions.

Under those common rules:

- baseline lattice plus baseline corridors requires about **$779.8B capital**, **$54.3B/year** mature operations and **$1.639T** over twenty-five years;
- dense local closure requires about **$1.906T capital**, **$75.1B/year** mature operations and **$3.092T** over twenty-five years; and
- the closing hybrid requires about **$1.148T capital**, **$73.6B/year** mature operations and **$2.311T** over twenty-five years.

These are scale comparisons, not cost estimates. The corridor force is especially immature: it lacks asset composition, basing, crew ratios, utilization, fuel or energy demand, maintenance, right-of-way compensation and schedule risk. The values exist to prevent “just move people” from appearing costless.

## 12. What this model still cannot prove

Twenty evidence gates remain open.

The most consequential gaps are:

- catchment boundaries have not been optimized or reviewed with affected governments;
- state-level campaign exposure is not site-level hazard or infrastructure damage;
- route distance is not derived from current road, rail, airport, port or waterway networks;
- mode capacities are not backed by fleet manifests, crew systems or damaged-network exercises;
- destination intake is a planning coefficient rather than a receiver-class throughput test;
- the flow heuristic does not optimize equity, mortality, clinical risk, family separation or uncertainty;
- workforce and cost are parametric screens;
- territorial, Tribal, interstate and international legal regimes are not closed;
- environmental and community burdens are not modeled; and
- no stochastic joint distribution links hazards, utilities, communications, routes, receivers and labor.

The model is `R2+` arithmetic supporting an `R1/R2` architecture. Green checks mean the declared formulas reconcile. They do not mean the system is ready.

## 13. Requirements generated for the force

This pass adds the following controlled requirements to the architecture.

| ID | Requirement | Threshold implication |
| --- | --- | --- |
| `NRG-01` | Allocate receiver force by population and correlated hazard, not equal regions | every capacity claim carries a catchment and damage case |
| `NRG-02` | Preserve a territorial floor | every SCA receives nonzero assured-capacity design attention |
| `NRG-03` | Separate hazard salience from fragility | NRI scores cannot become survival probabilities |
| `NRG-04` | Prove aggregate surviving capacity before optimizing routes | corridor investment cannot close a capacity deficit |
| `NRG-05` | Count interregional service only after destination intake | spare capacity is not arrival throughput |
| `NRG-06` | Treat relocation as a complete civil-service chain | accessible movement, clinical custody, rights and return are mandatory |
| `NRG-07` | Maintain four-mode alternatives | no single transport mode carries national continuity |
| `NRG-08` | Operate under disconnected and falsified-data stress | stale receiver state must fail safe |
| `NRG-09` | Measure distributional closure | national percentage cannot hide stranded populations |
| `NRG-10` | Test dense-local and corridor-heavy rivals | the Department must preserve architecture competition |

## 14. Decision and next research frontier

Advance neither the baseline lattice nor the closing hybrid as a preferred program. Retain three live rivals:

1. **anti-correlated dense reception**—more surviving capacity near high-demand populations without requiring mass movement;
2. **civil mobility at national scale**—purpose-built accessible road, rail, air and water movement with transfer nodes and destination intake; and
3. **mobile substitution**—additional complete service moved into the damaged area where lawful relocation is infeasible or undesirable.

Pass 33 performs that first multimodal and distributional screen in [The National Civil Mobility and Continuity Force](../mobility/national-civil-mobility-and-continuity-force.md). It finds that a universal-access force can average 97.8-percent closure while passing the joint distributional rule in only 13.8 percent of trials. The next frontier is parameter uncertainty, tract-scale collection, door-to-berth exercises and reference configuration of the transfer node and common passenger module.

Only then should the program select receiver classes for site-level engineering or mobility systems for platform configuration. Rendering remains prohibited.

## Sources

- U.S. Census Bureau, [Vintage 2025 state population estimates](https://www.census.gov/data/datasets/time-series/demo/popest/2020s-state-total.html) and [county datasets](https://www2.census.gov/programs-surveys/popest/datasets/2020-2025/counties/totals/).
- U.S. Census Bureau, [2025 Gazetteer files](https://www2.census.gov/geo/docs/maps-data/data/gazetteer/2025_Gazetteer/) and [2025 county adjacency](https://www2.census.gov/geo/docs/reference/county_adjacency/).
- Federal Emergency Management Agency, [National Risk Index v1.20 county table](https://www.fema.gov/about/reports-and-data/openfema/nri/v120/NRI_Table_Counties.zip).
- Bureau of Transportation Statistics, [National Transportation Atlas Database](https://www.bts.gov/ntad) and [Transportation Geography of the United States 2025](https://www.bts.gov/geography/geospatial-2/transportation-geography-united-states-2025).
- U.S. Department of Transportation, [2026 National Freight Strategic Plan](https://www.transportation.gov/freight/NFSP).
- Federal Highway Administration, [No-notice evacuation planning primer](https://ops-dr.fhwa.dot.gov/publications/evac_primer_nn/chap5.htm).
- U.S. Government Accountability Office, [Transportation-Disadvantaged Populations: Actions Needed to Clarify Responsibilities and Increase Preparedness for Evacuations](https://www.gao.gov/products/gao-07-44).

The executable argument is the [National Receiving Geography model](../../../models/national-receiving-geography-model.xlsx).
