# New York `L0` street-topology audit

**Run:** `DF-NYC-L0-PR41-v2`

**Parent protocol:** `DF-NYC-HB-PR38-v1`

**Prior operator run:** `DF-NYC-L0-PR39-v1`

**Status:** topology prerequisite complete at operator level; formal `L0` remains open

**Decision:** retain the twelve provisional references and three rehearsal commitments; do not generate `A2` or `S3` outcomes

## Executive judgment

The New York replication no longer depends on census-tract polygons touching. This audit reconstructs the outcome-blind selection universe on the official New York City Department of City Planning `LION 26b` street file, using segment endpoints, tract faces and relative vertical node levels. It admits a tract-to-tract relationship only when an eligible constructed street segment separates the tracts or when eligible segments attributed to the tracts meet at the same `(NodeID, NodeLevel)` key.

The result is strong evidence about the stability of the geographic selection and deliberately weak evidence about route usability.

The primary screen reduces 243,237 LION records to 145,378 qualifying name records and then to 126,779 canonical topological edges after exact alternate-name duplicates are collapsed and 107 distinct topologies under reused segment identifiers are retained. Those edges contain 97,108 node-level keys and support 7,129 tract adjacencies. Of the 2,325 land tracts in the frozen city surface, 2,224 have positive population, positive residential units and at least one street-supported neighbor.

The corrected graph produces 847 unique 32,000–38,000-person candidate catchments. Relative to the polygon rehearsal, 831 candidates survive unchanged, thirteen disappear and sixteen appear. Two populated residential tracts that the polygon rule treated as isolated acquire a street-supported connection: one in the City Island area of the Bronx and one in the Rockaway/Broad Channel geography of Queens. Despite those changes, every one of the twelve disclosed reference compositions is unchanged. The three holdout commitments are also unchanged.

That stability is not an artifact of one finely tuned filter. A stricter screen that removes step streets and records marked by the Department of Education for exclusion from pupil walking routes, and a permissive screen that admits private streets, highways, tunnels, ramps and connector layers, produce the same 847 candidates, the same selection thresholds, the same twelve references and the same three holdouts. The primary selection is therefore insensitive to the declared classification alternatives at this scale.

This pass closes only one stop condition. The graph is a versioned representation of mapped topology, not a claim that a resident, mobility device, ambulance, bus or `NCAC` vehicle can traverse a path after a blackout. It does not observe sidewalks, curb ramps, slope, width, doors, fences, controlled access, construction, traffic, debris, signals, floodwater, heat exposure or incident authority. Formal `L0` remains blocked by independent reproduction, governed age and disability covariates, salted external holdout custody and registration of empty outcome tables.

## Why polygon contact was not enough

Polygon touching was useful for the first operator rehearsal because it exposed the selection procedure before either architecture generated a result. It was not the registered test.

Two tracts can touch along a shoreline, rail corridor, grade-separated facility, restricted parcel or geometric artifact without a usable local connection. Conversely, cartographic generalization can prevent polygons from touching where a bridge or causeway creates a real street relationship. A geometric neighbor rule also cannot distinguish an at-grade intersection from lines that cross at different elevations.

The causal question is narrower than “do these areas look contiguous?” and more demanding than “is a road nearby?” For catchment construction, the question is:

> Can the set be represented as one connected component through mapped, constructed, non-vehicle-only local street or path topology, without creating a connection where the official network places the segments at different relative levels?

That question is still not incident access. It is the minimum defensible topological prerequisite for selecting a metropolitan test geography before route-condition worlds are introduced.

## Governing records and release control

The audit uses three official record families.

The governing network is the [NYC DCP LION dataset](https://data.cityofnewyork.us/City-Government/LION/2v4z-66xt). The frozen `nyclion_26b.zip` archive contains 243,237 line records, 139,674 node records and the associated alternate-name and node-street-name tables. Its SHA-256 digest is `14a2514303f0c53419cdc370bfd851db41dec038450b88b19d0897a35dad0660`.

The official [LION metadata](https://s-media.nyc.gov/agencies/dcp/assets/files/pdf/data-tools/bytes/lion_metadata.pdf) and [Record Processing Location documentation](https://s-media.nyc.gov/agencies/dcp/assets/files/pdf/data-tools/bytes/rpl_filelayout.pdf) define the semantics used here: `FeatureTyp`, `SegmentTyp`, `RB_Layer`, `NonPed`, `TrafDir`, roadway type, endpoint node IDs and relative node levels. The metadata endpoint had rolled to release `26C` by retrieval. This audit does not mix that newer geometry with the prior `26b` tract surface; it freezes the `26b` archive and uses the current documentation only to interpret stable field semantics.

The [NYC Office of Technology and Innovation Citywide Street Centerline](https://data.cityofnewyork.us/City-Government/Centerline/inkn-q76z) provides an independent official cross-check on roadway types, construction status, traffic direction and public-safety lineage. The city describes the centerline as a road-bed representation used in Geosupport, LION and 911 response. Its simplified public table lacks the endpoint identifiers required for the node-level audit, so it informs classification but does not govern adjacency.

The tract, population, PLUTO, building, elevator, heat-vulnerability and facility snapshots remain exactly those frozen in Pass 39. No architecture output, incident condition or modeled `A2`/`S3` advantage is introduced into the graph choice.

## Canonical graph construction

### Primary segment screen

The primary graph admits a LION record only when all of the following are true:

1. `Status = 2`, meaning constructed.
2. `FeatureTyp` is `0`, `A`, `W` or `C`: an ordinary non-vehicle-only street class, alley, addressable non-vehicular path or dedicated public-use street area.
3. `NonPed` is not `V`. Records marked vehicle-only are excluded. `D` records remain in the primary graph because the official definition says they are pedestrian accessible but excluded by the Department of Education from pupil walking routes.
4. `TrafDir` is present. Direction is not used to make the tract graph one-way; the field is used as evidence that the line participates in the mapped travel network.
5. roadway type is street, bridge, boardwalk, path/trail, step street, driveway or alley. Highways, tunnels, ramps, non-physical streets, U-turns and ferries are excluded.
6. `SegmentTyp` is `U`, `B` or `G`: undivided, both generic/roadbed or generic. Roadbed-only, connector, entrance/exit, faux, terminator and suppressed records are excluded to avoid counting divided-road drawing layers as extra local paths.
7. both endpoint node IDs and both endpoint node levels are present.

The row funnel is visible rather than buried:

| Stage | Records |
| --- | ---: |
| all `LION 26b` line records | 243,237 |
| constructed | 205,778 |
| public/addressable street feature class | 195,192 |
| not vehicle-only | 169,064 |
| traffic-direction code present | 169,061 |
| complete primary screen | 145,378 |
| canonical topological edges | 126,779 |

LION repeats some segment identifiers across street-name records. The audit does not assume that every repeated identifier is redundant. It collapses a row only when segment ID, endpoint node-level keys and both tract faces are identical. It retains 107 additional topologies under reused IDs and records the condition. This prevents an alternate name from creating a fictitious second edge while avoiding an arbitrary first-row rule when topology differs.

### Vertical topology

The graph key is the ordered pair `(NodeID, NodeLevel)`.

`NodeLevel` is relative, not an elevation. The letters generally place a record below, at or above the main level at the same node, but they do not describe terrain and cannot be compared across different node IDs. The audit therefore uses level only to prevent two lines attached to the same node identifier at different relative levels from becoming an intersection. It does not infer bridge clearance, grade, stair burden or accessible slope.

### Census-tract attribution

LION stores left and right 2020 census-tract components. The audit constructs an eleven-digit Census GEOID as:

```text
36 + county FIPS implied by borough + four-digit tract main + two-digit suffix
```

Blank suffixes become `00`. A derived GEOID is accepted only when it exists in the frozen 2,325-tract surface. This prevents malformed or out-of-scope face codes from entering the graph.

### Street-supported adjacency

For each eligible edge, the audit assigns its valid left and right tracts to both endpoint node-level keys. A tract pair is adjacent if either:

- the same eligible edge has two different valid tract faces; or
- eligible edges attributed to the two tracts are incident to the same `(NodeID, NodeLevel)` key.

The second rule is necessary because an intersection may connect tracts without one segment running exactly along their shared boundary. It also creates a clear audit trail: every pair has a count of segment-face witnesses and node-incidence witnesses. In the primary graph, 5,593 of 7,129 pairs have both forms of support; 1,536 are supported by node incidence alone.

Witness counts are not independent alternatives. Ten name or segment records at one intersection do not create ten operational routes. They show only that the official representation supplies repeated topological evidence for the pair.

## Candidate and selection procedure

All rules downstream of adjacency remain unchanged from Pass 39.

Each eligible tract becomes one seed. The candidate begins with that seed and repeatedly adds the street-adjacent frontier tract whose projected centroid is nearest to the current population-weighted centroid of the selected set. Coordinates are transformed to New York Long Island State Plane feet (`EPSG:2263`). A distance tie breaks by ascending GEOID. Growth stops when population first reaches 32,000; a group above 38,000 is rejected. Identical ascending GEOID sets are deduplicated.

The candidate ID and ordering hash remain SHA-256 of the canonical ascending pipe-delimited GEOID set followed by `|DF-NYC-HB-PR38-v1`. The three archetype thresholds are recomputed on the corrected candidate universe because percentile thresholds are properties of that universe. The disjointness, processing order, borough cap and second-slot borough-diversity rules are unchanged.

This separation is important. The topology correction is permitted because no outcome exists and because the registered requirement already demanded a street component. It does not authorize other convenient changes to selection rules.

## Results

### Graph sensitivity

| Screen | Canonical edges | Node-level keys | Tract pairs | Eligible residential tracts | Candidates | `V1` pool | `V2` pool | `V3` pool |
| --- | ---: | ---: | ---: | ---: | ---: | ---: | ---: | ---: |
| primary | 126,779 | 97,108 | 7,129 | 2,224 | 847 | 82 | 169 | 28 |
| strict mobility | 120,894 | 92,575 | 7,074 | 2,222 | 847 | 82 | 169 | 28 |
| permissive | 134,314 | 103,019 | 7,134 | 2,224 | 847 | 82 | 169 | 28 |

The strict sensitivity removes `NonPed=D` records and step streets. It is not labeled “accessible”: absence of those records does not prove curb, grade, width or device access. The permissive sensitivity admits private streets; highway, tunnel and ramp roadway types; and connector/entrance-exit segment layers. It is a bound on classification choice, not the preferred civil-access graph.

The three screens differ by 13,420 canonical edges and sixty tract pairs between their extremes. Yet candidate construction, thresholds, archetype pools and selected compositions are identical. At the 32,000–38,000-person aggregation scale, the selection is robust to these declared edge-class alternatives.

### Polygon-to-street reconciliation

| Reconciliation class | Candidates |
| --- | ---: |
| retained in both universes | 831 |
| added by street topology | 16 |
| removed from polygon topology | 13 |
| corrected street universe | 847 |

The small net change should not be misread as proof that polygon touching was acceptable. Candidate construction is a path-dependent growth algorithm. A single edge difference can change which tract is added next and therefore change the final canonical set even when most of the city graph is similar.

The direct tract-eligibility difference is interpretable. GEOID `36005051601` in Pelham Bay–Country Club–City Island had zero polygon neighbors and gains one node-incidence relation to `36005050400`. GEOID `36081107201` in Breezy Point–Belle Harbor–Rockaway Park–Broad Channel likewise had zero polygon neighbors and gains three node witnesses to `36081107202`. Causeways and island geography are exactly where a street graph should outperform polygon contact. Both relations are node-incidence-only, which is why independent reproduction and later person-specific route validation still matter.

### Reference stability

All twelve provisional reference catchments retain the same candidate ID and exact GEOID composition:

| Archetype | References retained exactly | Distinct reference tracts | Population range |
| --- | ---: | ---: | ---: |
| `V1` tower-intensive | 4 of 4 | 21 | 32,165–34,306 |
| `V2` mid-rise heat burden | 4 of 4 | 34 | 32,813–35,451 |
| `V3` campus/service friction | 4 of 4 | 32 | 34,486–37,606 |
| **total** | **12 of 12** | **87** | **414,234 combined** |

The governing thresholds move slightly because the universe changes from 844 to 847 candidates: mean-floor `V1` P80 rises from 8.519 to 8.586; device records per 1,000 P80 rises from 7.685 to 7.718; density P75 rises from 75,883 to 76,073 people per square mile; and campus-share P75 rises from 14.29 to 14.58 percent. None changes the selected set.

The three rehearsal holdout commitments are byte-for-byte unchanged:

| Holdout | Commitment |
| --- | --- |
| `NYC-V1-H01` | `2a5fbcafb3f8c6a3a673021cf7ac54c817131e9384d38c3886566bd118011d39` |
| `NYC-V2-H01` | `2f1b5528a53efb9288f3c9e70f3a3f592ef2f10bebf7f6366858f8fcf529ecc6` |
| `NYC-V3-H01` | `284f1a756375147329171dc38e34e45899f75cbf67492bf2e0c9fcc09b602315` |

That is commitment continuity, not secrecy. A public deterministic universe and unsalted hash remain reconstructable. The external-custody requirement does not close merely because the composition survived a topology correction.

## What the graph permits—and forbids—the study to say

The audit supports four bounded claims:

1. the candidate builder now uses an official, versioned street-node representation rather than polygon contact;
2. grade-separated records are not linked merely because they share a node identifier;
3. the twelve disclosed references are robust to the polygon-to-street correction and two declared street-class sensitivities; and
4. every primary tract adjacency can be traced to official segment-face or node-incidence witnesses.

It does not support these stronger claims:

- that any complete path is walkable, wheelchair accessible or vehicle-passable;
- that a mapped bridge, boardwalk, driveway, alley, step street or path will remain open;
- that a tract has sufficient entry capacity, redundancy or travel time;
- that a building entrance connects to the mapped centerline;
- that a route is public, authorized or safe for a specific responder or resident;
- that signals, lighting, transit, communications or curb operations will function;
- that post-event congestion, debris, heat, flooding, smoke or civil restrictions are tolerable; or
- that a selected catchment is representative of the city beyond the three declared mechanisms.

Those are `L1` design inputs and campaign-world variables, not facts that can be read out of a base map.

## Institutional implication

This audit reveals a small but important part of the mature Department of Resilience.

A force organized around public effect needs an independent **civil mission-graph service**: a standing capability that freezes authoritative network releases, reconciles street, building, utility, facility and household edges, preserves privacy and authority, works offline, carries uncertainty explicitly and can be reproduced by a separate team. Its job is not to make one perfect national map. Its job is to distinguish:

- mapped topology from present condition;
- public geometry from lawful access;
- physical access from accessible passage;
- a possible route from a capacity-bearing route;
- an operator assumption from an independently warranted fact; and
- selection data from architecture outcomes.

Military force projection invests heavily in common operational pictures, terrain, targeting, logistics status and contested-network resilience because movement and effect depend on them. A coequal resilience force requires an analogous civil representation, constrained by rights and service obligations rather than targeting. The New York graph is a modest operator prototype of that national function.

## Remaining `L0` closure package

The topology requirement is now complete only at operator level. Formal closure still requires:

1. **Independent reproduction.** A separate implementation must rebuild the 126,779-edge primary graph, 7,129 tract pairs, 847 candidates, twelve references and three commitments from the frozen records. It must reconcile the 107 retained reused-ID topologies and every candidate-universe difference.
2. **Demographic completion.** Governed age, disability, medical-power and accessibility inputs must be acquired with explicit denominator, vintage, missingness and privacy rules. They may characterize selected catchments and synthetic households; they may not retroactively optimize the geography after outcomes.
3. **External holdout custody.** An independent custodian must control compositions and secret salts, publish salted commitments and define the dated unsealing rule. The existing commitments remain useful continuity records but are not secure holdouts.
4. **Empty-table registration.** The full 24,000-row architecture-world schema, missing-data rules, exclusion flags, failure adjudication and hypothesis fields must be frozen while all result columns are empty.
5. **Rights and accessibility review.** Disability-led and civil-rights reviewers must decide which paths, buildings, services and dispositions require direct field or administrative validation before any modeled service credit.

Until all five close, the campaign remains sealed. No `A2` or `S3` outcome may be computed, no `NCAC` gate advances and no rendering is authorized.

## Audit artifact

The companion [street-topology audit workbook](../../../models/nyc-l0-street-topology-audit.xlsx) preserves the source manifest, filter funnel, three graph summaries, all 2,325 tract degrees, all 7,129 primary adjacency pairs and their witnesses, the 860-row union of polygon and street candidate IDs, exact reference reconciliation, sensitivity thresholds, unchanged commitments and formula-backed quality checks.

The earlier [catchment rehearsal](new-york-l0-catchment-rehearsal.md) remains the historical operator build. Its polygon-based candidate counts are not silently rewritten; this paper is the registered correction.
