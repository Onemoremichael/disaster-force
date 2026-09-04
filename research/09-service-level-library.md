# Service-level library

## Purpose and caution

The service-level library gives every design reference mission a common set of effect units and phased planning bands. These are **force-design inputs**, not universal entitlements and not claims that one number is safe for every person, climate, facility, or duration.

Every value must be adjusted for age, health, disability, culture, climate, activity, infection control, building type, technology, and local standards. The library distinguishes published guidance from design-study assumptions.

## Summary library

| Service | Primary effect unit | Survival or immediate | Emergency | Stabilized | Transfer |
|---|---|---|---|---|---|
| Household water | Liters delivered per person per day | 3.8 L storage-planning floor; higher where heat or illness requires | 7.5–15 L/person/day planning band | 15–20+ L/person/day plus non-domestic demand | Reliable owner-operated service meeting applicable quality and pressure |
| Health-facility water | Liters per patient, bed, or intervention | Critical clinical process loads protected | 40–60 L/inpatient/day planning reference plus special procedures | Facility-specific metered requirement with redundancy | Compliant utility or maintainable facility system |
| Food | Kilocalories and medically appropriate meals delivered per person per day | Ready-to-eat survival feeding | Approximately 2,100 kcal/person/day population planning reference | Nutrition, choice, special diets, local supply and cooking restored | Household and commercial food access |
| Shelter | People safely sheltered; dormitory and total support area | Hazard refuge only | 40–60 ft² dormitory/person; up to 100 ft² for some access needs | Non-congregate or dignified longer-term living with privacy and services | Stable housing or voluntary return |
| Sanitation | Users per fixture and liters of waste safely handled | Contain excreta and medical waste | Initial planning reference near 1 toilet/20 users, sex/access adjusted | Reliable toilets, bathing, handwashing, collection and treatment | Owner-operated wastewater and solid-waste service |
| Power | Critical-load MW continuously served at quality | Life-safety loads | Tier 1 critical facilities and communications | Critical-load islands plus thermal safety and economic nodes | Stable utility service or owner-operated microgrid |
| Thermal safety | People-hours inside safe temperature and air-quality envelope | Immediate refuge for highest-risk people | Accessible cooling, heating, clean-air shelter | Building or district service sufficient for daily life | Normal building and utility operation |
| Health care | Staffed treatment or bed-days by acuity; completed patient pathway | Triage, hemorrhage control, airway, emergency medication | Emergency, surgical, critical, obstetric, pediatric, dialysis, behavioral and public-health capacity | Continuity, rehabilitation, chronic care, workforce rotation | Definitive local/regional care and patient return |
| Communications | Priority users or area served at availability, latency, and throughput | Command, warning, 911/dispatch | Responder and public access; family contact | Utility, health, commerce, benefits, education and government access | Carrier and public-network restoration |
| Mobility | People or tons delivered end-to-end per day; route capacity | Rescue and life-safety access | Medical, fuel, water, food and repair priority flow | Predictable two-way logistics and evacuation/return | Safe civil network at required capacity |
| Debris and public works | Cubic yards or tons processed to compliant destination per day | Emergency clearance and hazard removal | Critical routes and facilities | Segregated removal, reduction, recycling, disposal and repair | Locally managed recovery works |

## Water

### Household demand

CDC recommends household storage of at least one gallon—about 3.8 liters—per person per day for three days for drinking, cooking, brushing teeth, and other uses.[^cdc-water-lib] That is used here only as an immediate storage floor.

WHO's emergency technical guidance supports staged planning and identifies additional health, sanitation, and institutional needs. Its examples include 40–60 liters per inpatient per day, 100 liters per operating-theater or maternity intervention, and substantial toilet-cleaning and flushing demand.[^who-water-lib]

The model therefore uses:

- **survival sensitivity:** 3.8–7.5 L/person/day for a very short period;
- **emergency range:** 7.5–15 L/person/day;
- **stabilized household target:** 15–20+ L/person/day; and
- **separate additive loads:** health care, shelter operations, schools, food production, firefighting, industry, animals, leakage, flushing, and Force self-use.

Water demand is measured at the **point of use**. Treatment output is increased for plant self-use, storage, leakage, spillage, distribution loss, and reserve.

### Quality and access

Quantity does not substitute for safety. Each module reports source, treatment train, testing, residual protection, storage, distribution, maximum collection distance or delivery interval, and residual disposal. Potable, hygiene, clinical, firefighting, industrial, and flushing water are separate quality classes so scarce high-quality water is not needlessly used for every purpose.

## Food and essential nutrition

UNHCR's long-used population planning reference is approximately 2,100 kilocalories per person per day.[^unhcr-health] The Force model uses a 1,800–2,400 kcal sensitivity range before demographic, temperature, labor, pregnancy, infant feeding, clinical, religious, allergy, and cultural adjustments.

Capacity is reported as **complete person-days of appropriate food delivered and safely stored**, not meals prepared at a distant kitchen. The chain includes potable water, energy, cold storage, transport, serving, waste, and safe preparation.

Emergency feeding should transition toward household choice, local purchasing, and restored commercial supply as rapidly as markets and access permit. Long-term centralized feeding is a failure mode, not a measure of institutional importance.

## Shelter and housing

FEMA's 2025 short-term shelter typing uses an average of 40–60 square feet of dormitory space per resident and notes that some disability-related accommodations may require up to 100 square feet; activity and support areas are additional.[^fema-shelter]

The model separates:

- **hazard refuge:** hours, high density, life-safety only;
- **short-term shelter:** days, 40–60 ft² dormitory/person planning band plus support space;
- **access-accommodated shelter:** up to 100 ft² dormitory/person for affected residents where required, plus power and caregiver/service-animal needs;
- **infection-controlled shelter:** event-specific spacing, ventilation, isolation, and hygiene;
- **non-congregate lodging:** rooms or household units; and
- **interim housing:** private living, cooking, sanitation, climate control, accessibility, schooling, transport, and connection to community.

The effect unit is a **safe occupied person-night** at the applicable service level. An empty cot or nominal facility capacity does not count.

## Sanitation, hygiene, and waste

The initial planning reference of roughly one toilet per 20 users is an emergency starting point drawn from humanitarian guidance, not a complete code.[^unhcr-health] The model adjusts for sex, disability, children, distance, cleaning, lighting, security, infection control, cultural practice, and peak use.

Sanitation capacity includes:

- excreta containment and treatment;
- handwashing and bathing;
- menstrual hygiene;
- laundry;
- solid and food waste;
- medical and pharmaceutical waste;
- hazardous and contaminated waste; and
- sludge, wastewater, and treatment residuals.

The effect is measured at compliant containment, treatment, discharge, reuse, or disposal—not at fixture delivery.

## Power and thermal safety

Per-capita wattage is a poor primary standard because critical loads depend on climate, building efficiency, medical technology, water systems, and network structure. Power is modeled through a **critical-load registry**.

### Load tiers

| Tier | Loads | Required response |
|---|---|---|
| P0 | Immediate life safety: ICU and life-support equipment, emergency lighting, 911/dispatch, control systems, water disinfection | No-break or near-no-break continuity with tested redundancy |
| P1 | Hospitals, water and wastewater, shelters, communications, fuel, emergency services, refrigeration, essential government | Energize within mission-specific hours and sustain continuously |
| P2 | Grocery and pharmacy, dialysis and outpatient care, cooling/heating centers, schools, finance, selected housing and transit | Restore as part of stabilized life-support |
| P3 | Broader commercial, residential, industrial, and public services | Prioritized recovery and economic continuity |

Each load record includes real and reactive power, voltage, frequency, harmonics, starting current, uptime, black-start behavior, connection, protection, fuel or energy input, thermal rejection, and safe disconnection.

The effect is **net critical-load megawatt-hours delivered at required power quality**. Generator nameplate megawatts are never reported as delivered effect.

Thermal safety is modeled separately as people-hours inside a defined temperature and air-quality envelope. This exposes cases where a small amount of power concentrated in efficient cooling, heating, filtration, and transport protects more people than attempting immediate household restoration.

## Health and medical care

Medical demand is built as a pathway:

```text
case finding → triage → stabilization → transport → regulating → definitive care
→ diagnostics and support → discharge or rehabilitation → patient return
```

Capacity is measured by completed stages and **staffed bed-days by acuity**, not tents or beds. Required categories include emergency, medical-surgical, critical care, burn, pediatric, obstetric, behavioral health, dialysis, isolation, rehabilitation, pharmacy, blood, oxygen, laboratory, imaging, sterilization, mortuary, and public health.

For every clinical module, the model adds power, water, oxygen, staffing, pharmaceuticals, blood, sterile supply, food, sanitation, waste, communications, cybersecurity, and patient transport. A bed without its care system has zero usable capacity.

## Communications and public-service access

Communications effects are divided into priority tiers:

- **C0:** warning, command, distress, 911/dispatch, responder safety, and critical infrastructure control;
- **C1:** health care, logistics, utility restoration, public information, and family reunification;
- **C2:** benefits, payments, commerce, remote work, education, and general public access; and
- **C3:** normal consumer capacity.

Every module reports geographic coverage, user count, availability, latency, throughput, backhaul, local power, cybersecurity, interoperability, and terminal distribution. A satellite backhaul terminal at headquarters does not count as public communications restoration.

## Mobility, access, and logistics

Mobility is measured end to end:

\[
Q^{delivered} = \min(Q_{origin}, Q_{strategic}, Q_{reception}, Q_{onward}, Q_{last-mile}, Q_{recipient})
\]

Separate flows are modeled for people, ambulatory and non-ambulatory patients, refrigerated cargo, fuel, bulk water, hazardous material, oversized equipment, debris and waste, and returning evacuees.

The planning record includes route capacity, cycle time, loading and unloading, weather, crew duty limits, staging, storage, manifests, damaged-network reliability, and empty or waste backhaul. Tons crossing a state line are not the effect; the effect is the intended people or facility receiving usable cargo.

## Debris, access, and temporary public works

Debris capacity is divided into:

1. emergency clearance;
2. search-support removal;
3. characterization and segregation;
4. loading and hauling;
5. reduction, recycling, treatment, or decontamination;
6. final disposal; and
7. documentation and site restoration.

The system throughput is the minimum stage. Cubic yards moved to an unpermitted temporary pile may create access but do not count as completed removal.

Temporary bridges, roads, ports, water networks, power systems, clinics, schools, and housing are measured by the civil service they enable, their inspection and operating requirements, and their transfer condition.

## Service bundles

People experience bundles, not portfolios. The model defines three initial bundles:

### Survival bundle

Safe location, drinking water, emergency food, immediate medical access, warning/communications, sanitation containment, and protection from lethal heat, cold, fire, flood, contamination, or violence.

### Stabilization bundle

Sustainable water and sanitation, appropriate nutrition, accessible shelter or housing, critical power and thermal safety, communications and public-service access, continuing health care, mobility, waste removal, and a functioning civil interface.

### Transfer bundle

Responsible ownership, qualified operators, reliable inputs, finance, maintenance, regulatory compliance, data and documentation, spare parts, and a tested transition without renewed service collapse.

The project's primary outcome—time to stabilized life-support—is the time at which the defined target share of the affected population receives the stabilization bundle, not the time at which the first federal asset arrives.

## Model implementation rules

- Store every quantity as low, base, and high or as an explicit distribution.
- Separate affected, outage, unmet, reachable, and served populations.
- Add facility and responder demand rather than hiding it inside per-capita values.
- Preserve quality classes and do not sum unlike services.
- Track cumulative person-days of deficit as well as peak demand.
- Make access and distribution explicit constraints.
- Report gross production, self-consumption, loss, and net delivered effect.
- Prevent a transfer of demand between services from appearing as a reduction in total harm.
- Record the evidence class and source for every major input.
- Treat all values in this library as editable; the workbook is the scenario engine, not a frozen answer.

[^cdc-water-lib]: Centers for Disease Control and Prevention, [*How to Create an Emergency Water Supply*](https://www.cdc.gov/water-emergency/about/how-to-create-and-store-an-emergency-water-supply.html), June 27, 2025.
[^who-water-lib]: World Health Organization, [*How Much Water Is Needed in Emergencies*](https://www.who.int/docs/default-source/wash-documents/wash-in-emergencies/technical-notes-on-wash-in-emergencies/who-tn-09-how-much-water-is-needed.pdf), Technical Note 9, accessed September 4, 2026.
[^unhcr-health]: United Nations High Commissioner for Refugees, [*Refugee Health*](https://www.unhcr.org/uk/publications/refugee-health), 1995. Values are used as humanitarian planning references, not current U.S. regulatory standards.
[^fema-shelter]: Federal Emergency Management Agency, [*Resource Typing Definition for Mass Care Services: Short-Term Shelter*](https://rtlt.preptoolkit.fema.gov/Public/Resource/ViewFile/9-508-1197?a=False&p=2&q=mass+care&s=FemaId&type=Pdf), September 2025.
