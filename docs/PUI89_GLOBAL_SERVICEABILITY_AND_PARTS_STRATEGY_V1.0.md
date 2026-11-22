# PUI89 AI Global SUV — Luxury, Serviceability & Global Parts Strategy

**Document ID:** PUI89-SUV-SERVICEABILITY-PARTS-STRATEGY  
**Version:** 1.0  
**Status:** Proposed engineering requirements — not a production specification, approved BOM, supplier nomination or validated service procedure.  
**Applies to:** PUI89 AI Global SUV — World Climate & All-Road Edition

## 1. Purpose and product direction

The SUV is intended to deliver a premium five-seat ownership experience while remaining practical to inspect, diagnose, maintain and repair across international markets.

Approved project direction:
- Five-seat Luxury First-Class SUV.
- 2.5L Hybrid (HEV) as the first powertrain architecture to evaluate.
- FWD / e-AWD architecture study.
- Payload target: 500 kg.
- GVWR target: 2,700 kg, subject to vehicle mass, axle-load, tyre, brake and structural validation.
- Operating-climate design target: -40°C to +50°C.
- Extended engineering challenge: -50°C to +60°C.
- Global serviceability, repairability and export-oriented design.
- AI is advisory; safety-critical vehicle controls remain independently protected.

All values are design targets, not validated vehicle capabilities. Exact engine, transmission, motor, battery, dimensions, component models, suppliers and part numbers remain unselected.

## 2. Luxury must be measurable

Luxury is not limited to styling or a large screen. The engineering programme should translate the first-class experience into verifiable requirements:

### 2.1 Cabin comfort and usability
- Supportive seats with a wide adjustment range and validated posture/pressure distribution for a broad range of occupant sizes.
- Clear ingress/egress, rear-seat access, useful storage and practical luggage loading.
- Low cabin noise, vibration and harshness (NVH), including tyre, wind, powertrain and road-surface noise.
- Effective heating, cooling, ventilation, demisting and defrosting across target climates.
- Intuitive controls, legible displays, restrained alerts and physical access to essential driving and climate functions where human-factors review requires it.
- Durable, cleanable, UV-, heat-, humidity- and abrasion-resistant cabin materials.
- Consistent fit, finish, tactile quality, lighting and acoustic comfort without decorative features that reduce visibility or service access.

### 2.2 Exterior and all-road quality
- Premium, original PUI89 proportions and restrained detailing using the current brand direction: Deep Navy, Sapphire Blue and Platinum Titanium.
- Functional body protection and replaceable trim where impact and repair studies justify it.
- Corrosion protection for body cavities, fasteners, underbody, connectors and dissimilar-material interfaces.
- Serviceable lighting, wipers, glass, sensors and bumper-area components.
- Ground clearance, approach/departure geometry, wheel/tyre size and underbody protection must be selected from validated use cases, not appearance alone.

### 2.3 Durability and ownership experience
- Design for long service life under heat, cold, dust, salt, humidity, vibration and rough-road exposure.
- Make wear items and common failure-prone service items replaceable without unnecessary removal of major assemblies.
- Define warranty, maintenance intervals and durability claims only after engineering validation and market-specific review.
- Provide a clear owner schedule and technician service information in destination-market languages.

## 3. Easy inspection, diagnosis and repair

The vehicle package should be reviewed by service technicians during design, not only after styling and CAD are frozen.

### 3.1 Routine access
Provide safe, clearly labelled access to:
- Engine oil, coolant and other approved fluid inspection/fill/drain points.
- Engine and cabin air filters.
- Fuses, relays and low-voltage battery service points.
- Diagnostic connector and approved diagnostic access.
- Wiper service position, lamps and commonly replaced exterior items.
- Hybrid-system inspection points that are explicitly designated for qualified high-voltage technicians.

Routine service should not require removal of the engine, transmission, dashboard or large unrelated assemblies unless a documented safety or packaging reason exists.

### 3.2 Modular repair
- Prefer replaceable subassemblies for pumps, fans, valves, sensors, harness sections, brackets, lamps, switches and control modules where safe and economically sensible.
- Design connectors, mounts, fasteners and access panels to reduce damage during removal and installation.
- Keep replaceable exterior protection, wheel-arch liners and underbody shields separate from major structural members where crashworthiness permits.
- Provide repair options for trim, upholstery, switches and cabin modules rather than forcing full interior-assembly replacement.
- For the high-voltage battery, inverter and e-motor, define safe isolation, inspection, lifting, removal and replacement procedures. Module-level repair is permitted only if the selected battery design, manufacturer procedure, law and qualified technician competence explicitly allow it.
- Never instruct owners or unqualified technicians to open or repair high-voltage components.

### 3.3 Diagnostic design
- Provide a standardised, documented diagnostic strategy with clear DTC definitions, freeze-frame/context data, system status, software/hardware identity and fault severity.
- Use read-only vehicle-data interfaces for PUI89 AI unless a separately approved safety case authorises otherwise.
- Keep conventional vehicle diagnostics and safety systems independent of the PUI89 AI runtime.
- Distinguish confirmed faults, suspected faults, degraded operation and unknown data; never convert missing data into a healthy status.
- Provide offline-capable basic diagnostics and service documentation where technically and legally appropriate.
- Protect vehicle networks with a secure gateway, authenticated service access, least privilege, audit records and controlled software updates.

## 4. Global parts availability and supplier strategy

### 4.1 Preferred sourcing regions

Evaluate qualified suppliers and service ecosystems in:
- Thailand and ASEAN;
- Japan;
- South Korea;
- Europe;
- United States.

These are target sourcing regions, not pre-approved suppliers or a guarantee that a specific component is available. Supplier selection requires evidence for country of origin, manufacturing site, ownership and sub-tier provenance, quality system, technical support, warranty, cybersecurity where relevant, lifecycle status and replacement supply.

The programme retains the user's zero-China-dependence requirement: do not select China-origin components, software, models or critical supply-chain dependencies. Verify provenance at the relevant component and sub-tier level; do not infer origin from a brand headquarters or distributor location.

### 4.2 Commonality and second-source strategy
- Prefer established automotive component families with documented specifications, mature service networks and long-term production support.
- Use industry-standard dimensions, connectors, fasteners, fluids and diagnostic protocols where they meet safety and performance requirements.
- Avoid unique one-off components without a clear engineering benefit.
- Identify a qualified second source for critical service parts where technically feasible.
- Define approved equivalents by engineering specification and validation, never by visual similarity alone.
- Maintain a regional availability and lead-time register for critical parts.
- Define end-of-life notification, last-time-buy review, repair alternatives and supersession rules.
- Do not allow a substitute part to change safety, thermal, EMC, sealing, crash or durability characteristics without revalidation.

### 4.3 Parts priority groups

| Priority | Component families | Sourcing/maintenance intent |
|---|---|---|
| A — Routine service | Filters, wiper blades, brake pads, 12V battery, approved fluids, tyres, bulbs where replaceable | Widely supported service items; documented fitment and regional supply |
| B — Wear and repair | Bearings, bushings, suspension links, dampers, hoses, belts, seals, wheel-speed sensors, lamps, mirrors, body clips | Replaceable assemblies; validated interchangeability and repair procedures |
| C — Powertrain/HEV | Engine service parts, pumps, cooling fans, inverter cooling components, e-motor and transmission service assemblies | Select suppliers with trained service networks and high-voltage safety procedures |
| D — Electronics/AI | Cameras, radar, GNSS, IMU, ECUs, gateways, displays, harnesses and compute modules | Long-term software support, provenance, calibration, secure diagnostics and replaceable modules |
| E — Structural/safety | Crash structures, restraints, airbags, steering, braking and high-voltage protection parts | Controlled configuration, traceability and approved repair/replacement only |

## 5. Part-number and configuration control

Do not publish invented or supplier-specific part numbers before components are selected.

Proposed internal identifier pattern (not an assigned production part number):
`P89-SUV-[SYSTEM]-[ITEM]-[REV]`

Each approved component record should contain:
- PUI89 internal item ID and revision;
- manufacturer and exact manufacturer part number;
- manufacturer and manufacturing country/site;
- country-of-origin evidence and critical sub-tier provenance;
- specification, drawing and interface revision;
- approved vehicle configuration and fitment position;
- safety/quality classification;
- service interval or condition-based replacement rule, where applicable;
- diagnostic/calibration/software dependencies;
- approved alternate and interchangeability evidence;
- supplier lifecycle, warranty and regional availability;
- inspection, installation, torque and post-repair verification instructions.

A PUI89 internal identifier must never be mistaken for an actual manufacturer part number.

## 6. Service documentation and technician experience

Provide a controlled service package for each released configuration:
- Owner's manual and quick-reference maintenance schedule.
- Workshop service manual with safe work steps and required skill level.
- Electrical wiring diagrams and connector/pinout references.
- Diagnostic trouble-code catalogue and fault-isolation flowcharts.
- Removal/installation instructions, special-tool list and verified torque specifications.
- Calibration and relearn procedures after replacement.
- High-voltage isolation, PPE, rescue and emergency-response procedures for trained personnel.
- Repair limits, one-time-use fasteners, fluid specifications and disposal/recycling guidance.
- Revision history, service bulletins, approved substitutions and technical-query process.
- Thai and English at minimum; destination-market languages as required.

No torque value, service interval, fluid specification or high-voltage procedure may be invented. Publish only values verified against the released component and vehicle configuration.

## 7. Maintainability and repairability verification

Create measurable serviceability tests before design freeze:

| Requirement | Verification method | Acceptance evidence |
|---|---|---|
| Routine inspection access | Timed task with representative technicians | Recorded access time, tools, steps and any obstruction |
| Filter/fluid service | Repeatable workshop task | No unintended removal/damage; correct refill and leak check |
| Component replacement | Remove/install selected service modules | Approved procedure, time, tool list and post-repair function check |
| Diagnostic clarity | Inject controlled faults in a test setup | Correct DTC, severity, context and recovery guidance |
| Parts interchangeability | Fit and validate approved alternate | Fit, function, safety and durability evidence |
| Corrosion/service exposure | Environmental and fastener testing | Inspection results and defined acceptance limits |
| Software/module replacement | Controlled replacement and configuration check | Correct identity, calibration, secure update and rollback evidence |
| Technician usability | Review with trained service personnel | Closed review findings and revised procedures |

Task-time targets must be set after baseline studies with qualified technicians. Do not claim "easy to repair" solely because a component is modular.

## 8. AI support for maintenance — advisory only

PUI89 AI may:
- Summarise authorised read-only diagnostic data.
- Explain DTCs using approved service information.
- Identify trends in temperature, vibration, voltage and operating history where valid sensors and data are available.
- Suggest inspection priorities and likely service items with uncertainty and evidence.
- Track component identity, service history and replacement/calibration status.
- Alert when data is missing, stale, conflicting or outside validated bounds.

PUI89 AI must not:
- Clear or suppress safety faults to make the vehicle appear healthy.
- Write to engine, transmission, brake, steering, airbag, battery-management or propulsion controllers.
- Command vehicle motion or bypass safety interlocks.
- Replace a qualified technician's inspection or an OEM-mandated service procedure.
- Present a prediction as a confirmed diagnosis.

## 9. Luxury and ownership quality gates

Before design freeze, review:
1. Cabin ergonomics, seating comfort, visibility, ingress/egress and accessibility.
2. NVH, HVAC, demisting, thermal comfort and climate-specific usability.
3. Material durability, repairability, cleanability, UV and chemical exposure.
4. Exterior fit/finish, corrosion, water management and replaceable protection.
5. Routine maintenance access and repair task studies.
6. Regional service coverage, parts lead time, warranty and technician training.
7. Total cost of ownership using transparent assumptions and market-specific evidence.
8. User experience when connectivity, sensors or optional AI features are unavailable.



## 10. Eight long-term engineering priorities and measurable governance

Apply the following eight principles as controlled lifecycle requirements:

1. **Easy to Inspect:** accessible, labelled routine inspection points and diagnostics; verify through timed technician task studies, tool/access records and no-damage inspection.
2. **Easy to Repair:** modular replacement and repairable subassemblies where safe; verify removal/install steps, required tools, repair limits, calibration and post-repair checks.
3. **Globally Serviceable:** assess qualified service capability and parts pathways in Thailand/ASEAN, Japan, South Korea, Europe and the US. Record actual country/site coverage, training, lead time and support evidence; target regions are not proof of availability.
4. **Parts Traceability:** retain manufacturer, exact manufacturer part number, manufacturing site, country of origin, sub-tier provenance, revision, approved fitment and validated alternatives. Unknown or conflicting provenance is a stop condition.
5. **Long-Term Support:** control owner/workshop manuals, wiring and diagnostic data, technician training, warranty/recall handling, software support, end-of-life notices, supersession and last-time-buy decisions.
6. **Offline Reliability:** primary driver controls and required safety functions remain independent of app, phone, internet and cloud. Provide local status, essential warnings and an offline service-information path.
7. **AI Maintenance Intelligence:** advisory/read-only analysis only; preserve evidence, timestamps, uncertainty and fault severity. Never clear/suppress safety faults, write to safety-critical controllers, bypass interlocks or replace qualified inspection.
8. **Lifetime Reliability:** establish repeatable environmental, corrosion, thermal, vibration, fatigue, serviceability and post-repair tests; retain failures, corrective actions and field feedback against exact configuration.

For every priority, the requirements register must identify an owner, applicable configuration, verification method, test conditions, measurable acceptance criterion, evidence location, review date and approval authority. “Easy”, “global”, “long-term” and “lifetime” are not accepted as unmeasured marketing claims. No supplier coverage, repair-time target, maintenance interval, service life or availability statement is approved by this section alone.

## 11. Governance and evidence status

This document defines proposed engineering requirements. It does not establish:
- a selected engine, hybrid system, battery, supplier or vehicle platform;
- a production BOM, approved manufacturer part number or qualified alternate;
- actual parts availability or service coverage in any country;
- measured maintenance time, repair cost, reliability, durability or service interval;
- a physical prototype, vehicle integration, test result or regulatory approval.

All items remain Proposed until assigned an owner, configuration, verification method, acceptance criterion and traceable evidence. Hardware purchases, downloads, installations and supplier commitments require separate explicit approval.

**Engineering principle:** Premium to own. Practical to maintain. Repairable by design. Supported across markets. Proven by evidence.
