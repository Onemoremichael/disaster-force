# The service survives only if the system has state

## Degraded-service architecture for the Department of Resilience first-reach water force

Pass 64 defined a complete first-reach water mission: establish ten kilometres of temporary trunk conveyance and deliver 10,000 cubic metres of certified water per day to accessible public and institutional interfaces. It also stated that rupture of the single installed trunk would reduce service to zero. That statement was correct about **bulk inflow through the trunk** and incomplete about **public service at the receiver**. A clean, charged and connected downstream store can preserve service while the trunk is isolated and repaired. An empty, contaminated, disconnected or upstream store cannot.

**Successor correction.** Pass 66's [federated receiver architecture](wrg-fr10-federated-receiver-architecture.md) resolves the receiver-wide hold as a boundary problem rather than a site-count problem. Three independently branched, powered, controlled and quality-released half-demand islands pass eight of ten declared receiver worlds; a four-island design with a half-demand alternate source provenance passes nine. Both remain unadmitted, and all architectures correctly stop under a national unknown-contaminant no-issue order. That successor replaces this paper's generic call for “alternate receiver switching or isolated public-service islands” with a controlled federation and evidence contract.

That correction changes the object of acquisition. The force is not buying a pipe with a tank attached. It is buying a stateful service system whose readiness depends on route topology, storage location, measured inventory, quality release, distribution continuity, repair time, treatment headroom and receiver authority. Hardware quantity alone cannot establish any of those conditions.

Pass 65 competes four degraded-service architectures inside the same first-reach mission:

1. `A1`: one full-flow trunk with one centralized twelve-hour gross buffer;
2. `A2`: two half-flow trunks in one corridor with the same storage split into two sectors;
3. `A3`: one full-flow trunk, a staged half-flow bypass kit and two storage sectors; and
4. `A4`: two half-flow trunks on separated routes with a distributed twenty-four-hour gross buffer divided into four sectors.

The companion [degraded-service architecture model](../../../models/force/projection/wrg-fr10-degraded-service-architecture.xlsx) carries the hydraulic screen, storage initialization, architecture mass, seven failure worlds, program consequences and evidence contract. Under the declared assumptions, `A1` passes one of seven worlds, `A2` four, `A3` four and `A4` six. These are **declared design screens**, not observed performance. Every architecture remains unadmitted, every scenario result is untested, and rendering remains blocked.

The deeper result is institutional. First water and resilient-service readiness are different milestones. Two lines in one trench are not two independent routes. Storage is a readiness state, not a nameplate quantity. A receiver-wide contamination hold defeats every topology in this pass. The water force therefore extends beyond mobile production and conveyance into a federation of prepared receivers, isolated public-service islands, continuous inventory assurance and independent quality authority.

## Executive judgment

Six judgments should govern the next water-force design cycle.

First, **bulk flow, stored inventory and accessible service are different state variables**. A broken trunk can carry zero flow while the public continues to receive water from a downstream buffer. Conversely, a functioning treatment plant can produce water while the public receives none because pressure, quality release, distribution or access has failed. Readiness reporting must publish these states separately.

Second, **installed storage receives no continuity credit until it is sanitary, charged, measured, connected and releasable**. The first-reach baseline has 5,000 cubic metres of gross storage and 4,250 cubic metres of declared usable inventory. At a fifty-percent service floor, that usable inventory covers 20.4 hours. At full demand, it covers only 10.2 hours. The same hardware at first water may contain no reserve at all.

Third, **the current treatment train cannot charge the buffer while meeting full demand**. Its declared capacity and the service requirement are both 10,000 cubic metres per day. Surplus is therefore zero. Filling the gross 5,000-cubic-metre store requires twelve hours if public service is withheld. A twenty-five-percent treatment headroom would allow concurrent filling in forty-eight hours. The expanded 10,000-cubic-metre store requires twenty-four hours with service withheld or ninety-six hours at the same headroom. Treatment reserve is thus partly a readiness-time technology.

Fourth, **parallel hardware is not independent capacity unless its correlated losses are controlled**. Dividing the reference flow between two pipes preserves total flow area and normal velocity. It also creates a common-corridor failure when both lines share access, power, control and damage geography. `A2` survives one-line rupture and uncharged rupture but fails severance of its common corridor. `A4` pays for geographic separation and retains fifty-percent inflow when one route is lost.

Fifth, **a timed bypass can compete with full duplication**. `A3` uses stored inventory to bridge a declared six-hour bypass deployment, then restores half flow around an isolated block. It passes the full-buffer rupture, partial-buffer rupture, common-corridor severance and compound storage-sector worlds on paper. It fails an immediate rupture at first water because the buffer is empty. The decisive technologies are not merely flexible pipe; they are rapid sanitary connections, prepared isolation blocks, route access, robotic placement and a certified transition from stored service to bypass service.

Sixth, **the leading local architecture still fails at the receiver boundary**. `A4` passes six declared worlds but cannot deliver safe water during a receiver-wide contamination hold. More pipe and more tanks cannot solve a shared quality authority, contaminated distribution system or closed public interface. The next proof object must include alternate receiver switching or isolated public-service islands. `A4` is the test leader, not a selected architecture.

## 1. Research question and correction

The question is not whether redundancy is desirable. It is:

> What minimum combination of conveyance paths, stored inventory, treatment reserve, isolation and prepared receiver capacity can maintain at least fifty percent of accessible first-reach water service through a registered failure for twenty-four hours?

The phrase **accessible service** is deliberate. The [first-reach competition](wrg-fr10-first-reach-water-system-and-technology-competition.md) already established a complete chain from source through residual custody. The present pass does not reduce that chain to hydraulic delivery. It isolates one missing layer: how the chain changes state when production or conveyance is interrupted.

Pass 64’s zero-service statement came from a common analytical shortcut. If one pipe carries all normal flow, a full-bore rupture produces zero downstream pipe flow. The shortcut then equates that flow state with public service. That equivalence holds only if there is no downstream usable inventory, no alternate path and no distributed source. Once storage exists, three clocks matter:

- the time until the buffer becomes usable;
- the time the buffer can support the required service floor; and
- the time until inflow is restored through repair, bypass or another route.

The architecture passes a bounded loss only if the service clock outlasts the restoration clock. It fails even with abundant gross storage if the store has not been charged, the clean sector is isolated from users, the public distribution system has lost power, or the quality authority has placed the receiver on hold.

This is not a semantic refinement. It determines what the force must own, what the receiver must prepare, what the command must observe and when a formation may be declared ready.

## 2. A stateful service model

Let normal product-water demand be `Q`, the required degraded-service share be `s*`, immediately surviving line share be `s_l`, usable storage be `V_u`, initial charged share be `c`, surviving clean-sector share be `q_s`, and the bridge interval be `h_b` hours. The buffer available to the scenario is:

```text
V_available = V_u × c × q_s
```

The volume required to cover the gap between surviving inflow and the service floor is:

```text
V_required = max(s* - s_l, 0) × Q × h_b / 24
```

The declared screen passes when the receiver remains available and either surviving line flow already meets the floor or available clean inventory covers the gap until repair or bypass. For the compound sector-contamination world, the surviving clean-sector share itself defines the accessible service share during source loss.

The model uses `Q = 10,000 m³/day`, `s* = 0.50` and a twenty-four-hour evaluation horizon. It does not assign probabilities. The worlds are a requirements set: each exposes a different dependency, and a design receives no credit for being likely to pass a world it was not required or observed to survive.

This simplified screen is intentionally conservative in two ways. It does not award a partial pass when inadequate storage sustains the floor for only part of the bridge. It also does not assume water can be rationed perfectly across a damaged receiver. A representative trial must measure pressure, queueing, accessibility, quality and distribution, not merely tank drawdown.

The screen is incomplete in other ways. It does not yet solve transient pressure, valve timing, fire-flow competition, leakage, reserve water quality over time, pump failure, generator black start, branch-network hydraulics or household access. Those omissions remain explicit evidence gates.

## 3. Storage is an initialized capability

The force requires a storage state machine rather than a line item called “tankage.” Five states matter.

| State | What is true | Continuity credit |
|---|---|---|
| hardware delivered | structure, liner, valves and pumps have reached the receiver | none |
| sanitary store commissioned | cleaning, disinfection, structure and quality release are complete | water may enter; duration remains zero |
| partially charged | measured usable inventory is below target | only measured duration |
| resilient-service ready | target usable inventory, isolation, power and clean distribution are live | registered coverage may be claimed |
| contaminated or isolated | one or more sectors are unavailable | only surviving clean, connected inventory |

This state machine creates two operational milestones.

**First water** is the time when independently released water reaches an accessible interface. **Resilient-service ready** is the later time when the registered downstream reserve and isolation state can support the failure contract. A commander may rationally begin public service before the reserve is full, but the formation may not claim the corresponding continuity until charging is complete.

The baseline exposes a cold-start dilemma. A treatment train producing exactly normal demand has no concurrent charging surplus. The receiver can:

- withhold service for twelve hours to fill the 5,000-cubic-metre gross store;
- begin full service immediately and never fill it;
- ration service below production so the difference charges storage;
- arrive at a precharged receiver;
- add treatment headroom; or
- combine these policies over time.

None is free. Withholding delays public effect. Rationing reduces early service. Precharge transfers readiness burden to the receiver and requires turnover and quality control. Treatment headroom adds mobile or fixed capital, energy, intake and residual capacity. The acquisition system must compete these policies, not hide one in the schedule.

Under the declared construction assumptions, the architectures reach first water at 152 to 184 hours, already beyond Pass 64’s 120-hour target for the sectional reference. If service is withheld while the base buffer fills, resilient readiness moves to 164–196 hours. With twenty-five-percent treatment headroom and simultaneous full service, it moves to 200–232 hours. `A4` reaches first water in 184 hours, the expanded buffer with service withheld in 208 hours, and the expanded buffer with twenty-five-percent headroom in 280 hours.

The longer headroom case is not paradoxical. A small surplus preserves full service but fills slowly. The time metric must say whether it prioritizes first public water, full normal service, or a charged resilience reserve.

## 4. The four architectures

### `A1`: one trunk and centralized storage

`A1` retains the Pass 64 reference: one 0.5-metre internal-diameter trunk, one corridor, twelve hours of gross storage, and one storage sector. It is the least complex and least expensive topology. Its declared complete dry mass is about 3,994 tonnes and its chargeable burden about 4,142 tonnes.

Its protection mechanism is time. With a full clean buffer, 4,250 cubic metres of usable inventory exceed the 3,750 cubic metres required to maintain half service for an eighteen-hour rupture repair. It therefore passes the full-charge rupture world. It fails the same rupture at first water because the buffer is empty. It fails a delayed repair at half charge, a twenty-four-hour corridor loss and a twenty-four-hour treatment loss because available inventory is inadequate. A compound loss of treatment and the sole storage sector removes all protected service.

`A1` is valuable as a control architecture. It proves that storage can correct the earlier zero-service inference while showing that an aggregate tank quantity is brittle. One failure or quality hold can erase the entire reserve.

### `A2`: two half-flow lines in one corridor

`A2` divides normal flow across two 0.3536-metre internal-diameter lines. Each carries 5,000 cubic metres per day. The store remains 5,000 cubic metres gross but is split into two isolated sectors. The declared dry mass is about 4,053 tonnes and chargeable burden about 4,189 tonnes.

The design preserves half service immediately after one-line rupture, including at first water when storage is empty. It also passes the partial-charge delayed-repair world because line flow alone meets the floor. During compound treatment loss and one-sector contamination, the surviving sector provides exactly fifty percent of the registered storage service. These four passes expose the value of both line and storage partitioning.

The weakness is geography. Both lines share one corridor. A washout, debris impact, ground displacement, access denial, fire front or control failure can remove both. The same fully charged buffer that bridged eighteen hours cannot bridge the twenty-four-hour common-corridor evaluation: 4,250 usable cubic metres are short of the 5,000 required. Parallel line count therefore cannot stand in for route independence.

### `A3`: one trunk with a staged bypass

`A3` keeps the full-flow trunk and adds a 1.2-kilometre staged half-flow bypass kit, prepared isolation blocks and two storage sectors. Its declared dry mass is about 4,079 tonnes and chargeable burden about 4,228 tonnes. The bypass is required to reach certified half flow within six hours.

The system’s resilience mechanism is sequential. Immediately after trunk rupture, line flow is zero. Stored inventory covers half service during bypass placement. Once connected and released, the bypass supplies half flow while the main line is repaired. At 10,000 cubic metres per day, six hours of half service requires 1,250 cubic metres. The full buffer provides 4,250; a half-charged buffer provides 2,125. Both bridge the declared bypass time.

The architecture consequently passes full-charge rupture, half-charge delayed repair, common-corridor severance that can be routed around a local isolated block, and compound treatment loss with one of two storage sectors unavailable. It fails rupture at first water because zero charged inventory cannot bridge the six-hour gap. It also fails a full treatment outage over the twenty-four-hour horizon because the base buffer is too small. A receiver-wide hold defeats it.

The stated common-corridor pass is a demanding technology hypothesis. It assumes survey, access and prepared connections allow the bypass to route around the damaged block. A geographically broad corridor event could defeat both main access and bypass handling. Representative trials must vary damage length, debris, contamination, elevation, road crossing and available work area.

### `A4`: separated twin lines and distributed storage

`A4` combines two half-flow trunks on separated routes with twenty-four hours of gross storage divided among four sectors. A ten-percent route factor raises installed line length from twenty to twenty-two route-kilometres. The declared dry mass is about 4,324 tonnes and chargeable burden about 4,496 tonnes.

The architecture preserves fifty-percent inflow after one-line or one-corridor loss. Because flow survives, an empty buffer at first water does not defeat the service floor. Four storage sectors preserve seventy-five percent of storage service after one sector is contaminated during treatment loss. The 8,500 cubic metres of usable inventory also cover the 5,000 cubic metres required for a twenty-four-hour half-service treatment outage.

It passes six declared worlds and fails the seventh: receiver-wide contamination hold. That result locates the remaining common mode outside the local line-and-storage topology. If the distribution network, receiver quality release or all public interfaces are unavailable, a second trunk ending at the same receiver does not create service.

`A4` is therefore the test leader. It is not selected. Route separation is presently a label, not a demonstrated absence of common cause. The two paths could still share treatment, intake, power, control, crossings, maintenance, security, labor, telemetry or public distribution. These dependencies must become a controlled route-separation contract.

## 5. Hydraulic and material consequences

The twin-line designs use a diameter chosen to preserve the reference total flow area:

```text
D_half = D_single / √2 = 0.3536 m
```

Two such lines have the same combined internal area as one 0.5-metre line. When each receives half the flow, mean velocity remains about 0.589 metres per second. At fixed dimension ratio and material density, total wall material is also approximately preserved for equal aggregate route length because material section scales with diameter squared.

Hydraulic friction does not remain equal. Darcy friction head is proportional to `L × v² / D`. With velocity preserved and diameter smaller, each half-flow line has about `√2` times the friction head of the full-diameter line over the same route. In the declared ten-kilometre screen, `A1` and `A3` have about 5.31 metres of friction head and 38.3 kilowatts of shaft power after the representative twenty-metre static head is included. `A2` has about 7.51 metres of friction head and 41.7 kilowatts total. The eleven-kilometre separated route in `A4` raises friction head to about 8.27 metres and total shaft power to 42.8 kilowatts.

These power differences are modest relative to water treatment and residual handling, but they show that redundancy topology cannot be treated as mass-neutral and energy-neutral simultaneously. The pressure and transient design also becomes more complex. Parallel lines require isolation, balancing, cross-connections, air management and controls that preserve one route while another fails. A bypass introduces rapid connection and surge. Distributed storage introduces multiple pressure zones and sanitation boundaries.

The four complete systems occupy a narrow but meaningful planning range. `A1` carries about 583.6 tonnes of pipe material including repair reserve. `A2` carries the same material mass before fittings because the total route length and total wall area are preserved. `A3` rises to about 615.5 tonnes because of the bypass kit. `A4` rises to about 642.0 tonnes because its separated routes are ten percent longer. Fittings and fixed handling also increase with line count, sector count and isolation demand.

These are configuration screens, not bills of material. Valve bodies, anchors, branches, couplings, instrumentation, electrical systems, trench protection, road plates, disinfection equipment and sector manifolds remain first-order factors. The next object-level release must replace the percentage fittings allowances with serialized components and tested interfaces.

## 6. The seven registered failure worlds

The failure set is designed to separate topology, initialization, duration, quality and receiver state.

| World | Initial condition and loss | Dependency exposed |
|---|---|---|
| `W1` | one-line rupture after full charge; eighteen-hour repair | storage bridge or surviving line |
| `W2` | one-line rupture at first water; buffer empty | cold-start independence |
| `W3` | one-line rupture at half charge; thirty-six-hour repair | partial inventory and bounded bypass |
| `W4` | common-corridor severance; buffer full | geographic correlation |
| `W5` | one storage sector contaminated during treatment loss | sector isolation and clean inventory |
| `W6` | treatment train unavailable; buffer full | source-independent stored service |
| `W7` | receiver-wide contamination hold | alternate receiver or service island |

No probability is attached. `W5` is explicitly compound because a storage-sector loss by itself would not interrupt service while full treatment and line inflow remained available. Combining it with treatment loss forces the architecture to demonstrate that sectorization preserves a meaningful clean reserve.

The declared result is:

| Architecture | `W1` | `W2` | `W3` | `W4` | `W5` | `W6` | `W7` | score |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| `A1` centralized single trunk | pass | fail | fail | fail | fail | fail | fail | 1/7 |
| `A2` same-corridor twins | pass | pass | pass | fail | pass | fail | fail | 4/7 |
| `A3` staged bypass | pass | fail | pass | pass | pass | fail | fail | 4/7 |
| `A4` separated twins and distributed storage | pass | pass | pass | pass | pass | pass | fail | 6/7 |

The tie between `A2` and `A3` is informative. They achieve four passes through different mechanisms. `A2` buys immediate half-flow resilience against a line rupture but retains corridor correlation. `A3` accepts an initial flow gap and uses inventory plus rapid reconfiguration to cross it. They should not be collapsed into one middle alternative. A representative competition may find that route access, pressure transients, storage reliability or transport burden strongly separates them.

The failure matrix also reveals that a count is not a utility function. Passing six worlds does not make `A4` six-sevenths ready. The only world it fails is a common receiver state that can erase all public effect. A catastrophic common mode cannot be averaged away by success in easier worlds.

## 7. Program and mobility consequence

Pass 64 declared a $110.4 billion twenty-five-year first-reach technology program. It included twenty-four initial operational sets and twelve prepared development receivers at baseline allowances of $1.2 billion per set and $0.6 billion per receiver. Pass 65 holds the common research, proving, production and support program constant, removes those baseline fielding allowances, and inserts architecture-specific comparators.

| Architecture | equipment per set | receiver per node | revised program | change from base |
|---|---:|---:|---:|---:|
| `A1` | $1.20B | $0.60B | $110.4B | $0.0B |
| `A2` | $1.35B | $0.75B | $115.8B | $5.4B |
| `A3` | $1.40B | $0.80B | $117.6B | $7.2B |
| `A4` | $1.65B | $1.10B | $127.2B | $16.8B |

The values are declared planning cases, not estimates. They make one principle visible: resilience mechanisms consume both mobile and prepared capital. `A4` does not merely buy more pipe. It needs separate routes, easements, crossings, power and control independence, four sanitary sectors, distribution isolation and a larger prepared footprint. Charging all of that to the mobile set would hide the receiver. Charging it all to local infrastructure would hide the national force requirement.

The $16.8 billion spread between `A1` and `A4` is therefore not an estimate of “the price of resilience.” It is a controlled acquisition variable within one technology program. Real site acquisition, carrier redesign, source-specific treatment, distribution construction and operating cost remain outside this replacement calculation.

Mobility also changes. Declared dry mass rises from about 3,994 tonnes for `A1` to 4,324 tonnes for `A4`. Chargeable burden rises from about 4,142 to 4,496 tonnes. The range is smaller than the variation among Pass 64 pipe technologies because all four architectures use the same sectional reference material. That is intentional. This pass isolates topology. The surviving topology should later be crossed with the sectional, reeled, field-extruded and fold-flat material rivals rather than selecting both variables from one paper screen.

## 8. Force-design consequences

### Readiness becomes a continuously observed state

A formation cannot be reported ready because its storage modules exist in inventory. The readiness ledger must include usable volume, sector isolation, water age, quality release, pump and power state, distribution availability, route status, repair inventory and time since representative trial. A change in any one may revoke a failure claim without changing the equipment count.

This resembles ammunition, fuel and platform mission-system readiness more than ordinary emergency stock reporting. It requires custody, telemetry, thresholds, independent assurance and an operational authority empowered to deny a deployment claim.

### The receiver becomes part of the formation

Storage, corridors and public distribution occupy geography. A mobile water group cannot carry every easement, anchor, sanitary basin, crossing and alternate public interface in its vehicles. The complete formation is therefore a contract between generated mobile capacity and prepared receiver capacity.

The receiver must maintain sites, access, route surveys, cross-connections, sanitary works, local labor interfaces, quality authority and public-service plans before activation. That fixed capacity is not assistance supplied by a subordinate partner. It is one half of the force system and must receive capital, inspections and readiness status.

### Corridor independence becomes an acquired property

“Separate routes” must be decomposed. Physical distance alone is insufficient. Two paths can be spatially separate and still share a bridge, power feeder, control network, intake, treatment train, access road, maintenance crew, cyber dependency or floodplain. The configuration authority must register common causes and the proving enterprise must seed them.

Route-survey technology should optimize correlated-loss exposure rather than shortest distance. Autonomous mapping, subsurface sensing, damage forecasting and rapid civil-rights workflows could become decisive mission systems. Their output must remain contestable and auditable because a routing algorithm can silently concentrate risk.

### Recovery and the second event enter the mission

The failure worlds end when service is restored, but the force is not ready for another event until the damaged line is repaired, bypass recovered, tanks refilled, contaminated sectors sanitized, consumables replaced, evidence recorded and crews reset. A design that passes once and requires weeks of bespoke recovery may be operationally inferior to a slightly heavier system with fast regeneration.

The representative mission must therefore include a second activation. This is where reusable conduits, standardized couplings, automated cleaning, replaceable liners, distributed spares and configuration discipline become force multipliers.

## 9. Technology competitions implied by the architecture

The Department of Resilience should use this failure model to drive technologies that do not yet exist at mature scale.

**Autonomous sanitary storage** should combine rapidly erected structure, low-mass liners, automated cleaning and disinfection, water-age management, sector isolation, protected pumping and continuous trusted inventory. The critical innovation is not capacity alone; it is the ability to know which volume is safe and deliverable after damage.

**Robotic bypass emplacement** should survey a damaged block, prepare access, position conduit, make large-bore sanitary connections, pressure test, disinfect, flush and obtain independent release inside a six-hour target. A machine that lays hose quickly but cannot close quality and pressure authority has not met the requirement.

**Correlation-aware route autonomy** should produce multiple feasible corridors whose shared dependencies are explicit. It must combine terrain, subsurface conditions, contamination, access, crossings, population use, workfront productivity and damage propagation. The acquisition metric is surviving service under seeded common cause, not routing speed.

**Treatment headroom and modular overdrive** should compete three mechanisms: permanent reserve trains, short-duration overdrive in existing trains and receiver precharge. Overdrive may reduce capital but increase membrane, chemical, energy and residual stress. The useful output is resilient-ready time across source cases, not nameplate flow.

**Distributed public-service islands** should allow a receiver-wide network hold without eliminating all safe access. Each island would require isolated water quality, power, pressure, communications, queue management and accessible distribution. Islands could be fed from alternate trunks, mobile treatment or sealed storage. Their purpose is to turn `W7` from a universal failure into a bounded switching problem.

**Trusted readiness telemetry** should record inventory and quality without creating a single cyber or governance common mode. Local manual verification, independent sensing, signed state transitions and degraded communications are part of the architecture. The force must be able to operate safely when national networks are unavailable.

These programs should remain rival portfolios. The model does not prove that four-sector storage, a six-hour bypass or a twenty-five-percent treatment reserve is optimal. It defines the experimental surface on which different mechanisms can compete.

## 10. Evidence contract

Fourteen gates govern the next stage:

1. continuous verified storage charge and sector state;
2. separate first-water and resilient-ready cold-start milestones;
3. a representative single-line rupture;
4. rupture with an uncharged buffer;
5. delayed repair with partial inventory;
6. common-corridor severance;
7. storage-sector contamination during source loss;
8. a full treatment-train outage;
9. safe alternate service during receiver contamination hold;
10. hydraulic transient control during startup, trip, isolation, cross-connect and bypass;
11. demonstrated route independence for `A4`;
12. certified half-flow bypass at or before six hours for `A3`;
13. recovery, sanitation, configuration reset and a second mission; and
14. rendering release only after representative physics and degraded-service evidence.

All thirteen technical and mission gates are open. The rendering gate is blocked. A declared pass in the workbook is a target for a trial; it is not an admission result. The independent research, test and evaluation authority—not the generating service or contractor—must release the evidence.

This distinction prevents a familiar acquisition error. A spreadsheet can verify arithmetic consistency and sensitivity. It cannot establish installation rate, pipe durability, connection sanitation, route independence, human access or service continuity. The workbook’s twenty-eight passing integrity checks prove that its own relationships reconcile. They do not prove the field system.

## 11. Acquisition decision and next proof

No architecture should be selected. `A1` should remain the control. `A2` and `A3` should advance because they reach the same declared score through different mechanisms. `A4` should advance as the test leader and upper comparator. The next proving campaign should build paired same-corridor and separated-route trials, instrument storage state, seed ruptures before and after charging, impose a compound sector-and-treatment loss, recover the configuration and repeat the mission.

The next architectural pass should also move outward from the local receiver. Every current rival fails `W7`. A useful successor is a **federated receiver architecture**: two or more prepared public-service islands or receiving nodes with independent quality release and a controlled switching path. That study should ask how much receiver separation, mobile branching, storage, local power and public-access capacity is required to maintain the fifty-percent floor when one receiver is placed on hold.

In parallel, the object-level configuration program should release one architecture’s fittings, valves, anchors, storage manifolds, pumps, sensors, generators, sanitation equipment, bypass connections, tools, spares and crews as serialized transport objects. Percentage allowances are no longer sufficient for the protection mechanism.

Only after these steps should the architecture be crossed with Pass 64’s four conveyance technologies. Otherwise the study would confuse the best pipe form with the best failure topology and could prematurely optimize an unproven combination.

## Conclusion

The first-reach water force cannot be understood as a pipeline that begins producing service when the last joint closes. It is a stateful public utility assembled across mobile equipment and prepared geography. Its ability to survive depends on where water is stored, whether that water is clean and charged, which routes and sectors remain independent, how quickly a bypass can be released, whether treatment has reserve, and whether the receiver itself can lawfully distribute water.

Pass 65 corrects the prior bulk-flow inference and makes the consequence measurable. A charged centralized buffer can bridge one ordinary rupture. Same-corridor twin lines and a staged bypass produce different four-world protection strategies. Separated lines and distributed storage lead the declared screen but still fail a receiver-wide hold. The resulting $110.4–127.2 billion program range and 3,994–4,324-tonne dry-system range make the cost and mobility of those mechanisms visible without pretending they are estimates.

The Department of Resilience should treat this not as a choice among four diagrams but as the beginning of a military-grade mission-system competition. It must acquire rival architectures, prepared receivers, proving geography, independent evidence, regeneration and the industrial capacity to learn from repeated failure. The successful object is not the pipe, the tank or the treatment plant. It is safe public service that remains present when one of them disappears.
