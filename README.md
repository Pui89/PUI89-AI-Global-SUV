# PUI89 AI Global SUV

**A medium-size, five-door SUV concept with driver-first, advisory-only AI.**

[English project page](https://pui89.github.io/ai-global-suv.html) · [ภาษาไทย](https://pui89.github.io/ai-global-suv-th.html) · [PUI89 portfolio](https://pui89.github.io/)

![PUI89 AI Global SUV concept](assets/images/pui89-ai-global-suv-concept.svg)

*Concept artwork only. It is not a production vehicle, selected platform or functioning prototype.*

## What this product is

PUI89 AI Global SUV is a **software-first vehicle intelligence concept** for a medium-size, five-door SUV. Its purpose is to help drivers understand road, weather, route and selected vehicle-health information. The driver remains in control at all times.

**ผู้ใช้งาน:** ผู้ขับขี่ ครอบครัว ผู้ดูแลยานพาหนะ และผู้ให้บริการยานพาหนะ  
**ประโยชน์หลัก:** ช่วยสังเกตความเสี่ยงบนถนน สภาพอากาศ เส้นทาง และข้อมูลสุขภาพรถ พร้อมแจ้งเตือนเพื่อสนับสนุนการตัดสินใจของผู้ขับขี่

## Product-specific functions

- Road-scene and nearby road-user awareness using sensors selected and validated for the vehicle.
- Weather, visibility, road-surface and water-on-road context.
- Flood-risk and route-avoidance advice; unknown depth, current or passability must remain **unknown — do not enter**.
- Read-only vehicle-health observations where the vehicle provides a verified interface.
- Driver-facing alerts and evidence-based decision support.

**Powertrain direction:** HEV-first research, while keeping the AI architecture powertrain-neutral. No production vehicle, donor platform or drivetrain has been selected.

## What is not established

- No vehicle integration, road testing, crashworthiness result, flood-wading capability or regulatory certification is established.
- No autonomous steering, throttle, braking or propulsion control is in scope.
- No claim of safe water crossing, waterproofing, fire protection or validated predictive maintenance is made.
- AI advice does not replace the driver, vehicle safety systems or professional maintenance.

## Current development status

**Implemented — early software-only safety and contract foundations.** No vehicle integration or road validation is claimed.

**Next evidence gate:** define priority driver use cases, operating conditions, read-only data interfaces, hazard analysis and measurable scenario acceptance criteria before choosing a vehicle platform or integrating hardware.

## Product documentation

- [Master engineering specification](docs/MASTER_ENGINEERING_SPEC_V2.md)
- [Automotive AI compute and sensor architecture](docs/SUV_AUTOMOTIVE_AI_COMPUTE_AND_SENSOR_ARCHITECTURE_V1.0.md)
- [Fire and flood resilience requirements](docs/FIRE_FLOOD_RESILIENCE_REQUIREMENTS_V0.1.md)

## Shared PUI89 engineering

Cross-product architecture, evidence contracts, safety, privacy, security, recovery, device interaction and localization requirements are maintained in the [PUI89 Shared AI Core](https://github.com/Pui89/PUI89-Shared-AI-Core). Vehicle interfaces, road-risk thresholds and driver safety cases remain SUV-specific.

Current maturity labels follow the [PUI89 Portfolio Alignment Register](https://github.com/Pui89/Pui89.github.io/blob/main/docs/PUI89_PORTFOLIO_ALIGNMENT_REGISTER_2026-11-18.md) and [Evidence-Based Development Maturity Standard](https://github.com/Pui89/Pui89.github.io/blob/main/docs/PUI89_DEVELOPMENT_STAGE_STANDARD.md).

## Vehicle Capabilities & Functional Capacity

**Scope boundary:** PUI89 AI Global SUV is a medium-size, five-door SUV concept with driver-first, advisory-only AI. No production vehicle, donor platform, vehicle integration or road validation is established.

### 1. Physical capacity
- Vehicle class/form: medium-size, five-door SUV concept.
- Seating, occupant mass, cargo volume, gross vehicle mass, towing, ground clearance, dimensions and axle loads: **TBD** pending platform selection and applicable vehicle engineering.
- No passenger, cargo or towing rating is claimed.

### 2. Mobility capacity
- Intended vehicle use is on-road mobility; supported road, weather and environmental operating conditions must be defined for the selected platform.
- Define speed envelope, turning/parking constraints, tyre and braking interfaces, ground clearance and any water exposure limits from verified vehicle specifications.
- No autonomous driving, flood-wading depth or off-road capability is claimed.

### 3. Perception capacity
- Candidate perception: road scene, lanes, vehicles, pedestrians, cyclists, animals, signs/signals, visibility, road surface and water-on-road context.
- Assess flood-risk and route context; if water depth, current or passability is unknown, report **unknown — do not enter**.
- Sensor placement, coverage, detection range, weather limits and performance must be validated on the selected vehicle.
- No driver monitoring or identity inference is claimed unless separately specified, permissioned and validated.

### 4. Computing capacity
- Define automotive compute, memory, storage, thermal and latency budgets after sensor and vehicle-platform selection.
- Prefer local processing for safety-relevant perception; document model provenance, version, confidence and failure behaviour.
- Vehicle data interfaces should be read-only unless separately approved through a safety case.
- **Compute hardware and measured performance:** TBD.

### 5. Power capacity
- Powertrain research direction is HEV-first while keeping AI architecture powertrain-neutral; no drivetrain has been selected.
- Define AI-system power draw, vehicle electrical interface, standby load, thermal limits and fault isolation after platform selection.
- **Traction battery/fuel, AI power budget and runtime:** TBD.

### 6. Communication capacity
- Define in-vehicle network interfaces, local connectivity, GNSS/navigation data sources and approved update paths only after platform review.
- Local driver alerts must not depend on internet availability.
- Define data minimisation, consent, cybersecurity and loss-of-connectivity behaviour.
- **Protocols, coverage and range:** TBD.

### 7. Safety capacity
- AI is advisory only. The driver retains full control of steering, throttle and braking.
- No autonomous steering, propulsion, throttle or braking commands.
- Alerts must be prioritised, understandable and designed to minimise driver distraction; critical vehicle functions remain independent.
- Flood, collision and road-hazard warnings are not guarantees of prevention or safe passage.

### 8. Maintenance capacity
- Define read-only diagnostics, sensor cleaning/calibration, wiring inspection, software/model version records and service procedures with the selected vehicle platform.
- Predictive-maintenance outputs must identify the source evidence and must not replace professional inspection.
- **Maintenance intervals and supported vehicle diagnostics:** TBD.

### 9. Operating limits
- Concept only; no vehicle integration, road testing, crashworthiness result, flood-wading capability or regulatory certification is established.
- Vehicle capacity, sensor performance, compute, power and communication specifications remain TBD until a platform is selected and tested.
- No autonomous vehicle control or claim of safe water crossing is made.

**Capacity evidence status:** Vehicle form is a concept; all numeric vehicle capacities and operational performance remain TBD / not validated.
