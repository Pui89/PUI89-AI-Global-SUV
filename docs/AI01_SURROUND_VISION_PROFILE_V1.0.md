# PUI89 AI Global SUV — AI-01 Surround Vision Profile v1.0

**Status:** Proposed product profile. No cameras, model, compute hardware or vehicle integration are established.
**Shared module:** [PUI89 Multi-Vehicle Surround Vision — Shared Module v1.0](https://github.com/Pui89/PUI89-Shared-AI-Core/blob/main/docs/architecture/PUI89_MULTI_VEHICLE_SURROUND_VISION_V1.0.md).

## 1. Purpose

Define the SUV-specific adaptation of PUI89 AI-01 for multi-camera visual awareness, near-field context and a possible surround-view display. It is a driver-advisory perception system, not an autonomous driving or collision-prevention system.

## 2. Proposed camera configuration

Initial research layout:
- CAM-F: forward camera near the front grille, with protected mounting and a validated view past the vehicle body.
- CAM-R: rear camera near the tailgate, with view and mounting assessed against liftgate operation and contamination.
- CAM-L: left-side camera near the mirror or approved body location.
- CAM-RH: right-side camera near the mirror or approved body location.
- Optional corner cameras only where a coverage map demonstrates material blind-zone reduction.

Four cameras are a starting research configuration, not proof of complete 360-degree coverage. Final positions, lenses, field of view, resolution, frame rate, environmental rating and calibration method remain TBD.

## 3. Functional pipeline

Capture and timestamp → source/quality validation → calibration and distortion correction → per-camera perception → optional stitched visualisation → cross-camera association where justified → uncertainty/coverage map → driver advisory interface → evidence and fault logging.

Keep parking/low-speed surround visualisation distinct from moving-road object perception. A stitched image must not conceal seams, occlusions or unsupported regions.

## 4. SUV-specific requirements

- Define near-field ground coverage, front/rear corner visibility, wheel/bumper occlusion and camera overlap.
- Assess road grime, rain, spray, glare, night, backlight, temperature and vibration.
- Use synchronised frames for cross-camera tracking; otherwise mark observations as unaligned.
- Maintain camera-specific calibration records and detect calibration expiry or movement.
- Evaluate driver display legibility and distraction; mirrors and direct observation remain necessary.
- Optional radar/ultrasonic evidence must retain separate provenance and modality identity.

## 5. Shared AI Core interfaces

Reuse Observation, WorldState, ActionProposal and FailureReport. Include camera ID, capture/receive timestamps, calibration version, quality, freshness, confidence, uncertainty, coverage status and model version. Driver-facing proposals are limited to information and warnings.

## 6. Verification

Test daylight, night, glare, rain/spray, dirty/blocked lens, disconnected camera, timestamp skew, calibration drift, stitching seams, moving-object association, parked and moving contexts, and compute overload. Record held-out detection metrics, false/missed detections, latency, resource use, uncertainty and per-camera coverage.

No numerical targets are set until SUV use cases and hazard analysis define them. No gate is passed by this document.

## 7. Safety and evidence boundary

No autonomous steering, throttle, braking or propulsion. No claim of complete 360-degree awareness, collision prevention, validated detection range, ADAS certification or road testing. The driver remains responsible and in control.

**Maturity:** Proposed profile specified; implementation and validation not evidenced.
