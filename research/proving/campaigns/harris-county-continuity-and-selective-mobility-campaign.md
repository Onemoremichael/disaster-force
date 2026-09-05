# Harris County continuity and selective-mobility campaign

**Status:** design-reference campaign; `R1/R2` architecture with `R2+` exploratory arithmetic

**Decision:** advance the protected-local assured neighborhood mesh (`H3`) only as the next test architecture. Admit no architecture as a national reference from this campaign.

**Companion model:** [Harris County continuity and mobility campaign](../../../models/harris-county-continuity-mobility-campaign.xlsx)

## Interim judgment

The national doctrine survives contact with a metropolitan road network, but in a more demanding form.

The correct alternative to mass relocation is not simply more local shelter, power, water, or cooling. It is a **protected local operating system with an assured neighborhood access layer**. People must be able to reach that system, be reached inside buildings, or move from it into a complete civil-mobility chain when remaining becomes unsafe. The force therefore needs a formation below the regional transfer node and beside the occupied district: a **Neighborhood Continuity and Access Cell (`NCAC`)**.

An `NCAC` is the smallest formation that can bind six things into one accountable operation:

1. a protected district with complete local service;
2. door- and building-level access, including vertical extraction;
3. an accessible neighborhood pickup and information mesh;
4. local route reconnaissance, control, clearance, bridging, repair, and marking;
5. a declared interface to a civil transfer node, clinical pathway, and receiving system; and
6. one rights, household, property, care, and return record that persists across the chain.

This is not a renamed bus company, rescue team, shelter staff, public-works crew, or incident-command liaison. It is a permanent combined-arms civil formation whose output is protected or restored person-hours. Its defining capability is not a vehicle. It is control of the seam between **remaining safely** and **moving safely**.

That requirement now has a first configuration. [`NCAC-35`](../../force/mobility/neighborhood-continuity-and-access-cell.md) uses one 61-tract analytical catchment from this campaign to compare four formations against approximately 35,000 demand people. The assured conventional cell requires about 7,587 deployed people and 6,388 packed tonnes. It survives eight declared physical losses but verifies only 79.6 percent of required households by hour 36 when commercial communications are unavailable. A technology target closes the arithmetic only through unproved offline records, higher access productivity, and lighter prepared-district imports. Neither formation is admitted.

The campaign also rejects a tempting procurement conclusion. More line-haul capacity does not solve the governing problem. In the reference case, movement-led `M0` creates a collection queue of about 266,682 people while its line-haul queue is effectively zero. Even the corrective `H3` architecture still peaks near 73,750 people waiting in collection. The scarce effect is early, accessible, block-to-node service—not distant seats.

## The decision this campaign tests

[Mobility assurance under deep uncertainty](../../force/mobility/mobility-assurance-under-deep-uncertainty.md) changed the national reference from a restorable movement mesh to protected-local continuity. That study was deliberately broad. It could show that a movement-heavy conclusion depended on a narrow probability distribution, but it could not answer four metropolitan questions:

- Can a person reach protected local service across damaged streets?
- When local service is unavailable, can the force reach the person before it can move the person?
- Does an apparently connected road graph create operational access quickly enough?
- Where does delay accumulate when protection, collection, transfer, line haul, destination admission, and return share one clock?

This campaign answers those questions at tract scale for Harris County, Texas, in a synthetic seven-day compound coastal-flood and lifeline-loss event. It is a **design-reference campaign**, not a replay of Hurricane Harvey, a forecast, a flood-loss estimate, an evacuation plan, a site recommendation, or a claim about the performance of existing agencies.

Political permission is assumed. Geography, access, time, demand, workforce, capacity, equity, and common failure are not.

## The campaign object

The analytical population is ten percent of the 2024 ACS tract population in Harris County, spatially weighted and then normalized to **481,049.8 people**. The fraction is a declared demand scale for comparing architectures, not an estimate of how many people would need help in a particular storm.

The force is evaluated every six hours through hour 168. Demand can be satisfied in only two ways:

- **local closure:** a person receives the required protected service in place or in an accessible nearby protected district; or
- **movement closure:** the person completes collection, transfer-node processing, line haul, and destination admission.

Departure does not count. Arrival at a terminal does not count. A seat does not count. People waiting in a building, in collection, at a transfer node, or before destination admission remain unprotected for the campaign clock.

The admission rule requires all four conditions in the same analytical world:

| Measure | Threshold | Why it exists |
| --- | ---: | --- |
| Seven-day total closure | at least 95% | aggregate service obligation |
| Seven-day priority closure | at least 95% | high-need demand cannot be traded away |
| Seven-day bottom-demand-decile closure | at least 80% | low-volume and peripheral tracts cannot disappear inside a county average |
| Mean unprotected time | no more than 60 h/person | eventual service cannot erase dangerous delay |

The thresholds are policy hypotheses. They create a falsifiable comparison; they do not establish medically sufficient service levels.

## Geography, exposure, and what the data do not say

The campaign joins four official data families with prior research-program configurations.

The road layer begins with the Census Bureau's 2025 Harris County TIGER/Line all-roads file. Selected motor-road features are split at every internal vertex, producing **65,144 features, 667,739 graph segments, and 584,857 graph nodes**. TIGER supplies geometry and MTFCC classification. It does not supply emergency direction, throughput, bridge survival, grade separation, debris, signal state, traffic, flood depth, or authority to use a road.

FEMA National Flood Hazard Layer polygons for DFIRM `48201C` place tract centroids and road segments into high, moderate, or low mapped-exposure classes. Those are regulatory screening classes. They are not event-specific inundation depth, duration, probability of closure, or an engineering fragility function.

The TxDOT evacuation-route feature layer marks designated routes. A model assumption gives marked segments a 30-percent restoration-time preference. The designation itself does not prove that a road survives, is controlled, has capacity, or remains reachable from a neighborhood.

ACS tables provide tract population, disability share, a zero-vehicle person proxy, and the share of housing units in structures with twenty or more units. The last is only a vertical-access proxy. Housing units are not residents; building size is not story count; story count is not elevator dependence; and elevator dependence is not assisted-extraction demand.

These boundaries matter because the model contains a network, not a solved transportation system. It is appropriate for architecture comparison and evidence-gap discovery. It is not appropriate for routing people in an incident.

## A research correction: intersection topology is not optional

The first implementation connected each TIGER feature only at its endpoints. That graph stranded most demand and appeared to prove that local road access was catastrophically sparse. The result was wrong.

Many road features contain internal vertices that must participate in the graph. Splitting features at those vertices changed the topology from an artifact into a useful first screen. The correction is preserved because it demonstrates a general assurance rule:

> A network model can be numerically reproducible and still be conceptually false if its representation erases the interfaces through which the real system works.

The corrected graph is still generous. It treats coincident geometry as connection without solving grade separation and treats restored geometry as traversable without solving lane capacity, control, bridge state, congestion, debris, or pickup dwell. Two tracts remain disconnected at hour 168 in the reference topology; that should be read as a graph-screen result, not proof of two physically inaccessible communities.

## Four rival architectures

The architectures are bundles, not isolated fleet choices.

| ID | Architecture | Governing wager | Reference local share | Active CTNs | Collection rate | Line-haul rate | Route groups |
| --- | --- | --- | ---: | ---: | ---: | ---: | ---: |
| `M0` | Movement-led surge | scale transfer and line haul; local continuity remains secondary | 20% | 7 | 2,800 people/hour | 3,200 people/hour | 10 |
| `B1` | Balanced continuity and movement | divide investment across local protection and movement | 65% | 5 | 1,800 people/hour | 2,100 people/hour | 8 |
| `P2` | Protected-local selective movement | protect most demand locally and move the mandatory remainder | 92% | 4 | 1,150 people/hour | 1,400 people/hour | 8 |
| `H3` | Protected-local assured neighborhood mesh | add faster local activation, building access, collection, and route assurance to `P2` | 95% | 5 | 1,800 people/hour | 2,000 people/hour | 14 |

`M0`, `B1`, and `P2` are the initial rivals. `H3` is a **post-result corrective rival** created after the first three exposed early collection as the dominant seam. It is therefore not an independent confirmation of a predeclared winner. It is a hypothesis generated by this campaign and must be replicated elsewhere.

All architectures carry some local protection, transfer, accessible continuity modules, route restoration, destination readiness, return capacity, command, bases, and sustainment. The comparison changes their balance and timing. It does not compare a complete system against a caricature with missing functions.

## Reference-campaign results

Under the declared reference assumptions, three architectures pass the arithmetic admission rule and the movement-led architecture fails.

| Measure | `M0` | `B1` | `P2` | `H3` |
| --- | ---: | ---: | ---: | ---: |
| Local closure, people | 72,905 | 246,611 | 357,263 | 370,610 |
| Movement demand, people | 408,145 | 234,438 | 123,786 | 110,440 |
| Movement caused by local-protection shortfall | 318,401 | 144,694 | 34,042 | 20,696 |
| Closure at hour 72 | 34.4% | 65.9% | 82.1% | 83.6% |
| Closure at hour 168 | 79.8% | 99.1% | 99.7% | 99.7% |
| Priority closure at hour 168 | 79.9% | 99.5% | 99.8% | 99.8% |
| Bottom-decile closure at hour 168 | 17.9% | 91.3% | 97.3% | 97.4% |
| Mean unprotected time, h/person | 103.9 | 56.9 | 29.6 | 24.1 |
| Peak collection queue, people | 266,682 | 145,936 | 79,584 | 73,750 |
| Peak CTN queue, people | 45,980 | 4,746 | 0 | 2,343 |
| Network-stranded at hour 168 | 2,014 | 1,567 | 1,297 | 1,266 |
| Displaced at day seven | 224,624 | 122,250 | 59,401 | 36,255 |
| Reference result | fail | pass | pass | pass |

The important distinction is between **mandatory movement** and **movement created by inadequate local protection**. The reference demand contains about 89,744 people who must move because of the modeled hazard, access, or service state. `M0` adds more than 318,000 people to that chain because its local system is weak. `H3` adds about 20,696. The former uses mobility to compensate for an absent public service; the latter reserves mobility for the smaller population whose needs cannot safely be met locally.

The time profile matters as much as the final percentage. `H3` reaches 77.4-percent closure at hour 18 and 83.6 percent at hour 72, then climbs slowly toward 99.7 percent. The plateau is the signature of residual collection, building access, and network restoration demand. This is why a seven-day result cannot substitute for an hour-by-hour protection account.

## The broad-world test

The model then varies campaign demand, mandatory-movement burden, local-protection realization, road-restoration time, collection, CTN processing, line haul, destination intake, accessible-module capacity, restoration, and return across **300 paired broad worlds per architecture**. The same sampled world is applied to all four architectures. The ranges are intentionally broad and mostly judgmental.

These are not event probabilities. A success share means “fraction of declared stress combinations passed,” not “chance this force succeeds in Harris County.”

| Architecture | Complete-rule success | Mean closure | P05 closure | Mean priority | Mean bottom decile | P95 unprotected h/person |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| `M0` | 0.0% | 66.1% | 56.1% | 67.7% | 11.5% | 120.6 |
| `B1` | 0.7% | 80.7% | 71.9% | 82.2% | 42.2% | 86.7 |
| `P2` | 11.7% | 86.2% | 75.5% | 87.4% | 55.0% | 65.0 |
| `H3` | 55.3% | 94.4% | 81.7% | 94.5% | 75.0% | 52.5 |

`H3` is best in all 300 paired worlds. It nevertheless fails the complete rule in **134 worlds**. Winning a weak field is not admission.

The failure pattern is diagnostic:

- `M0` fails every criterion in every world.
- `B1` fails total closure in 293 worlds, priority closure in 291, bottom-decile closure in 298, and exposure in 288.
- `P2` fails total closure in 252, priority closure in 242, bottom-decile closure in 262, and exposure in 44.
- `H3` fails total closure in 112, priority closure in 107, and bottom-decile closure in 134, but does not fail the 60-hour exposure criterion.

The corrective architecture therefore solves average waiting more readily than distributional completeness. It protects people much sooner while still leaving too many lower-demand tracts short in adverse combinations. The next design task is not simply faster average service. It is assurance at the edge of the operating area.

## What governs performance

Within the declared ranges, the rank association between `H3` closure and realized local protection is `+0.461`; the association with mandatory movement is `-0.281`, and with collection capacity `+0.117`. For `P2`, the local-protection association rises to `+0.787`. `M0` is governed primarily by demand (`-0.754`).

These are Spearman rank associations inside one experimental design. They are not causal elasticities and will change if the ranges change. Their value is architectural: once local protection is weak, the whole campaign becomes a demand-amplification machine. Once local protection becomes strong, the governing uncertainty migrates toward who still must move, how early the force reaches them, and whether peripheral tracts receive complete service.

The corrected road graph tells the same story. In the `H3` reference network, reachable demand is about 41.3 percent at hour zero, 51.3 percent at hour 48, 63.0 percent at hour 72, 73.0 percent at hour 96, and 99.5 percent at hour 120. The graph becomes almost fully connected before the service chain closes. Later line-haul capacity cannot repair an early interval in which a person lacks safe local service and cannot reach collection.

## The Neighborhood Continuity and Access Cell

The `NCAC` is the formation implied by the result. It occupies the seam between `PCC-D1`, `CTN-10`, the route-assurance group, the `UCM-8` module, and local civil authority. None of those existing concepts alone owns the complete seam.

### Mission

For a bounded neighborhood population and access envelope, the cell must:

- establish a verified common operating picture down to buildings and blocks;
- activate complete local service where safe;
- identify people whose needs cannot be met locally;
- perform or coordinate accessible door- and vertical extraction;
- create reachable pickup points and mobile service contacts;
- open, control, mark, and sustain local routes;
- regulate movement into transfer, clinical, and destination capacity;
- preserve consent, family, care, property, benefit, and privacy records; and
- maintain the option to return people as local service and origin safety recover.

### Internal elements

The first organizational hypothesis contains eight mutually dependent elements:

| Element | Required effect | Failure if omitted |
| --- | --- | --- |
| Civil authority and rights team | lawful priority, consent, remedy, household integrity, local legitimacy | speed becomes coercion or unaccountable exclusion |
| Building access platoons | assessment, stairs/elevators, assisted descent, litter movement, welfare checks | reachable roads do not make residents reachable |
| Neighborhood service detachments | water, power, thermal, communications, health, sanitation, food interface | movement demand expands because protection is incomplete |
| Collection squadrons | accessible vehicles, dispatch, loading, clinical separation, household movement | people accumulate between buildings and the network |
| Route-assurance companies | reconnaissance, debris clearance, pumps, bridging, traffic control, repair, marking | mapped connectivity does not become operability |
| Mobility-regulation center | match people, mode, node, destination, care, custody, and return | local optimization overloads the next stage |
| Maintenance and sustainment company | fuel/energy, charging, spares, cleaning, decontamination, crew relief | early throughput collapses after the first operational period |
| Data and communications section | offline identity/household record, service status, route state, audit trail | the chain fragments when commercial networks fail |

The table is a functional architecture, not a billet authorization. The campaign does not yet establish how many cells Harris County requires, how many people belong in one cell, which functions should be organic, or which equipment class should carry them.

### Command relationship

The cell should be generated jointly by the Community Stabilization, Civil Mobility and Continuity, Land Engineering, Infrastructure Restoration, and Health Protection Services. In employment it should report to a geographic joint effect command and operate under the affected civil authority's outcome priorities. Technical release authority remains with the competent engineering, clinical, environmental, transport, and safety professions.

This is an intentionally difficult arrangement. The seam is cross-professional by nature. Assigning it to whichever organization arrives first would reproduce the fragmentation the Department is meant to abolish.

### Readiness standard

An `NCAC` is ready only if a representative population can be contacted, protected, extracted, collected, transferred, admitted, and returned under simultaneous loss of commercial power, communications, several road classes, one supplier, and one command node. Separate demonstrations of shelter, buses, road clearing, and registration do not sum to cell readiness.

## Technology programs generated by the campaign

The campaign produces mission-driven invention requirements rather than vehicle concepts ready for rendering.

### Vertical continuity and extraction system

The objective is not a faster stair chair. It is a building-to-safe-service system for high-rise and multi-unit structures after power, water, elevators, communications, and normal staffing fail. Rival concepts should combine building status sensing, portable elevator or hoist power where feasible, powered ascent/descent aids, low-burden assisted movement, responder load reduction, resident communications, and continuity of medical equipment.

The proving question is: **how many representative residents can remain safely served or be moved from a damaged building per crew-hour without avoidable injury, separation, or power dependence?**

### Flood-passable collection mesh

This program should explore purpose-built families of accessible road, high-water, low-ground-pressure, and shallow-water vehicles with a common cabin and restraint interface. Autonomy may reposition empty vehicles, scout routes, and reduce exposure; accountable people retain authority over passenger movement.

The proving question is the complete duty cycle: dispatch, approach, curb or building interface, loading, clinical and mobility-device accommodation, travel, unloading, energy, cleaning, maintenance, crew relief, and degraded manual recovery.

### Transferable neighborhood service point

The force needs a protected point that can begin as a local continuity site, become a collection point, and later interface with a `CTN` without re-registering or re-triaging everyone. Power, clean air, water, sanitation, communications, clinical stabilization, mobility-device energy, family waiting, and records must scale as the site's role changes.

### Dynamic civil route assurance

The route program should combine dense sensing, unmanned reconnaissance, rapid road and culvert repair, temporary bridging, localized pumping, debris systems, traffic control, and offline machine-readable route status. Its output is not kilometers cleared. It is a route envelope certified for a declared vehicle, passenger, load, and time window.

### Intermittent civil identity and continuity record

The Department needs a privacy-preserving, offline-first household and care record that can reconcile after disconnection without creating a permanent domestic movement-surveillance system. It must support consent, accessibility, family integrity, clinical escalation, property custody, benefits, destination admission, and return while minimizing data collection and enabling independent remedy.

### Neighborhood operations digital twin

A useful system would fuse building condition, road state, service availability, queues, vehicles, personnel, receiving capacity, and uncertainty into an operational model that remains auditable under degraded communications. This is not authorization for autonomous civil control. The machine may recommend; accountable civil and professional authorities decide.

None of these programs has earned a platform image. Each must first close a requirement, alternatives screen, physics and human-system model, degraded modes, safety case, formation fit, and representative mission trial.

## Workforce and industrial consequence

The reference architecture workforces are campaign-deployed staffing hypotheses:

| Architecture | Deployed people |
| --- | ---: |
| `M0` | 47,919 |
| `B1` | 46,150 |
| `P2` | 46,267 |
| `H3` | 56,554 |

The protected-local alternatives are not labor-light. `P2` moves far fewer people than `M0` with approximately the same deployed workforce because labor moves from terminals and line haul into protected-local operations. `H3` adds about 10,287 people over `P2`, principally for faster local protection, collection, transfer, route assurance, and their command and relief burden.

That is strategically important. A Department optimized around local protection needs a large national profession of district operators, building-access specialists, accessible-mobility crews, route engineers, community-service personnel, maintainers, clinical regulators, dispatchers, civil-rights officers, and receiving staff. It cannot be assembled only from occasional volunteers or borrowed utility and transit workers during a regional catastrophe.

The industrial demand likewise shifts. The major market is not only large evacuation vehicles. It includes protected district kits; all-condition accessible collection fleets; portable building-access systems; distributed pumps, bridges, and road repair; rugged service points; interoperable cabin and restraint modules; offline operational systems; depot maintenance; training environments; and full-mission proving ranges.

## Fiscal frame

The campaign includes a first-order comparative fiscal account in real 2026 dollars. It is not an independent cost estimate and it is not additive to the Department-wide models.

| Architecture | Capital | Mature annual operations | Capital plus 25 years of operations |
| --- | ---: | ---: | ---: |
| `M0` | $116.16B | $17.92B | $564.11B |
| `B1` | $97.80B | $16.13B | $501.08B |
| `P2` | $87.69B | $15.34B | $471.26B |
| `H3` | $115.32B | $19.41B | $600.45B |

Inside the declared frame, `P2` is both the least expensive and a much stronger architecture than `M0`; local protection avoids moving, processing, receiving, and returning people whose service can safely be maintained near home. `H3` costs more because the corrective architecture buys assured last-mile access and additional workforce. Its higher broad-world performance is not a benefit-cost result: the model lacks empirical failure distributions, causal health and social benefits, independent unit costs, learning curves, supplier constraints, and residual value.

The useful fiscal finding is architectural. Capital categories must be organized around complete neighborhood service and access, not around separate grants for shelters, buses, roads, terminals, or registration systems. Otherwise each program can appear efficient while the seam remains unfunded.

## Rights, legitimacy, and return

Protection-first doctrine carries its own civil-rights risk. “Shelter in place” can become abandonment if the state uses local protection as a reason not to reach people. Selective movement can become coercive if eligibility, warning, consent, destination, family separation, property custody, or return are opaque.

The `NCAC` therefore requires public rules before an event:

- the service conditions under which remaining is safe;
- the conditions that trigger an offer or requirement to move;
- who decides and how the decision can be reviewed;
- what assistance is available regardless of disability, language, immigration status, income, vehicle access, incarceration, institutional residence, or digital access;
- how households, caregivers, service animals, mobility devices, medications, records, and essential property remain together;
- how data are minimized, secured, expired, and corrected;
- what the receiving destination owes; and
- who pays for and authorizes return or durable settlement.

Bottom-decile closure is included because a county average can hide geographic abandonment. It is still a crude safeguard. The next campaign must test distribution by disability, zero-vehicle status, building condition, institutional setting, language, income, race and ethnicity, medical dependence, and civil status without turning demographic data into an automated entitlement or coercion score.

## What the campaign changes

The campaign modifies six parts of the mature force concept.

1. **Protected-local continuity remains the national doctrine, but it gains an access obligation.** Service that exists across an impassable block or inaccessible stair is not local protection for the person who needs it.
2. **Collection becomes an operational maneuver layer.** It requires command, vehicles, building access, routing, maintenance, and assurance at formation scale.
3. **Route restoration must be planned from people outward.** Strategic corridors do not close a mission when neighborhood approach and pickup remain broken.
4. **The transfer node is downstream of a neighborhood force.** `CTN-10` cannot be the first accountable owner of a person journey.
5. **Mobility demand is partially endogenous.** A weak local service architecture manufactures passengers; a strong one preserves scarce movement capacity for mandatory cases.
6. **Distributional assurance is a design driver.** `H3` solves mean exposure before it solves bottom-decile closure, so edge access—not average throughput—is the next frontier.

## What the campaign does not establish

All eighteen campaign evidence gates remain open. The most decision-relevant limitations are:

- the flood layer is regulatory exposure, not a simulated event;
- the road graph does not represent bridges, grade separation, direction, capacity, traffic, debris, control, or actual closure;
- no parcel, building, story, elevator, resident, institutional, or medical-equipment inventory is present;
- household demand timing, compliance, spontaneous movement, and refusal are assumed;
- local protection, collection, CTN, line-haul, destination, restoration, and return performance are planning factors;
- broad-world ranges are not fitted joint distributions;
- workforce values are task-class factors, not occupation and qualification models;
- costs are unit-factor comparisons, not acquisition or lifecycle estimates;
- destination sites, legal authorities, host agreements, and origin-release conditions are not solved; and
- `H3` was generated after reviewing initial results and has not been independently replicated.

An internally consistent workbook is evidence that the declared experiment ran as specified. It is not evidence that the architecture will perform in the world.

## Decision and next research campaign

No architecture is admitted as a national reference from this pass. `M0`, `B1`, and `P2` remain comparison subsystems. `H3` advances as the next test architecture because it dominates the declared rivals in every paired world and cuts mean reference exposure to 24.1 hours per demand person. Its 55.3-percent complete-rule success is far below a force-admission standard.

The next pass should do two things in sequence.

First, configure one `NCAC` around a bounded Harris County operating area. Replace shares and aggregate rates with a building inventory, named service points, explicit crew tasks, accessible vehicle cycles, route classes, energy and fuel, maintenance, communications, data custody, command, shift relief, and itemized deployment. The design should fail if the cell cannot reach its assigned buildings and close a complete person journey while one service point, one route group, and commercial communications are lost.

Second, preregister and repeat the architecture comparison in a different metropolitan system with a different hazard and built form. Pass 38 selects New York extreme heat plus prolonged power and communications loss because it shifts the dominant network into occupied vertical buildings while leaving much road pavement physically present. The ranges and admission rule are fixed before the corrective architecture sees the result.

Only after those tests should the Department decide whether `NCAC` is a permanent formation, how it nests under a campaign cell, and which novel machines deserve first-principles configuration.

The resulting [New York vertical heat-blackout protocol](new-york-vertical-heat-blackout-replication-protocol.md) reports no outcomes. Its companion [full-mission test program](../test-enterprise/ncac-full-mission-test-program.md) converts the representative experiment into a staged, independently governed evidence enterprise.

## Sources and interpretation boundaries

1. U.S. Census Bureau, [2025 TIGER/Line technical documentation](https://www.census.gov/programs-surveys/geography/technical-documentation/complete-technical-documentation/tiger-geo-line.2025.html) and Harris County all-roads file. Used for geometry and MTFCC class only.
2. Federal Emergency Management Agency, [National Flood Hazard Layer](https://hazards.fema.gov/arcgis/rest/services/public/NFHL/MapServer/28), Harris County DFIRM `48201C`. Used for regulatory mapped-exposure classification only.
3. Texas Department of Transportation, [Evacuation Routes feature layer](https://services.arcgis.com/KTcxiTD9dsQw4r7Z/arcgis/rest/services/TxDOT_Evacuation_Routes/FeatureServer/0). Used only as a designated-route marker.
4. U.S. Census Bureau, 2024 ACS five-year tables `B18101`, `B08201`, and `B25024`. Used for tract disability share, zero-vehicle proxy, and 20-plus-unit structure proxy with the limitations stated above.
5. Disaster Force research program, [Civil Mobility Assurance Under Deep Uncertainty](../../force/mobility/mobility-assurance-under-deep-uncertainty.md). Used for the first `CTN-10` and `UCM-8` configuration hypotheses.
