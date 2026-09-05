# Design reference missions

## Mission set

No single catastrophe can size the Department of Resilience. The initial set deliberately stresses different combinations of warning, geography, infrastructure correlation, duration, seasonality, and access.

| Code | Design reference mission | Primary design stress |
|---|---|---|
| DRM-1 | Bay-region no-notice earthquake and urban fire | No warning, dense lifeline interdependence, port and road damage, fires without water, prolonged displacement |
| DRM-2 | California atmospheric-river megaflood | Enormous flooded area, long dewatering, agricultural and hazardous contamination, mass movement, months of public works |
| DRM-3 | Gulf–Atlantic major hurricane sequence | Forecast staging, coastal and inland flood, wind, port disruption, two landfalls competing for the same force |
| DRM-4 | Cascadia earthquake and tsunami | Regional isolation, destroyed coastal access, long-range reception, medical evacuation, ports and fuel |
| DRM-5 | Western wildfire–heat–smoke complex | Simultaneous incidents, mobile fire front, aviation saturation, heat mortality, smoke and grid stress |
| DRM-6 | Continental grid failure during temperature extreme | Systemic rather than regional event, fuel and communications dependence, health and water cascades |
| DRM-7 | Caribbean territory compound catastrophe | Island logistics, port and airport restoration, water and power replacement, months of external sustainment |
| DRM-8 | National respiratory epidemic plus regional disasters | Workforce attrition, medical supply and bed competition, shelter modification, persistent nationwide demand |
| DRM-9 | Great Plains–Mississippi drought and water emergency | Slow onset, agriculture and municipal competition, long-distance water and economic continuity |
| DRM-10 | Allied coastal megacity earthquake | Intercontinental deployment, host-nation integration, sovereignty, unfamiliar standards, global sustainment |

The set is not a forecast of the ten most likely events. It is an engineering test suite. Additional technological, cyber, conflict-related, dam-failure, volcanic, Arctic, and hazardous-material cases can be added when they generate a materially different force requirement.

## Common time windows

Every mission is analyzed in the same windows:

- **H0–6:** survival, reconnaissance, local rescue, warning, and authority;
- **H6–24:** initial national entry and critical-facility bridging;
- **D1–3:** rapid reinforcement and reception expansion;
- **D3–7:** mass effect and first replacement crews;
- **W2–4:** stabilized services and major public works;
- **M2–6:** enduring operations, interim infrastructure, housing transition, and industrial replenishment; and
- **transfer:** service-specific handoff rather than a single incident end date.

## DRM-1: Bay-region no-notice earthquake and urban fire

### Evidence anchor

The USGS HayWired scenario models a magnitude-7.0 Hayward Fault earthquake and cascading infrastructure and social effects. A USGS extension estimated approximately 3.7 million of 7.6 million residents without potable-water service soon after the event.[^haywired-water] The societal-consequences volume gives a mid-range displacement estimate of 750,000 people.[^haywired-social] The scenario also describes more than 400 possible gas- and electric-related fire ignitions, with fire response constrained by communications, roads, traffic, and water.[^haywired-fire]

These are modeled scenario outputs, not predictions or a worst case.

### Force-driving consequence chain

```text
ground motion and rupture
→ building damage + road/rail/port disruption + pipe/cable breaks
→ water and communications outage
→ delayed rescue and uncontrolled fire following earthquake
→ hospital and shelter stress
→ large displacement + prolonged utility repair
```

### Initial planning bands

| Variable | Initial band | Evidence class |
|---|---:|---|
| Potable-water outage population | 3.0–4.0 million | M |
| Displaced population requiring some support | 0.5–1.0 million | M plus uncertainty band |
| Initial rescue and fire window | 0–72 hours | S/A |
| Stabilization horizon | 30–180 days | A pending restoration curves |
| Access condition | Mixed intact, congested, bridge-constrained, debris-isolated, port-degraded | M |

### Critical force questions

- How much water can be distributed during the first 72 hours while pipe repair and source assessment proceed?
- Can independent fire-water systems reach hundreds of ignitions when hydrants and roads fail together?
- Which maritime routes remain usable if bridges and highways constrain cross-bay movement?
- How many acute-care beds remain usable after power, water, workforce, and structural losses?
- What shelter and interim-housing mix prevents 750,000 displaced people from becoming a months-long mass-care population?

## DRM-2: California atmospheric-river megaflood

### Evidence anchor

USGS's ARkStorm is a scientifically plausible California storm sequence. The scenario includes a Central Valley flood roughly 300 miles long and 20 or more miles wide in places, flooding and wind in major coastal regions, hundreds of landslides, and lifeline restoration lasting weeks or months. It estimates an inland and delta evacuation of approximately 1.5 million residents and about $725 billion in property and business-interruption losses in the report's historical dollars.[^arkstorm]

### Force-driving consequence chain

```text
weeks of extreme precipitation and wind
→ river, levee, drainage, coastal, and slope failures
→ evacuation + route loss + contaminated standing water
→ agricultural, industrial, housing, and utility disruption
→ long dewatering, debris, waste, and temporary infrastructure campaign
```

### Initial planning bands

| Variable | Initial band | Evidence class |
|---|---:|---|
| Supported population movement | 1.0–1.5 million | M |
| Flood extent | Multiregion; hundreds of miles | M |
| Heavy pumping and water-control horizon | Weeks to months | M/A |
| Public-works horizon | 6–24 months | A |
| Access condition | Flooded, landslide-isolated, bridge-constrained, coastal/riverine | M |

### Critical force questions

- What pump head, flow, debris tolerance, energy source, and discharge path are required for each basin rather than for “the flood” in aggregate?
- How does the force move people and cargo when north–south road and rail corridors are simultaneously interrupted?
- Where can contaminated sediment, municipal debris, agricultural waste, and hazardous material be processed safely?
- Which temporary levee, bridge, power, water, wastewater, and communications systems must remain for an entire wet season?

## DRM-3: sequential Gulf–Atlantic hurricanes

This synthetic mission uses official hurricane and 2017 response evidence but intentionally combines two major landfalls separated by 10–20 days. The first strikes a Gulf energy and port complex; the second affects a dense Atlantic coastal region while the first campaign is still in mass stabilization.

The case sizes forecast-driven staging, evacuation support, shallow- and deep-water rescue, port opening, fuel, temporary power, shelter, debris, and rotation. It also tests whether national leaders can protect the second region without prematurely stripping the first.

Key variables are landfall separation, population in outage areas, flooded-road duration, port throughput, utility mutual-aid draw, heat after landfall, and contractor overlap.

## DRM-4: Cascadia earthquake and tsunami

This no-notice regional mission assumes coastal communities isolated by tsunami and ground failure, damaged ports and airfields, mountain corridor loss, fuel interruption, and major urban demand inland. It is the primary requirement case for austere coastal entry, distributed reception, vertical lift, shallow-draft access, expeditionary communications, field care, and community-scale service packages.

The scenario must be modeled as many disconnected logistics islands, not one Pacific Northwest theater. A high-capacity system delivered to an intact inland hub does not satisfy an isolated coastal community.

## DRM-5: wildfire–heat–smoke complex

This mission assumes multiple geographic areas at high fire preparedness, prolonged extreme heat, dense smoke, grid curtailment, evacuation, and simultaneous demand for aircraft, crews, medical care, cooling, shelter, and public information.

It distinguishes four effects:

1. fire detection and initial attack;
2. extended attack and community protection;
3. population protection from heat and smoke outside the fire perimeter; and
4. post-fire access, debris, contamination, water, and housing.

The design must not size aircraft without turnaround bases, suppressant or water supply, airspace coordination, maintenance, crews, ground containment, and post-drop effectiveness.

## DRM-6: continental grid failure during temperature extreme

This systemic case cannot be solved by moving regional stocks from an unaffected area because most areas are affected or preserving their own reserves. It tests black-start support, islanded critical-load power, transformer and switchgear replacement, communications, water and wastewater, fuel distribution, building heat or cooling, medical-device dependence, and public-order interfaces without giving the Department a police mission.

The key modeling unit is a **critical-load island**: a connected cluster of water, health, shelter, communications, fuel, food, and public-service loads that can be safely energized and sustained. Household generators are treated as one layer, not the national solution.

## DRM-7: Caribbean territory compound catastrophe

This case assumes severe wind and flood damage, widespread grid and communications loss, impaired ports and airports, damaged health facilities, constrained local workforce, and a six-month external sustainment requirement. It prevents the force from using continental travel times, fuel access, receiving capacity, or private logistics as universal assumptions.

The scenario requires organic port and airfield opening, maritime distribution, water production, grid bridging, medical continuity, responder basing, and replacement crews. It also tests whether forward posture avoids the long delay created when every heavy effect must originate on the mainland.

## DRM-8: epidemic plus regional disasters

The epidemic case removes people rather than roads. It applies workforce absence and infection-control constraints across health, logistics, utilities, manufacturing, transportation, shelter, and the Force itself, then introduces a hurricane and wildfire campaign.

The design questions are replacement labor, protected clinical capacity, oxygen and pharmaceutical supply, modified shelter density, medical transport, supply-chain prioritization, remote operation, and the rate at which trained teams can be regenerated without spreading disease.

## DRM-9: drought and water emergency

This slow-onset case sizes a different institution: monitoring, allocation support, emergency interties, groundwater and surface-water treatment, wastewater reuse, mobile and semi-permanent production, long-distance conveyance, agricultural and livestock protection, community transition, and economic support.

It is the principal test for whether offshore or inland water-production concepts solve the binding problem. Treatment capacity has little value if intake, brine or residual disposal, energy, rights, pipelines, elevation head, storage, and local distribution make delivered water prohibitively slow or costly.

## DRM-10: allied coastal megacity earthquake

The global case assumes an invited U.S. response to a dense coastal city with damaged port, airport, hospitals, water, and power. Host institutions remain sovereign and capable but overwhelmed. The mission tests intercontinental movement, unfamiliar grid and pipe standards, language, customs, licensing, data sharing, urban density, security coordination, and transfer.

The Department's objective is not to reproduce an American city overseas. It is to provide modular services that connect to host systems, operate independently where required, strengthen local response, and leave maintainable capacity behind by agreement.

## Concurrency campaign: the 3C + 5M + 2G test

The first quantitative stress case combines:

- **C1:** DRM-6 grid failure at partial national scale;
- **C2:** DRM-3 first hurricane landfall;
- **C3:** DRM-4 Cascadia no-notice event;
- **M1–M5:** a wildfire complex, heat emergency, inland flood, major tornado sequence, and territorial drought-support mission;
- **G1:** DRM-10 allied earthquake response; and
- **G2:** a sustained regional flood and displacement mission abroad.

The case is intentionally severe. It asks which effects truly require a 20 percent residual reserve, which can be substituted, which must be forward positioned, and which industrial lines become the limiting national resource.

## What this pass establishes—and does not

The mission set establishes differentiated requirement environments and two externally modeled anchor cases. It does not yet claim authoritative national quantities for every service in every scenario. Those values belong in the editable demand model with low, base, and high cases.

The immediate next requirement is a common service-level library that turns each scenario's affected populations and facilities into comparable effect units.

[^haywired-water]: U.S. Geological Survey, [*A Simplified Method for Rapid Estimation of Emergency Water Supply Needs After Earthquakes*](https://www.usgs.gov/publications/a-simplified-method-rapid-estimation-emergency-water-supply-needs-after-earthquakes), September 25, 2021.
[^haywired-social]: U.S. Geological Survey, [*The HayWired Earthquake Scenario—Societal Consequences: Overview*](https://pubs.usgs.gov/sir/2017/5013/vol3/r/sir20175013r.pdf), version 1.1, 2021.
[^haywired-fire]: U.S. Geological Survey, [*The HayWired Earthquake Scenario—We Can Outsmart Disaster*](https://pubs.usgs.gov/fs/2018/3016/fs20183016_.pdf), 2018.
[^arkstorm]: U.S. Geological Survey, [*Overview of the ARkStorm Scenario*](https://pubs.usgs.gov/of/2010/1312/), Open-File Report 2010-1312, 2011.
