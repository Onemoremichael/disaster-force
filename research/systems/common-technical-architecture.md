# The common resilience technical architecture

## A constitution for machines, organizations and public authority

The Department of Resilience cannot become a peer instrument of national power by purchasing excellent systems that work only inside their own product lines. A water formation must accept power from a grid-bridge unit it has never met. A field hospital must reject an unsafe water connection even when its normal network is gone. An autonomous work machine must understand the same action boundary whether it arrives with a flood group, a fire group or an international partner. A replacement module made by an alternate supplier must carry enough evidence to be installed without importing the original vendor's engineers. And every high-consequence action must remain legible to the civil authority that owns the incident.

This is not mainly a connector problem. It is a constitutional problem.

A connector joins two pieces of equipment. A constitution specifies what each party may do, what it must disclose, what state is authoritative, how disagreement is handled, how safety is preserved when institutions or networks fail, and what evidence allows a claim to be trusted. The Department therefore needs a **Common Resilience Technical Architecture** (`CRTA`) that governs physical exchange, information, machine authority, configuration and proof across the force.

The accompanying [common technical architecture workbook](../../models/resilience-common-technical-architecture.xlsx) turns that proposition into an auditable first design. It allocates a $400 billion common layer within the selected $2 trillion technology case; defines ten common primitives and fifty boundary contracts; maps them across twenty-five representative system families; establishes four degraded modes and five machine-action authority classes; identifies thirty-two common-mode failures; and specifies twenty cross-system trials. The workbook is an architecture hypothesis, not an adopted standard, safety case, cost estimate or certification.

Its most important result is negative and therefore useful: all twenty-five representative systems remain blocked from rendering. None of the fifty interface contracts has representative-mission closure, and twenty-four of thirty-two screened common-mode failures exceed the current risk-priority threshold. A clean architecture drawing would conceal precisely the uncertainty this research program is meant to expose.

> The Department should be able to recompose a formation from independently designed systems, under damaged conditions, without surrendering civil authority, safety, traceability or the ability to operate manually.

## 1. Architecture is a public capability

Military acquisition provides a useful method precedent. The Department of Defense's Modular Open Systems Approach treats modular functions, consensus-based standards, published interfaces and appropriate technical data rights as means to sustain competition and make systems changeable across their life cycles.[^mosa] NASA systems engineering similarly treats interface definition, configuration management, verification and validation as continuing lifecycle disciplines rather than documentation performed after design.[^nasa-se]

The Department of Resilience needs those disciplines, but its operating problem is different in four consequential ways.

First, the Department exchanges consequential services with civilian infrastructure and people, not only data or payloads among government systems. Water quality, grid protection, clinical oxygen, flood discharge and bridge load capacity cross public boundaries. An interface failure may contaminate a hospital, energize a damaged feeder or flood another neighborhood.

Second, local, tribal, territorial and state authorities remain politically and legally real. A federal technical architecture must carry their decisions; it cannot manufacture jurisdiction by protocol. FEMA's National Incident Management System supplies a lower-bound doctrine of common terminology, resource typing, modular organization and unified coordination while preserving agency authority.[^nims] The future architecture must make that human authority executable without pretending that a machine token is legitimacy.

Third, the force must work after communications, positioning, cloud services, identity providers, utilities and supplier networks fail together. Connected performance is the easiest case. Isolated and manual-safe performance defines whether the system is actually a resilience system.

Fourth, scale magnifies correlation. Commonality reduces training, logistics and integration burden, but a common model, clock, credential service, connector, signing root, material process or software update can disable many formations at once. Modularity without diversity and containment can make the national force brittle.

The architecture is therefore a public capability in its own right. It requires laboratories, reference implementations, conformance services, fault-injection ranges, configuration authorities, trained interface engineers, public registries, alternate suppliers and operational exercises. A PDF standard without these institutions is an aspiration.

## 2. Design rules

The proposed architecture follows nine rules.

1. **Standardize the boundary, not the interior.** A vendor may use novel machinery, models and materials behind the boundary if the system exposes required state, obeys authority and safe-state rules, meets physical protection requirements and passes independent tests.
2. **Use profiles, not a universal plug.** Power, fluids, structures and data span irreducibly different scales and hazards. The common architecture defines bounded families and translation rules.
3. **Make units and uncertainty first-class.** A value without unit, calibration, time, location, provenance and uncertainty is not interoperable operational state.
4. **Carry authority with the action.** Every consequential machine instruction identifies issuer, jurisdiction, action class, geographic and physical limits, start, expiry and required approvals.
5. **Define failure behavior before nominal behavior earns credit.** Loss of link, time, position, identity, sensor confidence, software control or receiving infrastructure must lead to a predetermined bounded state.
6. **Separate compatibility from readiness.** A module may conform to a boundary and still fail mission physics, workforce, safety, environmental or formation tests.
7. **Bind evidence to configuration.** Test results apply to the article, software, model, supplier process and interface revision that were tested—not to a product name.
8. **Design for independent substitution.** Stable boundaries and qualified equivalence packets should allow new suppliers, local production and allied systems to compete without uncontrolled drift.
9. **Measure public effect.** Architecture evidence ends with delivered service, affected populations, environmental burden, workforce exposure and unintended consequences—not packet transfer or connector fit.

These rules prevent two opposite failures. A closed prime-contractor ecosystem produces dependency and expensive lock-in. An over-specified universal standard freezes the frontier and creates national common modes. The target is an open, versioned and tested set of contracts with deliberately diverse implementations.

## 3. Ten common technological primitives

Pass 16 identified ten technological primitives that recur across the Department's twelve mission-science directorates. This pass converts each primitive into five controlled interfaces.

| Primitive | Department-level boundary | Selected-case allocation |
|---|---|---:|
| Observation fabric | identity, time, location, measurement quality and provenance | $50B |
| Causal digital twin | component exchange, uncertainty, intervention, validation envelope and decision trace | $40B |
| Extreme-environment autonomy | task, authority, health, safe state and human takeover | $50B |
| Mobile power/fluid/thermal bus | media identity, connection, protection, metering and transfer | $55B |
| Advanced separations | feed, process module, product release, residuals and product switch | $30B |
| Rapid infrastructure fabrication | design package, site state, process qualification, acceptance and removal | $35B |
| Adaptive structures/materials | material state, health sensing, sacrificial behavior, repair and end of life | $30B |
| Distributed biomanufacturing | recipe, containment, in-process measurement, batch release and decontamination | $25B |
| Industrial digital thread | item identity, configuration, provenance, field history and substitution | $35B |
| Resilient communications/edge compute | identity, priority, disconnected reconciliation, update and audit | $50B |
| **Total common layer** | **ten primitives; fifty contracts** | **$400B** |

These dollars are a cross-classification within the strategic $2 trillion technology envelope, not another claim on top of it. The allocation says that one-fifth of the technology enterprise must create reusable national infrastructure rather than remain inside mission silos.

The same $400 billion is classified a second way: $180 billion for core science and components, $40 billion for reference implementations, $80 billion for test harnesses and proving infrastructure, $40 billion for standards and conformance, $40 billion for cyber/safety/public assurance, and $20 billion for open data, training and adoption. These classifications reconcile but are not additive.

The balance is intentional. Standards without working reference systems become ambiguous prose. Reference systems without adversarial conformance testing become favored products. Tests without independent evidence custody become demonstrations. Architecture without training and small-firm access becomes a cartel.

## 4. The fifty interface contracts

Each primitive receives five contracts because interoperability must cover more than message format.

The **observation fabric** distinguishes sensor and platform identity; event time from receipt time; horizontal and vertical reference systems; value, unit, method and calibration; and the transformation chain from raw observation to derived product. This guards against failures that look trivial in software but become enormous in the physical world. A vertical-datum mismatch can place a barrier, intake or evacuation route on the wrong side of a hydraulic threshold. Clock drift can corrupt the apparent order of a grid fault, fire drop or authorization.

The **causal digital-twin layer** specifies model inputs and outputs, units, state resolution, uncertainty, intervention representations, intended-use validation envelopes and decision trace. It does not bless one national model. It makes rival models comparable and makes it possible to refuse a model outside the conditions in which it has evidence. The NIST AI Risk Management Framework's govern–map–measure–manage structure is a useful lower-bound discipline for linking technical performance, context and accountable risk treatment; it does not by itself validate a disaster decision system.[^ai-rmf]

The **autonomy layer** separates mission intent from task execution. It transmits physical and jurisdictional bounds, exposes machine health and confidence, specifies deterministic behavior on link loss, and records operator qualification and takeover. A robot advertised as “Level 4 autonomous” communicates far less operational meaning than: authorized to excavate within this polygon, below this energy limit, until this time, under this supervisor, then stop and mechanically isolate if localization confidence falls below the bound.

The **utility-exchange layer** identifies the actual medium and its quality; defines keyed connection and isolation; coordinates electrical faults, pressure relief, grounding, bonding and permissives; meters service at the custody boundary; and governs black start, purge, drain-down and transfer. It joins water, power, fuels, thermal loops, medical gases and process streams as one architecture problem without pretending they share hardware.

The **separations layer** binds feed characterization to an approved process envelope, then holds product until an authorized quality-release decision. It also accounts for residual mass and lawful disposition. Product output is not public service if the concentrate, spent media, emissions or contaminated wash stream simply move the hazard elsewhere.

The **fabrication and adaptive-material layers** link digital design, site conditions, materials, process windows, proof and inspection to removal, repair and recertification. Fast infrastructure cannot waive state knowledge. It must know what was built, from which batch, by which process, on which foundation, under which load case, with what observed damage and remaining limit.

The **biomanufacturing layer** is deliberately stricter. Signed recipes, containment state, critical quality attributes, independent batch release and validated product switching remain separate functions. A field node that can change product rapidly but cannot prove decontamination or independent release is an experimental reactor, not medical supply.

The **industrial digital thread** keeps a persistent link from requirement and design through supplier, process, inspection, serialized item, field load, repair, software/model versions and retirement. NIST's digital-thread work provides an existing method base in product-definition standards, conformance, traceability and lifecycle exchange.[^digital-thread] The Department extends that chain into damaged, intermittently connected field operations and public-effect evidence.

Finally, the **communications and edge layer** supplies explicit human, device and service identity; traffic priority; store-forward-reconcile behavior; signed and reversible update; and tamper-evident audit with bounded emergency access. Zero-trust architecture contributes the principle that network location creates no implicit trust and that access decisions authenticate and authorize explicit subjects and resources.[^zero-trust] Disaster operations add a harder requirement: safety cannot depend on continuous access to the policy engine.

## 5. A minimum operational data contract

The Department should not impose one enormous ontology before it understands every mission. It should impose eight field groups without which operational state cannot be safely interpreted.

| Field group | Minimum question answered |
|---|---|
| Identity | What exact person, organization, system, item or component is this? |
| Time | When did the event occur and arrive, according to which clock and uncertainty? |
| Location | In which coordinate and vertical datum, with what geometry and error? |
| Measurement | What property, value, unit, method, calibration, quality and missing state? |
| Configuration | Which hardware, software, model, interface profile, deviation and maintenance state? |
| Authority | Who may cause which action, where, within what limits and until when? |
| Uncertainty | What distribution or interval applies, where is it calibrated and what tail warning exists? |
| Outcome | What effect was requested and delivered, to whom, with what environmental and workforce burden? |

Several distinctions are non-negotiable. Missing is not zero. Event time is not receipt time. Identity is not merely an IP address. A coordinate without a datum is incomplete. A model version is part of configuration. An expired authority cannot be silently renewed by connectivity loss. “Success” reported only by the producing system is not independent outcome evidence.

The contract must work locally. Every field has an offline rule, a validation rule, a privacy or security treatment, a retention policy and an explicit failure state. Precise person location may require aggressive minimization even while equipment configuration is kept for its full lifecycle. Public outcome reporting should be aggregated, while the evidence required to investigate a harmful action remains protected and reviewable.

## 6. Machine authority is an engineered boundary

The architecture defines five action classes.

| Class | Meaning | Default decision condition |
|---|---|---|
| `A0 Observe` | sensing without material physical action | pre-authorized mission and privacy boundary |
| `A1 Advise` | recommendation only | accountable human accepts consequential action |
| `A2 Reversible local` | bounded, low-consequence physical control | delegated local policy; supervisor for exceptions |
| `A3 High-energy infrastructure` | grid energization, pumping, heavy earthwork or fire attack | qualified human authorization plus independent inhibit |
| `A4 Life, rights or irreversible` | clinical, forced movement, occupied demolition or major release | accountable civil, clinical or legal authority makes final decision |

This taxonomy is based on consequence, reversibility and public authority—not on whether the underlying model is called artificial intelligence. A simple relay can be `A3`; a sophisticated planning model can remain `A1`.

At `A3`, the action message includes the named operation, geographic zone, physical envelope and expiry. Execution requires a qualified human, a technical safety channel and an independent physical inhibit. At `A4`, autonomy may gather evidence, simulate choices and execute bounded substeps, but it does not make the final life-, rights- or irreversible decision. Where an emergency stop is physically possible, it remains independent of the primary control path.

This architecture does not settle future law. It makes responsibility visible enough that lawmakers, courts, civil authorities, operators and affected communities can govern it. The crucial rule is that technical sophistication cannot launder an authority gap.

## 7. Degraded operation is the normal design case

Every primitive and every system must publish a tested service promise for four operating modes.

| Mode | Condition | Required posture |
|---|---|---|
| `D0 Connected` | diverse backhaul and online services available | full certified service with continuous replication |
| `D1 Intermittent` | variable connectivity and high latency | expiring queued orders, visible staleness and store-forward records |
| `D2 Isolated` | no external network | local trust domain, local authoritative state and 72 hours of mission-essential output |
| `D3 Manual safe` | digital control unavailable or distrusted | physical roles and controls, bounded output or safe shutdown |

The important transition is not simply down the table. Systems must rejoin safely. After isolation, two valid command histories, patient records, inventory states or maintenance states may conflict. Reconciliation preserves both records, applies declared authority and version rules, and requires human adjudication where the system cannot resolve the conflict safely. “Last write wins” is not an incident doctrine.

`D3` is equally concrete. A manual-safe claim requires local instruments, physical keys or roles, two-person controls where appropriate, accessible procedures, practiced operators and a controlled restart. A touchscreen with the network disconnected is not manual control. A system whose valves, breakers, brakes or stop functions cannot be directly reached has no `D3` mode.

NIST's cyber-physical and secure-systems engineering work supports treating physical, informational and trustworthiness concerns together across the lifecycle.[^cps][^secure-systems] The Department's doctrine adds a formation-level test: essential public service must survive the simultaneous loss or distrust of shared digital services.

## 8. Physical interoperability without false universality

The workbook establishes twelve **exploration bands**. They organize research, handling and adapter strategy; they are not voltage selections, connector standards, code approvals or design ratings.

### 8.1 Power

- `PWR-LV`: 12–60 VDC for sensor, control and small loads up to approximately 5 kW.
- `PWR-FAC`: familiar 120/208/240/480 VAC and a 380–800 VDC research envelope up to approximately 500 kW for facilities, treatment, shelters and workshops.
- `PWR-MV`: 4.16–34.5 kVAC and 0.5–25 MW for formation-scale islands, mobile substations and major utility modules.
- `PWR-HV`: 34.5–115+ kVAC and 25–300 MW for grid bridges; held pending evidence on what can safely remain mobile.

At low power, form factor and human handling may dominate. At medium and high voltage, fault duty, grounding, protection coordination, synchronization, visible isolation, utility authority and oversize transport dominate. The standard object is therefore a **profile**: electrical envelope, protection behavior, boundary measurement, handling class, safe state and test procedure. DOE's microgrid strategy reinforces the need for adaptive control, protection and self-healing among interconnected microgrids, but a Department formation also needs cold deployment into an unknown and possibly damaged topology.[^microgrid]

### 8.2 Fluids and thermal service

- `FLU-S`: 2.5–10 cm services for potable water, fuels, medical gases, samples and local thermal loops.
- `FLU-M`: 10–30 cm formation distribution for raw water, product, wastewater, fuel and thermal service.
- `FLU-L`: 30–100 cm regional trunks requiring transient, anchor, air/vacuum and rupture control.
- `FLU-XL`: roughly 1–2 m equivalent megaflow corridors for strategic drainage or water conveyance; held as a field-assembled system problem.

Diameter alone does not establish compatibility. Media identity, material, pressure, temperature, quality, cleanliness, transient behavior, decontamination, valve state and residual disposition matter. Physical keying should prevent plausible dangerous cross-connections. An improvised adapter may restore flow while destroying water quality or pressure safety; the architecture must make that trade impossible to hide.

### 8.3 Mechanical and structural exchange

The four mechanical bands cover person/pallet handling, road/container-compatible frames, heavy mission modules and field structures. ISO geometry remains a transportation opportunity, not a rule that every operating system fit inside a box. Modules may unfold or assemble. Their interface exposes mass, center of gravity, lift and restraint points, transport loads, operating envelope, foundation demand, proof state and visible damage.

At field-structure scale, the boundary also includes site survey, load path, inspection, exclusion zone, removal and restoration. A bridge, barrier or treatment hall is not conformant because a crane can lift it.

## 9. The correlated-risk problem

The architecture model registers thirty-two failure modes across the ten primitives. The current ordinal screen multiplies likelihood, consequence and detection difficulty on five-point scales. At a threshold of seventy-five, twenty-four modes are marked critical. These numbers are prioritization devices, not probabilities or expected losses.

The list reveals why common architecture requires more—not less—testing.

**Shared state failures** include spoofed or drifting clocks, vertical-datum mismatch, calibration drift and provenance loss. Each can silently corrupt multiple services.

**Shared reasoning failures** include correlated model bias, optimization that exploits a model error, unit mismatch and stale topology. A nationally shared model can make a confident national error.

**Shared autonomy failures** include fleet-wide perception error, incompatible lost-link policies, replayed authority and takeover that arrives after the physical consequence.

**Shared utility failures** include electrical protection mismatch, fluid cross-connection, pressure or thermal transient, and a defective connector lot. A standard connection concentrates exposure unless lot surveillance, alternate designs and sectional isolation are part of the standard.

**Shared production failures** include contaminant breakthrough, wrong fabrication version, hidden material damage, false structural-health state, erroneous batch release, incomplete decontamination, compromised authoritative baseline, unqualified supplier substitution and lost field history.

**Shared digital failures** include unavailable identity, a malicious or defective but correctly signed update, priority inversion under congestion and unsafe reconciliation after isolation.

Each entry therefore includes local detection and containment. The fleet should be partitionable by software and model lineage. Updates should move through canaries. Independent clocks, surveys and measurements should be available. Common modules should have alternate qualified implementations. High-energy systems should sectionalize physically. Safe degradation should sacrifice optimization before it sacrifices life safety.

Commonality earns acceptance only when the reduction in integration burden exceeds the new correlated-risk burden under representative fault injection.

## 10. Conformance is a chain of evidence

The architecture requires more than certification of a component on a bench. NIST's smart-grid framework is a useful method precedent: conceptual models and communication pathways lead to interoperability profiles, tests and certification rather than an assumption that a published standard produces an interoperable grid.[^smart-grid] NIST's emergency-response robot program likewise builds repeatable elemental tests into mission profiles and measures operator proficiency as well as machine performance.[^response-robots]

The Department's conformance chain has six levels.

1. **Schema and reference implementation:** the boundary can be instantiated and inspected.
2. **Conformance harness:** expected states, invalid states and failure behavior can be reproduced across laboratories.
3. **Representative boundary trial:** independently built systems exchange the intended service under relevant load and environment.
4. **Fault-injected mission thread:** failures are detected, contained and recovered without unacceptable public consequence.
5. **Formation trial:** recomposed systems deploy, operate, sustain and transfer under civil command.
6. **Operational replication:** different units, vendors, regions and crews reproduce the result.

The workbook sets level 3 as the minimum primitive evidence for the rendering screen, and it separately requires the platform to reach project `R3` and at least 80 percent weighted architecture closure. This is only a visualization gate, not field acceptance. Fielding requires the deeper formation and operational chain.

Twenty interoperability trials operationalize the doctrine. They include forecast-to-pump action under clock drift; water-to-hospital service with mis-keying and a quality-sensor fault; grid black start with protection mismatch; mixed-fleet night fire operations under GNSS error and link loss; live-flow breach arrest with shared perception fault and pressure surge; autonomous route opening amid public traffic; a rapid bridge built from a seeded wrong version; alternate-supplier cold activation; seventy-two-hour isolated communications; prospective model tournaments; manual-safe utility operation after a corrupt signed update; a damaged-port water–energy platform interface; maritime patient transfer; distributed bioproduct switching; structural-state-to-route-opening decisions; vulnerable-population utility federation; cross-region formation swaps; international civil handoff; fleet update rollback; and a ninety-day, three-theater complete campaign.

The trials intentionally cross program lines. A prime contractor cannot pass by bringing a complete proprietary stack. At least some trials must substitute modules, operators and suppliers without advance tuning. Thresholds must report tails and subgroup effects, not only averages. Seeded faults must be hidden from the operating team. Raw evidence remains with `RTEA`.

## 11. The digital thread is a safety structure

Every fielded item should remain connected to nine lifecycle states: measured need, requirement, design, supplier/process, verification, field issue, mission use, repair/change and retirement.

At each state, the Department defines an authoritative object, required links backward and forward, immutable evidence, editable state, signer, disconnected copy, reconciliation rule, release gate and consequence of failure. Corrections append; they do not silently overwrite. Effectivity is by serialized item or lot where necessary. A substitution is an evidence packet, not a purchasing note.

This thread prevents several common institutional errors:

- evidence from one prototype being attributed to a later design;
- a supplier process changing without changing the authoritative product state;
- field loads and environmental exposure disappearing before depot disposition;
- repaired equipment returning to service without a signed limit;
- software or model changes outrunning physical configuration;
- lessons being detached from the exact command, crew, environment and public outcome; and
- retired materials or biological hazards becoming orphaned.

The thread also creates industrial opportunity. A qualified small firm can sell a better module, inspection method, adapter, model or repair process against an open boundary. An alternate plant can prove equivalent output. Depots can diagnose equipment across vendors. International partners can own their operational records while participating through shared profiles. Exportability becomes compatible sovereignty, not permanent dependence on a U.S. cloud or prime contractor.

## 12. Institutions and decision rights

The common architecture needs its own durable institutions.

An **Architecture Board** owns interface allocation, version law, backward-compatibility policy and disputes among service directorates. It does not certify products.

The **Standards, Data and Public Assurance Office** maintains open specifications, reference vocabularies, accessibility and privacy requirements, public results and small-firm participation. It convenes affected infrastructure owners, workers and communities before a profile hardens.

The **National Resilience Laboratories** build competing reference implementations and metrology. A reference implementation demonstrates meaning; it is not the required product.

`RTEA` owns conformance harnesses, seeded faults, independent data, certificates, limitations and withdrawal. A certificate names the configuration, profile version, tested envelope and expiration or surveillance condition.

The **Resilience Manufacturing and Mobilization Administration** maintains product and supplier provenance, qualifies alternates, runs cold-start production tests and ensures that common standards do not silently collapse to one source.

Service Technology Commands integrate conformant systems into formations and doctrine. Civil authorities retain incident decisions. Technical safety authorities may stop an unsafe act but cannot appropriate the political decision to allocate services or compel people.

Change law matters. A new interface revision must state compatibility, adapter burden, security implications, fleet effect and retirement path. The Department funds adapters when continued compatibility is strategically valuable and retires an interface deliberately when it is not. Vendors do not gain a perpetual veto, and the government does not externalize every architecture change onto local partners.

## 13. Twenty-five-year transition

The architecture is built in seven overlapping phases.

**Years 1–2: constitute.** Establish the Board, the `RTEA` conformance directorate, the controlled registry and version/change law. Major new systems receive explicit interface allocations.

**Years 2–4: reference layer.** Produce independently implementable references for identity, time, minimum data, authority, disconnected exchange, power protection and fluid safety. Fund at least two implementations where correlation would be dangerous.

**Years 3–6: conformance services.** Deploy portable fixtures, hardware-in-the-loop systems, simulators, test datasets and public result registries. Demonstrate cross-laboratory repeatability and detection of seeded faults.

**Years 5–10: cross-hazard trials.** Execute trials 1–19 across utilities, hazard control, health, mobility, communications and industrial mobilization. Down-select profiles based on mission effect, safety and openness.

**Years 8–15: formation qualification.** Test cold deployment, module recomposition, manual-safe operation, maintenance, public effect and civil handoff. Low-rate production begins only behind representative formation evidence.

**Years 12–20: national scaling.** Prove cross-region swaps, independent suppliers, depot repair, multilingual operation and international handoff. Competition moves behind stable boundaries.

**Years 16–25: renewal.** Exercise backward compatibility, bounded break, adapter funding and retirement. Every rendering, specification and certificate remains tied to an actual configuration and interface revision.

## 14. What this architecture changes about the force

The `CRTA` changes formation design before it changes hardware.

A joint effect command can request **service**—potable water of a defined quality and flow, firm power with a defined fault envelope, clinical capacity with a defined acuity, safe passage at a defined load—without specifying the vendor stack that creates it. Units can be formed from different product lines because boundary evidence travels with the module.

The theater-opening force carries architecture scouts as well as engineers. They inventory local voltages, fault levels, water media, pressures, datums, route constraints, identity systems, laws and ownership. Their product is an interface map and safe connection plan.

Sustainment commands become configuration and evidence organizations. They distribute physical parts together with effectivity, repair method, inspection and updated limits. A warehouse cannot substitute a nominally similar seal, sensor, power electronic or bioprocess input without tracing the effect.

Training shifts from brand-specific operation toward boundary understanding, degraded modes, authority and fault containment. Vendor-specific skill remains, but the operator understands why a connection is refused, which local state is authoritative and how to place the system into `D3`.

Procurement becomes portfolio-compatible. Contracts buy technical data and test artifacts at the interface, permit independent conformance, preserve government emergency rights and support qualified third-party repair. They do not require disclosure of every proprietary interior mechanism.

The industrial base becomes broader. Major resilience primes may still emerge, but their power comes from integrating exceptional systems and sustaining worldwide service—not controlling the only interface. Specialized firms can build sensors, pumps, thermal systems, field structures, autonomy kernels, medical modules, adapters, metrology and conformance tools into a market with legible entry points.

## 15. Research conclusions and stop conditions

This pass reaches five conclusions.

First, common architecture is a major national investment category. In the selected case, $400 billion over twenty-five years is required to make the shared layer an engineered and tested public capability rather than procurement paperwork.

Second, the common layer is primarily semantic, authoritative and evidentiary. Physical standardization is valuable only inside coherent envelopes. One universal connector across scales and hazards is neither plausible nor safe.

Third, offline and manual-safe operation must be designed at inception. They cannot be added after a connected prototype succeeds.

Fourth, the greatest systemic danger is correlated failure. Diversity, partition, canary deployment, independent measurement, physical isolation and alternate implementations are architecture requirements.

Fifth, platform form remains downstream. The model maps 217 nonzero dependencies among twenty-five representative systems and ten primitives. Every system still has unclosed primitives. None has reached the combined project-physics and architecture threshold for rendering.

Pass 18 begins the first front with a facility-scale [National Resilience Proving Network](../proving/test-enterprise/national-proving-network.md), including experimental power, safety envelopes, environmental control, replication capacity and cost. The remaining front is platform-specific interface allocation: take `WRG-50`, `PRG-100`, `HCG-100`, the fire force and the water–energy platform through actual port maps, physical boundary sheets, fault trees and complete mission trials. Only then can exterior form begin to communicate engineering reality rather than substitute for it.

The stop decision is deliberate. The architecture has enough structure to govern the next engineering passes, but not enough evidence to close a single interface contract. Twenty-four critical common modes remain open. All renderings remain deferred.

---

## Notes

[^mosa]: U.S. Department of Defense, *Modular Open Systems Approach Reference Framework*, May 2020, https://ac.cto.mil/wp-content/uploads/2020/06/MOSA-Ref-Frame-May2020.pdf.
[^nasa-se]: National Aeronautics and Space Administration, *NASA Systems Engineering Handbook*, Rev. 2, 2016, https://www.nasa.gov/wp-content/uploads/2018/09/nasa_systems_engineering_handbook_0.pdf.
[^nims]: Federal Emergency Management Agency, *National Incident Management System*, 3rd ed., October 2017, https://training.fema.gov/EMIWeb/IS/IS700b/Handouts/National_Incident_Management%20System_Third%20Edition_October_2017.pdf.
[^ai-rmf]: National Institute of Standards and Technology, *Artificial Intelligence Risk Management Framework (AI RMF 1.0)*, January 2023, https://www.nist.gov/publications/artificial-intelligence-risk-management-framework-ai-rmf-10.
[^digital-thread]: National Institute of Standards and Technology, “Digital Thread for Manufacturing,” accessed September 4, 2026, https://www.nist.gov/programs-projects/digital-thread-manufacturing.
[^zero-trust]: National Institute of Standards and Technology, *Zero Trust Architecture*, SP 800-207, August 2020, https://csrc.nist.gov/pubs/sp/800/207/final.
[^cps]: National Institute of Standards and Technology, *Framework for Cyber-Physical Systems: Volume 2, Working Group Reports*, SP 1500-202, June 2017, https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.1500-202.pdf.
[^secure-systems]: National Institute of Standards and Technology, *Engineering Trustworthy Secure Systems*, SP 800-160 Vol. 1 Rev. 1, November 2022, https://csrc.nist.gov/pubs/sp/800/160/v1/r1/final.
[^microgrid]: U.S. Department of Energy, “Microgrid Program Strategy,” accessed September 4, 2026, https://www.energy.gov/oe/microgrid-program-strategy.
[^smart-grid]: National Institute of Standards and Technology, *NIST Framework and Roadmap for Smart Grid Interoperability Standards, Release 4.0*, SP 1108r4, February 2021, https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.1108r4.pdf.
[^response-robots]: National Institute of Standards and Technology, “Performance of Emergency Response Robots,” updated April 24, 2026, https://www.nist.gov/programs-projects/performance-emergency-response-robots.
