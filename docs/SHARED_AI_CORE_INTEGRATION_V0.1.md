# PUI89 Shared AI Core Integration — AI Global SUV v0.1

**Current product:** PUI89 AI Global SUV  
**Current project ID:** `pui89-ai-global-suv`  
**Status:** Adapter and synthetic contract fixtures are implemented. The project identity has been aligned with the SUV product. Current SUV-specific central conformance and runtime test results are **not yet re-run or verified** after this identity migration.

## Pinned interface

- Shared contract schema version: `0.1.0`
- Project adapter manifest version: `0.2.0`
- Project adapter version: `0.1.0`
- Project ID: `pui89-ai-global-suv`
- Canonical repository: [PUI89-Shared-AI-Core](https://github.com/Pui89/PUI89-Shared-AI-Core)
- Conformance runner used for the historical predecessor report: `pui89-core-conformance-cli` v`0.1.0`
- Historical Shared AI Core source pin: `cb5fdecb12acf4d810522b6a1c86567996b99718`
- Historical predecessor project source pin: `47bcf06d4200bd1cba4e7fd49048e658b1b01810`
- SUV identity-alignment baseline before this PR: `69dc0353f7760ea0023c2951d083b6650bebe694`

The adapter maps deterministic SUV signal/advisory records into Observation, WorldState, ActionProposal, FailureReport and Evidence Passport. It is a serialization boundary, not a perception system or vehicle controller. The Python package path `pui89_car` and legacy callable names are retained temporarily for compatibility; they are not the product identity.

## Historical conformance evidence

The report at [reports/shared-core-conformance-2026-11-13.json](../reports/shared-core-conformance-2026-11-13.json) records **10/10 synthetic fixtures passed** for the predecessor project identity `pui89-ai-car` and its historical source pin.

That report is retained unchanged as historical evidence. It is **not** presented as a conformance result for the current `pui89-ai-global-suv` project ID or the current SUV source revision. A new report must be generated against the exact current SUV commit and a freshly verified Shared AI Core commit before claiming current SUV conformance.

The historical CLI recorded commit pins as caller-declared values; it did not independently inspect Git metadata. The historical result was schema-fixture conformance only, not proof of semantic correctness, runtime adapter behaviour, external evidence truth, sensor calibration, model quality, or physical safety. Its `runtime_adapter_tested` field was `false`.

## Runtime adapter safeguards

- Observation serialization rejects empty source/evidence references, invalid or timezone-naive timestamps, non-boolean values and unsupported quality labels.
- Signal quality is mapped explicitly: good → usable; degraded → degraded; invalid → invalid; unknown → unknown.
- Unknown and conflicting signal states remain explicit in WorldState.
- Every ActionProposal is advisory-only, requires human approval and sets `execution_authorized: false`.
- The Evidence Passport remains unreviewed and unverified until actual evidence is supplied.
- Runtime adapter tests exist, but their current default-branch result has not been confirmed in this identity-alignment change.

## Safety boundary

- No actuator, ECU, CAN, steering, throttle, brake or propulsion interface is added.
- Unknown, conflicting or missing evidence is never converted into a safe road or flood assessment.
- The adapter does not independently verify source truth, sensor calibration or physical conditions.
- No autonomous-driving or physical performance claims are made.
- Hybrid subtype, chassis architecture, GVWR/GAWR, curb mass, validated payload and flood/wading limits remain unresolved or unvalidated.

No physical vehicle, sensor, model, road test, paid service or new external dependency is enabled by this integration.
