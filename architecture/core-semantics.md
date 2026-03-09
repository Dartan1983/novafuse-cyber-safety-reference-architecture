# Core Semantics
## What Core Semantics Are

Core semantics define the **fundamental meaning of system states, actions, and composition** in the NovaFuse architecture.  
They answer the question:

> “Under what conditions is a system action allowed to exist?”

In NovaFuse, semantics are **deterministic, invariant-driven, and enforceable**.  
They are **not guidelines, suggestions, or policies** — they are the rules that make unsafe states structurally impossible.

---

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
