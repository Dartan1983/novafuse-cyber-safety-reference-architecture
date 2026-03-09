# Constraint Composition
## What Constraint Composition Is

**Constraint Composition** defines **how individual invariants and constraints combine** to determine whether system execution is admissible.  

In other words: while a **Core Invariant** defines a single atomic rule, **Constraint Composition** defines the **logic of multiple rules together**.

> All composition must preserve the atomic laws of NovaFuse (Core Invariants, DREA enforcement, refusal semantics).
> 
---

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
