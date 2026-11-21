# PUI89 AI Global SUV — AI-02 Object & Obstacle Detection Profile v1.0

**Status:** Proposed; no model, dataset, compute target or vehicle integration is verified.

## Objective
Detect supported road users and obstacles from approved SUV camera observations, returning evidence-linked hypotheses with confidence, uncertainty, freshness and sensor provenance. Outputs are driver advisory only.

## Operating domains
Define and test separately: low-speed parking/manoeuvring; forward road-scene awareness; rear and side awareness where coverage supports it. Do not transfer metrics between domains without evidence. AI-01 camera coverage does not imply every object is visible or detectable.

## Candidate priority classes
Cars, trucks/buses, motorcycles, bicycles, pedestrians, animals, cones, barriers, road-work equipment, debris, curbs and walls. Final ontology and priorities require requirements/hazard review. Retain unknown/other.

## Inputs and outputs
Consume AI-01 frames and metadata. Output class, image-space box/mask, timestamp, camera ID, model/ontology versions, confidence, uncertainty, visibility and quality. Optional tracking and spatial estimates require validated tracking/geometry, units and reference frame. Map through Observation, WorldState, ActionProposal and FailureReport. Never present unsupported metric distance or stale detections as current.

## SUV-specific challenges
Test body occlusion, wide-angle distortion, changing viewpoints, motion, small/distant objects, night, glare, rain/spray, dirty lenses, shadows, crowded scenes and partial occlusion. Evaluate each camera and operating domain separately before fusion.

## Evaluation
Use rights-cleared data, human-reviewed annotations and leakage-safe splits grouped by recording session/route/time. Report per-class precision/recall/F1, AP/mAP with IoU protocol, confusion matrix, missed critical objects, false positives, condition-specific results, calibration/uncertainty, latency, CPU/RAM and thermal performance. Requirements and numerical thresholds remain TBD. No gate is passed by this specification.

**Safety:** Advisory only. Driver retains steering, throttle, braking and propulsion control. No collision-prevention, autonomous-driving, complete 360-degree detection or road-validation claim.
**Maturity:** Proposed profile; implementation and validation not evidenced.
