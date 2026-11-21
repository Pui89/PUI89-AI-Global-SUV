# AI-04 — Driver Behaviour Awareness Profile (SUV) v1.0

**Status:** Proposed product profile only; not implemented, integrated, tested, validated, or certified.

## Intended use
Provide advisory context for selected SUV driving and manoeuvring events. Candidate scenarios include lane-change context, following/closing traffic where validated relative-motion data exists, intersections, pedestrian/cyclist conflict cues, reversing and low-speed manoeuvring. This is not a driver-monitoring or automated-driving system.

## Candidate inputs
- AI-01 camera observations and AI-02/AI-03 outputs, subject to their own maturity and health status.
- Optional read-only vehicle signals (for example speed, turn indicator, steering angle or yaw rate) only where a documented, authorised interface exists and the signal is validated.
- No assumption that a candidate signal is installed or available on the concept vehicle.

## SUV-specific hazards
Evaluate lane changes with motorcycles or vehicles in adjacent lanes; closing traffic; intersections with crossing pedestrians/cyclists; reversing near people or obstacles; parking structures; poor lane markings; roadworks; night, glare, rain and camera obstruction. Separate low-speed and road-scene operating domains.

## Alerts and control boundary
Use clear, low-distraction advisory alerts after human-factors evaluation. Do not present a blind or unobserved zone as clear. No automatic steering, throttle, braking, gear selection or propulsion commands. Driver retains full control.

## Validation gates
Define each event and its required evidence; validate camera geometry and any read-only vehicle signals; test representative traffic, road markings, speeds, lighting, weather and occlusion; measure event-level precision/recall, false alerts, missed events, latency, stale data and uncertainty; inject signal loss and clock mismatch; test alert comprehension and distraction. Set thresholds only after hazard analysis. No numeric thresholds are approved in this profile.

## Privacy and non-claims
No identity, face, emotion, voice, medical, fatigue, intoxication or fitness-to-drive inference. No cabin monitoring by default. No functioning SUV, installed sensor set, ADAS integration, road trial, driver monitoring, autonomous driving, collision avoidance, certification or performance is claimed.
