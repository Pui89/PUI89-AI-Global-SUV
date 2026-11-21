# AI-03 — Vulnerable Road User Protection Profile (SUV) v1.0

**Status:** Proposed product profile only; not implemented, integrated, tested, validated, or certified.

## Intended use
Advisory awareness for pedestrians, cyclists and other supported vulnerable road users around a future PUI89 AI Global SUV concept. Evaluate low-speed manoeuvring/parking and forward road-scene contexts as separate operating domains. Exact domains, camera coverage, mounting, and operating limits are TBD.

## Sensor and coverage assumptions
- Candidate input: approved RGB camera streams defined by the AI-01 SUV sensor profile. Additional sensing is not assumed.
- Do not claim complete 360-degree coverage. Blind zones, body occlusion, camera seams, near-field gaps and unavailable views must be mapped and disclosed.
- Optional radar or other sensor corroboration requires a separate interface, provenance review, calibration and validation; it is not part of this specification by default.

## SUV-specific hazards to evaluate
Pedestrians emerging from between parked vehicles; people behind or beside the SUV during low-speed manoeuvres; children or shorter pedestrians partly hidden by vehicle bodywork; cyclists approaching from the rear or sides; crossing paths at junctions; reversing scenes; crowded kerbs; loading areas; poor lighting, glare, rain, spray and dirty/obstructed lenses.

## Alert and driver interaction
Provide clear, prioritised visual and/or audible advisory alerts only after human-factors assessment. Avoid persistent nuisance alerts and avoid presenting an unobserved area as clear. Driver remains fully responsible and controls steering, throttle, braking and vehicle movement.

## SUV validation gates
Test each camera and combined view independently; measure blind zones and end-to-end latency; include stationary and moving VRUs, partial occlusion, multiple subjects, varied body sizes/clothing/mobility aids, day/night and adverse weather. Report per-class precision/recall/F1, false negatives, false alerts, track stability, calibration, stale-frame behaviour and sensor-fault response. Separate low-speed and road-scene results. No numeric pass threshold is approved yet; establish thresholds through hazard analysis before testing.

## Not claimed
No functioning SUV, installed camera system, production ADAS, automatic emergency braking, collision avoidance, 360-degree coverage, validated detection range, road testing, regulatory approval or certification is claimed.
