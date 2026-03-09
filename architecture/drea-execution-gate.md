# DREA Execution Gate

## Constraint Enforced
No execution may occur unless admissibility has been deterministically evaluated and satisfied across all applicable invariants.

## Enforcement Mechanism
Enforced by the DREA execution gate operating at the IDNA authority boundary prior to any materialization. Evaluation is atomic and applies logical AND semantics across all invariant checks.

## Failure & Refusal Semantics
Any failure, inconsistency, or violation during admissibility evaluation produces an immediate deterministic refusal. Partial evaluation, probabilistic outcomes, or deferred decisions are not permitted.

## Evidence Produced
Each evaluation produces a GMI-signed artifact recording of decision outcome, complete set of invariants evaluated, and applicable refusal reason code when relevant.

## Out of Scope / Not Claimed
This file does not specify implementation details, performance optimizations, caching strategies, or internal representations of the DREA engine.
