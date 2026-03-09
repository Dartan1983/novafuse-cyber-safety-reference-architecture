# Constraint Composition

## Constraint Enforced
Multiple constraints and invariants must compose without weakening admissibility guarantees.

## Enforcement Mechanism
All constraint composition is evaluated using logical AND semantics prior to execution. Composition order does not affect evaluation outcome.

## Failure & Refusal Semantics
Any contradiction, conflict, or violation within a composed constraint set results in global refusal. No prioritization, weighting, or override mechanism is permitted.

## Evidence Produced
The complete set of composed constraints evaluated is recorded in the admissibility evidence artifact.

## Out of Scope / Not Claimed
This document does not specify tooling, rule engines, or constraint authoring mechanisms.
