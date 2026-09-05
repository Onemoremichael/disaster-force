# Mission engineering: converting catastrophe into force demand

## Purpose

Mission engineering is the bridge between the Department of Resilience and its eventual systems. It converts a scientifically plausible event into time-phased demands for civilian effects, then converts those effects into complete mission packages, deployment flows, sustainment, and force-generation depth.

The method is designed to prevent three recurring errors:

1. sizing to hazard magnitude rather than human service failure;
2. treating everyone inside a damage polygon as having the same need; and
3. converting a production requirement directly into a platform count without access, connection, distribution, endurance, or rotation.

## The analytical chain

Every design reference mission follows the same chain:

```text
hazard sequence
    ↓
physical damage and environmental conditions
    ↓
service-system failures and restoration trajectories
    ↓
population and critical-function exposure
    ↓
unmet service demand by place and time
    ↓
required resilience effects and quality levels
    ↓
mission modules, reception, distribution, and sustainment
    ↓
deployment flow and time to stabilized life-support
    ↓
force inventory, crews, bases, lift, maintenance, and industrial depth
```

Skipping a link creates false precision. A million people without piped water does not automatically imply a million-person desalination plant: some have household stocks, some can evacuate, some systems restore quickly, some need only drinking water, hospitals require additional process water, and distribution may be more limiting than treatment.

## Unit of analysis: population-service-time cells

The fundamental demand record is a population or critical function (p), in location (g), requiring service (s), during time interval (t):

\[
D_{p,g,s,t} = N_{p,g,t} \times q_{p,s,t} \times f^{outage}_{g,s,t} \times f^{unmet}_{p,g,s,t} \times k^{access}_{g,t}
\]

where:

- (N) is the relevant people, beds, facilities, or economic functions;
- (q) is the service level per unit;
- (f^{outage}) is the share losing ordinary service;
- (f^{unmet}) is the share not covered by household, local, utility, commercial, or mutual-aid capacity; and
- (k^{access}) adjusts the mission burden for isolation, congestion, contamination, or damaged receiving infrastructure.

Demand is never a single peak number. It is a curve. Search and rescue may peak in hours; emergency water in days; dialysis and chronic care recur; debris and temporary housing persist for months.

## Population segmentation

At minimum, every scenario separates:

- people able to remain safely at home with partial services;
- people sheltering locally;
- people requiring supported evacuation;
- people in congregate or non-congregate shelter;
- people isolated by damaged access;
- hospital inpatients and emergency patients by acuity;
- people dependent on electricity for medical or mobility needs;
- institutional populations, including long-term care and detention;
- people without vehicles, documentation, banking, communications, or secure housing;
- responders and the support population they add; and
- animals, agriculture, and industrial processes where their failure creates human or environmental consequences.

The segments may overlap. The model must prevent double counting while retaining compounding needs.

## Service levels are phased

Each service uses at least four levels:

| Level | Meaning | Modeling use |
|---|---|---|
| Survival | Minimum that prevents imminent death or irreversible harm | No-notice first hours and isolated populations |
| Emergency | Safe short-duration service compatible with public-health and protection standards | Initial stabilization |
| Stabilized | Sustainable service adequate for weeks to months without progressive harm | Enduring campaign target |
| Transfer | Service quality, reliability, ownership, and maintainability sufficient for responsible civil operation | Demobilization condition |

The Department should not normalize survival conditions as acceptable long-duration service. CDC's household storage recommendation of at least one gallon per person per day is a preparedness floor for drinking, cooking, and hygiene, not a complete municipal water-service standard.[^cdc-water] WHO emergency guidance likewise uses phased water quantities and emphasizes additional non-domestic requirements for health facilities and sanitation.[^who-water]

## Restoration trajectories

For each ordinary service, the scenario defines a restoration curve:

\[
U_{s,t} = 1 - R_{s,t}
\]

where (R) is the share of pre-event service restored and (U) the unresolved outage share. A useful curve records at least:

- immediate surviving capacity;
- 24-hour, 72-hour, 7-day, 30-day, 90-day, and 180-day restoration;
- geographic islands of slower restoration;
- quality or reliability degradation despite nominal reconnection; and
- dependencies that can stall or reverse recovery.

The force demand is the gap between required service and credible restoration by responsible owners. It falls as ordinary systems recover, unless displacement, heat, disease, or secondary hazards cause a new peak.

## Dependency graph

Every mission includes a directed service graph. A simplified graph is:

```text
access ─┬─→ fuel ─→ power ─┬─→ water/wastewater ─→ health
        │                  ├─→ communications ─→ coordination
        │                  ├─→ cooling/heating ─→ shelter safety
        │                  └─→ commerce and food cold chain
        ├─→ medical movement and supply
        ├─→ debris removal and repair crews
        └─→ distribution and evacuation
```

The graph is used to identify critical path effects. If temporary power requires fuel deliveries across a failed bridge, bridge access may be the first power mission. If a hospital has power but no wastewater discharge, sanitation may set usable bed capacity.

## From gross demand to Force demand

The Department is not required to replace every failed unit of ordinary service. The model subtracts four capacity layers in order:

1. surviving household, facility, and utility capacity;
2. local and state response plus sector mutual aid;
3. commercial and nonprofit capacity that remains genuinely available under the scenario; and
4. allied, compact, or other federal capacity assigned without undermining the Department's assured floor.

Only verifiable capacity is subtracted. Contracts subject to the same regional outage, clinicians employed by damaged hospitals, generators without fuel, and trucks without drivers or routes are not independent capacity.

## Geography and access classes

Demand is grouped by operational access, not just jurisdiction:

- intact metropolitan network;
- congested or partially damaged urban network;
- flooded shallow-water zone;
- deep or moving-water zone;
- debris-isolated corridor;
- mountainous or landslide-isolated community;
- remote rural or tribal area;
- island with functioning port or airport;
- island with both port and airport impaired;
- coastal area accessible from sea but not land;
- contaminated or exclusion zone; and
- extreme heat, cold, smoke, wind, or fire environment.

Each access class changes payload, crew protection, transfer point, cycle time, and daily throughput.

## Capacity conversion

For module type (m), the required number operating in interval (t) is:

\[
M_{m,t} = \left\lceil \frac{D^{unmet}_{s,t}}{C^{net}_{m,s,t}} \right\rceil
\]

Net capacity subtracts module self-consumption, downtime, quality losses, and distribution loss:

\[
C^{net} = C^{rated} \times A^{field} \times Y^{quality} \times Y^{distribution} - C^{self}
\]

Procured inventory then applies movement, maintenance, training, rotation, contamination, and concurrency factors as defined in the readiness pass.

## Time-to-effect budget

Every reference mission assigns a maximum acceptable time to each link:

| Link | Question |
|---|---|
| Decision | When is enough known to alert, stage, or employ? |
| Alert and marshal | Are crew, equipment, consumables, and documentation already paired? |
| Strategic movement | What route survives and what is its realistic cycle time? |
| Reception | Can the destination unload, stage, fuel, and direct the module? |
| Setup | How long from arrival to safe technical operation? |
| Connection | What site work, inspection, switching, intake, discharge, or data integration is required? |
| Distribution | When does the intended person or facility receive the service? |
| Scale | When does initial effect grow to full required output? |

The required time is derived from consequence escalation. The design response may be forward posture, lighter entry systems, a faster connection standard, redundant reception, or anticipatory authority—not necessarily a faster vehicle.

## Scenario record

Each design reference mission must contain:

1. scientific basis and scenario date;
2. event sequence and uncertainty range;
3. affected geography and population;
4. damage and environmental conditions;
5. service outage and restoration curves;
6. population segments and critical facilities;
7. local, commercial, and partner capacity assumptions;
8. service-level targets;
9. dependency graph and critical path;
10. required mission modules by time and access class;
11. deployment, reception, distribution, and sustainment flow;
12. transfer conditions;
13. concurrent national commitments;
14. principal failure modes; and
15. sensitivity cases.

## Evidence classes

Inputs are labeled:

- **O:** observed event data;
- **M:** authoritative modeled scenario;
- **S:** published standard or guidance;
- **E:** engineering estimate;
- **A:** explicit design-study assumption; or
- **D:** derived value calculated from labeled inputs.

Ranges are preserved through the chain. Design-study assumptions are visually distinct in the later workbook and never cited as observed facts.

## Platform gate restated

A major system may enter concept design only when at least one reference mission establishes:

- a material unmet effect at a stated time and place;
- the capacity, quality, access, and endurance required;
- why distributed conventional means, mitigation, evacuation, contracting, or repair cannot meet it adequately;
- the number of simultaneous operating systems and rotation depth;
- the reception, connection, distribution, waste, and transfer system; and
- lifecycle and industrial variables needed for comparison.

The mission model is therefore not preliminary paperwork. It is the design authority.

[^cdc-water]: Centers for Disease Control and Prevention, [*How to Create an Emergency Water Supply*](https://www.cdc.gov/water-emergency/about/how-to-create-and-store-an-emergency-water-supply.html), June 27, 2025.
[^who-water]: World Health Organization, [*How Much Water Is Needed in Emergencies*](https://www.who.int/docs/default-source/wash-documents/wash-in-emergencies/technical-notes-on-wash-in-emergencies/who-tn-09-how-much-water-is-needed.pdf), Technical Note 9, accessed September 4, 2026.
