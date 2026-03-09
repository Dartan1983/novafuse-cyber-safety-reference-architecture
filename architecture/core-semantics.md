# Core Semantics

## Constraint Enforced
Every state transition in NovaFuse runtime must be either fully admissible under all defined invariants or impossible. No undefined, partially admissible, or contradictory state may exist.

## Enforcement Mechanism
Enforced atomically at the IDNA authority boundary and DREA execution gate prior to any materialization. All constraint composition is evaluated using logical AND semantics; any single violation blocks the entire transition.

## Failure & Refusal Semantics
Any inadmissible or undefined state produces an immediate deterministic refusal before any side-effect occurs. Refusal is atomic, inviolable, first-class, and carries an explicit reason code (ERI-00X series). No override, degradation, deferral, or recovery path exists.

## Evidence Produced
This constraint is evidenced by a GMI-signed artifact generated at the moment of evaluation. The artifact records the complete set of invariants evaluated and is written to the canonical evidence stream. Absence of a valid artifact renders the transition impossible.

## Out of Scope / Not Claimed
This definition does not specify concrete syntax, tooling, compilers, model training, output correctness, ethical evaluation, or implementation details of a private production codebase. It defines only the structural rules that make unsafe states unreachable.
