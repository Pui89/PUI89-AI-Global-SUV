# PUI89 AI Robot Car — Automotive AI Compute & Sensor Architecture v1.0

**Status:** Proposed engineering architecture — not implemented, installed, vehicle-integrated, road-tested or validated.  
**Scope:** Software-first, driver-assistance and vehicle-context research for a global vehicle concept; body style, dimensions and platform not yet selected.  
**Safety boundary:** Human-driver-first, advisory-only. No commands to steering, throttle, braking, propulsion, high-voltage isolation or battery management.

## 1. Why this product-specific architecture exists

The Global vehicle is a distinct PUI89 product, not merely a generic voice-assistant configuration. Its engineering work must explicitly address automotive compute constraints, sensor placement and calibration, vehicle electrical conditions, read-only data interfaces, driver distraction, thermal management, vibration, privacy and regional regulatory differences.

The architecture reuses PUI89 Shared AI Core contracts and intelligence groups. It does not create a separate AI platform or duplicate the Shared AI Core.

## 2. Functional architecture

1. **Sensing and data intake:** removable forward/rear/side cameras, GNSS/IMU, optional radar or other sensors only after a documented value and sourcing review, and isolated read-only vehicle-context adapters.
2. **Input validation:** timestamp, units, provenance, calibration state, freshness, quality, sensor health and plausibility checks.
3. **Perception & Task Intelligence (PTI):** road-scene elements, road users, supported signs/markings, visibility and road-surface context. Outputs include confidence, uncertainty and explicit unknowns.
4. **Multimodal and WorldState fusion:** combine only authorised, time-aligned observations; preserve disagreement rather than forcing a false consensus.
5. **Reasoning & Decision Intelligence (RDI):** assess bounded risks, compare route/context alternatives, explain rationale, and abstain when evidence is insufficient.
6. **Interaction Intelligence:** concise voice and visual advisories, prioritised to minimise driver distraction; complex dialogue is unavailable while the vehicle is moving.
7. **Independent Safety & Action Gate:** enforce advisory-only output, human authority, rate limits, fault handling and safe degradation. The AI model itself is never the safety authority.
8. **Evidence and diagnostics:** record versioned test results, faults, provenance and uncertainty with privacy controls and retention limits.

## 3. Compute architecture — staged, not preselected

| Stage | Compute approach | Purpose | Gate |
|---|---|---|---|
| A — software baseline | Existing development computer; CPU-first | Contract tests, synthetic scenarios, offline dataset evaluation | Reproducible tests and resource measurements |
| B — removable research kit | Low-power edge computer selected after benchmarking | Limited sensor capture and advisory inference on a bench or controlled test setup | Verified power, thermal, vibration, storage and fail-safe behaviour |
| C — vehicle research integration | Automotive-suitable compute and protected power design | Supervised, removable, non-invasive read-only research | Qualified automotive/electrical review, warranty/legal review and closed-course approval |
| D — production assessment | Automotive-grade platform only if justified | Long-life, temperature, EMC, functional-safety and cybersecurity assessment | Independent qualification and applicable regulatory approval |

Do not select a processor, accelerator, NPU, ECU interface or compute vendor before defining workloads and measuring CPU/RAM, latency, sustained power, thermal behaviour, boot/recovery, storage endurance and total landed cost. Keep model selection hardware-neutral where practical. Do not require cloud inference, paid APIs or metered GPU services.

## 4. Sensor strategy

| Input | Intended research role | Key limitations and controls |
|---|---|---|
| Forward RGB camera | Road scene, lane/edge cues, vehicles and vulnerable road users | Lighting, glare, rain, occlusion, calibration and field of view |
| Rear/side RGB cameras | Adjacent and rear context | Blind spots remain; camera coverage is not a substitute for mirrors or driver observation |
| GNSS | Position and route context | Multipath, tunnels, urban canyon and stale fixes |
| IMU | Motion context and sensor alignment support | Bias, drift, mounting and vibration |
| Radar (optional) | Complementary range/relative-motion evidence | Only after non-Chinese-origin sourcing, interface, weather, calibration and validation review |
| Vehicle context (read-only) | Selected speed, status or diagnostic fields where lawfully accessible | Vehicle-specific semantics, units, update rates and access restrictions; unavailable data must remain unavailable |
| Microphone/audio (optional) | Limited voice interaction and selected sound-event cues | Privacy, cabin noise, false triggers and distraction; no emergency detection guarantee |

No sensor list is a claim that hardware has been purchased, mounted or integrated. Avoid duplicating sensors already present in a selected vehicle unless the additional sensor has a documented safety and engineering rationale.

## 5. Read-only vehicle data boundary

Use versioned, vehicle-specific adapters. Begin with synthetic fixtures and public documentation. A passive/read-only interface is not automatically safe: electrical isolation, bus loading, gateway policy, cybersecurity, warranty and legal access must be reviewed before connection.

- No CAN/OBD message transmission that changes vehicle state.
- No write access, actuator commands, ECU coding, diagnostic clearing or configuration changes.
- No steering, throttle, brake, gear, propulsion, high-voltage contactor or battery-management control.
- Never infer a missing signal from another signal without an explicit, validated rule.
- Store signal name, source, units, timestamp, freshness, vehicle/adapter compatibility and quality.
- Unsupported vehicle/model/year combinations must return UNSUPPORTED or UNAVAILABLE, not guessed values.

## 6. Product-specific intelligence allocation

| Intelligence group | vehicle-specific use | Boundary |
|---|---|---|
| Vision Intelligence | Road-scene and supported road-user perception | No collision-prevention guarantee |
| Audio Intelligence | Limited speech interface and selected cabin/external sound cues | No guaranteed siren, horn or emergency detection |
| Multimodal Intelligence | Time-aligned camera, optional radar, GNSS/IMU, weather and authorised vehicle context | Conflicts and missing data remain visible |
| Robotics Intelligence | Route/context planning and advisory optimisation | No vehicle motion planning or actuation |
| Action & Reaction Intelligence | Risk assessment, concise warnings, route avoidance and escalation | Bounded proposals only |
| Safety & Control Intelligence | Independent permission checks, fault response, alert limits and human-driver authority | No control path to vehicle actuators |

## 7. Interaction profile

The current README shortlist remains candidate-only:
- Whisper Small — limited speech-to-text requests; evaluate Thai/English cabin noise and recognition errors.
- Kokoro-82M — English spoken prompts only unless a separately reviewed Thai-capable candidate is established.
- Silero VAD — speech segmentation candidate; evaluate road/cabin noise and false activation.

All remain **PENDING_REVIEW**. No candidate is approved, installed or integrated. Do not enable complex dialogue while driving. Voice input is an information interface, never a vehicle-control interface. Thai TTS remains an open research gap.

## 8. Required engineering tests

Before any physical vehicle connection:
- Contract/schema tests and unsupported-signal handling.
- Synthetic stale, missing, contradictory, malformed and out-of-range signal tests.
- Camera quality, calibration drift, timestamp skew and sensor-dropout tests.
- CPU/RAM, latency, storage, sustained power and thermal measurements.
- Driver-distraction and alert-comprehension review.
- Fault injection, safe degradation, restart and recovery tests.
- Privacy, data minimisation, retention and cybersecurity review.
- Country-specific legal, warranty, electrical and automotive engineering review.

Before controlled vehicle research:
- Written test plan, risk assessment, qualified supervision and closed-course approval.
- Removable, non-invasive installation and electrical protection review.
- Verify no write/actuation path exists, including through dependencies and debug interfaces.
- Driver retains full responsibility and control; a human safety operator can stop the test.

## 9. Non-goals and prohibited claims

This architecture does not establish autonomous driving, ADAS certification, collision avoidance, validated perception, production automotive reliability, crashworthiness, flood-wading, fire protection, vehicle integration or global homologation. Unknown flood depth/current/passability means **unknown — do not enter**. The system must not claim that it can detect every hazard or prevent every collision.

## 10. Evidence and release gates

| Gate | Required evidence | Current status |
|---|---|---|
| G0 — architecture | Reviewed requirements, interfaces and safety boundaries | Proposed |
| G1 — software contracts | Reproducible synthetic tests and schema conformance | Not evidenced by this document |
| G2 — offline perception | Permission-cleared data, held-out metrics, false/missed detections and uncertainty | Not started / not evidenced |
| G3 — edge feasibility | Measured CPU/RAM/latency/power/thermal results on selected hardware | Not started |
| G4 — bench integration | Fault injection, electrical protection and recovery evidence | Not started |
| G5 — controlled vehicle research | Qualified review, closed-course plan and verified read-only isolation | Not started |
| G6 — production/regulatory | Independent automotive qualification and market-specific approvals | Not started |

**Release rule:** a document, diagram, model card or simulation is not proof of physical capability. Update each gate only with reproducible evidence and named review. No gate is passed by this architecture document.

## 11. Open-source-first sourcing requirements

For each candidate compute board, sensor, connector and power component, record exact manufacturer, brand, model/part number, manufacturing country and origin evidence, datasheet, supplier, dated price/currency, stock, lead time, warranty, shipping and compatibility. Prefer non-Chinese-origin candidates only where exact manufacturing origin is evidenced. Unknown origin is **UNVERIFIED**. No purchase, download or installation is authorised by this document.
