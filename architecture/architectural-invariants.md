# Architectural Invariants

## Constraint Enforced
All system behavior must preserve the core invariant: unsafe or inadmissible states are structurally unreachable.

## Enforcement Mechanism
Architectural invariants are enforced through mandatory evaluation at the IDNA authority boundary and DREA execution gate. Invariants apply uniformly across all execution paths and compositions.

## Failure & Refusal Semantics
Any violation of an architectural invariant produces immediate refusal prior to execution. Invariant violations are not recoverable at runtime.

## Evidence Produced
Invariant evaluation outcomes are recorded as part of the GMI-signed admissibility artifact generated at execution evaluation time.

## Out of Scope / Not Claimed
This document does not define operational policies, implementation techniques, or optimization strategies.
