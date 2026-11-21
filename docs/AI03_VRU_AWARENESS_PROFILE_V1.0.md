# PUI89 AI-03 — Global SUV VRU Awareness Profile v1.0

**Status:** Proposed product profile; documentation only. No vehicle integration, sensor installation, model execution, road test or safety validation is claimed.

## Mission
Provide driver-facing awareness of pedestrians, children as pedestrians, cyclists and other supported vulnerable road users around the SUV. The system is advisory only; the driver retains steering, throttle, braking and propulsion authority.

## Operating contexts to specify
- Low-speed manoeuvring, parking, reversing and driveway/curbside movement.
- Urban streets, intersections, crossings, school-zone contexts and mixed traffic.
- Higher-speed road scenes only after a separate sensor, latency, range and hazard case demonstrates suitability.
- Stationary vehicle departure and close-proximity movement, if supported by validated coverage.

These are candidate test contexts, not established operating capabilities.

## Sensor and coverage assumptions
The project has not selected a camera/radar package or vehicle platform. Candidate camera views may include front, rear and side/corner views, but coverage, overlap, blind zones, mounting, cleaning, calibration and environmental protection remain TBD. Radar or other modalities may contribute only after interface, provenance and performance verification. Never describe the system as 360-degree or all-weather without measured evidence.

## SUV-specific hazards
Vehicle bodywork, pillars, mirrors, parked vehicles, large vehicles, trailers, open doors, vegetation and street furniture can occlude people. Small image size, crowding, unusual movement, low contrast, darkness, headlight glare, rain, spray, fog, dirty lenses, reflections and camera damage can reduce performance. A pedestrian emerging from behind an obstruction may be detected too late. Stationary objects and mannequins may cause false alerts; tracking may switch between nearby people.

## Driver interface
Use concise, prioritised and time-bounded alerts. Distinguish detected presence from uncertain path conflict. Avoid persistent alarms for non-relevant objects and avoid presenting a predicted trajectory as fact. The interface must not distract the driver or replace mirrors, direct observation, parking sensors, certified vehicle safety systems or safe driving practice.

## Evaluation plan
Create a scenario matrix for each intended view and operating context. Measure per-class precision/recall/F1, missed detections, false alerts, localisation, tracking continuity, end-to-end alert latency, calibration and abstention. Include occlusion, crossing direction, stationary/approaching/receding motion, multiple people, cyclists, low light, glare, rain/spray, dirty/blocked sensors, camera failure, dropped frames and compute overload. Report per-scenario results and confidence intervals; thresholds are TBD pending hazard analysis.

## Safety boundary and non-claims
No autonomous braking, steering, throttle, propulsion or evasive manoeuvre. No collision avoidance/prevention guarantee, detection-range claim, safety rating or certification. Missing detections must never be interpreted as a clear path. Driver remains responsible for observation and vehicle control.