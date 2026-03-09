# NovaFuse Cyber-Safety Reference Architecture

Reference architecture defining how unsafe states are made structurally unreachable through invariant-driven enforcement.

## Constraint Enforced
No execution path may proceed unless every defined invariant is satisfied at the authority boundary. Any violating composition or action is architecturally impossible.

## Enforcement Mechanism
Enforced at the IDNA authority boundary and DREA execution gate prior to materialization. All invariants apply uniformly across execution paths and compositions.

## Failure & Refusal Semantics
Violation produces an immediate deterministic refusal before any side-effect. Refusal carries an explicit reason code (ERI-00X series). No override, degradation, or deferral path exists.

## Evidence Produced
Evidenced by GMI-signed artifacts generated at evaluation time and written to canonical evidence stream. Absence of valid artifact renders transition impossible.

## Out of Scope / Not Claimed
This reference architecture does not document product features, model intent, output correctness, ethical evaluation, or private implementation details. It defines only the structural constraints that make unsafe states unreachable.
=======
# novafuse-cyber-safety-reference-architecture
Reference architecture defining invariant‑driven cyber‑safety for governed autonomous systems.

>>>>>>> 86ff43368075a485dad1ac969f0fb077f168fca8
