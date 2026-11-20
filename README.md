# PUI89 AI Global SUV

**A global-market SUV concept with original PUI89 vehicle intelligence architecture and driver-first, advisory-only AI.**

[English project page](https://pui89.github.io/ai-global-suv.html) · [ภาษาไทย](https://pui89.github.io/ai-global-suv-th.html) · [PUI89 portfolio](https://pui89.github.io/)

![PUI89 AI Global SUV concept](assets/images/pui89-ai-global-suv-concept.svg)

*Concept artwork only. It is not a production vehicle, selected platform or functioning prototype.*

## Product direction

PUI89 AI Global SUV is a software-first vehicle-intelligence concept intended for global-market requirements. The project aims to develop an original PUI89 design and engineering architecture informed by selected industry benchmarks:

- **Volvo — Safety:** layered occupant, road-user and system safety.
- **Mercedes-Benz — Luxury:** premium, calm, ergonomic cabin and user experience.
- **BMW — Engineering:** whole-vehicle integration and disciplined systems engineering.
- **Tesla and Rivian — Software-defined vehicle:** modular software lifecycle, integrated compute, updates and diagnostics.

These are learning benchmarks only. PUI89 will develop its own architecture, interfaces, design language and validation evidence; no proprietary technology or protected design is copied.


## Product identity and design specification

PUI89 AI Global SUV is a distinct medium-size, five-door SUV programme—not a generic AI car. Its exterior direction is an upright SUV body with a tall passenger cabin, rear cargo compartment, practical ride-height study, pronounced wheel-arch cladding and the PUI89 Deep Navy / Electric Cyan / Titanium Silver design language.

### Vehicle definition
- **Vehicle class:** medium-size global-market SUV concept.
- **Body direction:** five doors (four side doors and a rear liftgate), enclosed passenger cabin and dedicated rear cargo area.
- **Use context:** everyday and family travel, mixed urban/highway use, regional road conditions and serviceability; target markets and operating envelope require a formal requirements study.
- **Packaging:** seating layout, dimensions, wheelbase, track, curb mass, GVWR/GAWR, payload, cargo volume, towing, ground clearance, approach/departure angles and turning circle remain **TBD**. No numerical values are approved.

### Powertrain and energy
- Full Hybrid (HEV) is the first architecture proposed for evaluation.
- Petrol-only is a simplicity/cost benchmark; PHEV and BEV remain comparison cases.
- Engine, motor, transmission, battery chemistry/capacity, supplier, platform, fuel economy, range, emissions and performance are **not selected or established**.

### Product AI capabilities under research
- Road-scene and road-user awareness; obstacles, lane context, signs and visibility where supported by validated sensors.
- Weather, surface condition and water-on-road context, with conservative route-risk advice. Unknown water depth/current/passability must be treated as **unknown — do not enter**.
- Read-only vehicle-health and diagnostic observations through authorised, verified interfaces only.
- Explainable driver alerts, local event history, sensor-health reporting and Thai/English on-device interaction requirements.
- Software-first Shared AI Core, heterogeneous compute budgeting, local inference and fail-safe degradation. These are research/design goals, not claims of installed hardware or validated performance.

### Sensors, safety and data governance
- Candidate modalities may include RGB/depth cameras, radar, ultrasonic, GNSS, IMU, ambient/weather, thermal and supported vehicle telemetry. Exact sensor set, location, range and coverage remain TBD until vehicle-specific engineering and validation.
- Preserve sensor provenance, calibration state, timestamp, uncertainty, disagreement and failure status. Missing or stale evidence must not be presented as safe.
- Local-first processing/storage; no unapproved transfer of cabin images, voice, location or vehicle telemetry.
- Zero China supply-chain and technology dependence; verify origin, licence, security and supportability before adopting suppliers, components or software.
- The driver always controls steering, throttle, braking and propulsion. No autonomous control or actuator command path is in scope.

**Specification status:** the vehicle class, five-door body direction, design language and HEV-first evaluation order are design intentions. Physical dimensions, capacities, performance, installed hardware, production configuration and compliance remain open decisions or unvalidated.

## Master design and engineering document

**[PUI89 AI Global SUV — Master Design & Engineering Blueprint v1.0](docs/PUI89_AI_GLOBAL_SUV_MASTER_DESIGN_ENGINEERING_BLUEPRINT_V1.0.md)**

The master blueprint covers:
- Exterior identity and global SUV design requirements.
- Interior, luxury experience, HMI, ergonomics and privacy.
- Chassis, body structure and vehicle dynamics study areas.
- Powertrain and energy architecture comparison.
- Multimodal sensors, perception and sensor provenance registry.
- PUI89 AI Core and heterogeneous CPU/GPU/NPU/MCU compute orchestration.
- Safety architecture, cybersecurity and data sovereignty.
- Software-defined vehicle lifecycle and update governance.
- Global standards and regulatory investigation.
- Zero China Supply-Chain and Technology Dependence.
- Evidence gates, serviceability, lifecycle and open engineering decisions.

## Product-specific functions under research

- Road-scene and nearby road-user awareness using sensors selected and validated for the vehicle.
- Weather, visibility, road-surface and water-on-road context.
- Flood-risk and route-avoidance advice; unknown depth, current or passability must remain **unknown — do not enter**.
- Read-only vehicle-health observations where the vehicle provides a verified interface.
- Driver-facing alerts and evidence-based decision support.

## What is not established

- No production vehicle, donor platform, vehicle integration or road testing is established.
- No crashworthiness result, flood-wading capability, safety rating or regulatory certification is claimed.
- No autonomous steering, throttle, braking or propulsion control is in scope.
- No claim of safe water crossing, waterproofing, fire protection or validated predictive maintenance is made.
- AI advice does not replace the driver, vehicle safety systems or professional maintenance.

## Current development status

**Implemented — early software-only safety and contract foundations; master blueprint added as a proposed design baseline.** No vehicle integration or road validation is claimed.

**Next evidence gate:** create a traceable Vehicle Requirements & Decision Register covering user needs, operating conditions, packaging, safety, privacy, serviceability, target markets and supplier provenance before selecting a vehicle platform or integrating hardware.

## Existing project documentation

- [Automotive AI compute and sensor architecture](docs/SUV_AUTOMOTIVE_AI_COMPUTE_AND_SENSOR_ARCHITECTURE_V1.0.md)
- [AI architecture](docs/AI_ARCHITECTURE.md)
- [Project plan](docs/PROJECT_PLAN.md)
- [Fire and flood resilience requirements](docs/FIRE_FLOOD_RESILIENCE_REQUIREMENTS_V0.1.md)

## Shared PUI89 engineering

Cross-product architecture, evidence contracts, safety, privacy, security, recovery, device interaction and localization requirements are maintained in the [PUI89 Shared AI Core](https://github.com/Pui89/PUI89-Shared-AI-Core). Vehicle interfaces, road-risk thresholds and driver safety cases remain SUV-specific.

Current maturity labels follow the [PUI89 Portfolio Alignment Register](https://pui89.github.io/) and [Evidence-Based Development Maturity Standard](https://pui89.github.io/).

## Vehicle capabilities and functional capacity

**Scope boundary:** global SUV design intent with driver-first, advisory-only AI. Vehicle dimensions, seat count, mass, cargo volume, towing, ground clearance, platform, powertrain subtype and operational limits remain TBD pending qualified engineering.

### Perception and computing
- Candidate perception: road scene, lanes, vehicles, pedestrians, cyclists, animals, signs/signals, visibility, road surface and water-on-road context.
- Sensor placement, coverage, detection range, weather limits and performance must be validated on a selected vehicle.
- Define compute, memory, storage, thermal and latency budgets after workload and platform studies.
- Prefer local processing for safety-relevant perception; document model provenance, version, confidence and failure behaviour.

### Safety and authority
- AI is advisory only. The driver retains control of steering, throttle and braking.
- No autonomous steering, propulsion, throttle or braking commands.
- Flood, collision and road-hazard warnings are not guarantees of prevention or safe passage.
- If water depth, current or passability is unknown, advise **unknown — do not enter**.

**Capacity evidence status:** concept and software foundations only; numeric vehicle capacities and operational performance remain TBD / not validated.
