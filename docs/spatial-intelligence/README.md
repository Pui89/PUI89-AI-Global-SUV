# PUI89 AI Global SUV: Spatial Intelligence integration profile

This project now has a project-specific spatial integration profile at
`INTEGRATION_PROFILE.json`.

## Intended use
Advisory road-scene geometry, obstacle-relative position and scene-change evidence.

## Planned tasks
- 3D obstacle position and approximate dimensions
- Road-scene geometry and temporal change (after timestamps are validated)
- Spatial evidence references for human review

## Safety boundaries
- No road-boundary inference or collision prediction is implemented.
- No braking, steering, throttle or autonomous driving authority.
- Vehicle dynamics, weather, calibration and road testing remain unvalidated.

## Shared implementation dependency
The Spatial Intelligence Engine v0.1 was merged into the private Shared AI Core on 10 November 2026 ([PR #26](https://github.com/Pui89/PUI89-Shared-AI-Core/pull/26)). This file records the project-specific integration contract; it does not mean the project currently imports or executes the shared spatial module. The Shared AI Core is private and requires maintainer access.

Before runtime integration, require lawful sensor/data provenance, calibrated
coordinate frames, synchronized timestamps, sensor-health checks, uncertainty
handling, synthetic fault tests and project-specific human-review gates.
No physical actuation is enabled.

**Current evidence status:** profile documentation added; runtime adapter,
real sensor integration, accuracy, field performance and safety validation
remain pending. No hardware or paid service is required for this documentation
stage.
