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
