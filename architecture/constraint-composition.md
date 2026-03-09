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

---

## Constraint Composition FAQ

**What is a constraint in this architecture?**  
A constraint is a non‑negotiable architectural rule that limits what is considered admissible.

**What does “constraint composition” mean?**  
It describes how multiple constraints coexist and apply simultaneously without contradiction.

**Why is constraint composition important?**  
Architectures fail when individually valid constraints interact in incompatible ways.

**Where does constraint composition apply?**  
At the intersection of architectural rules, invariants, and semantic guarantees.

**What happens when constraints appear to conflict?**  
It signals either a misunderstanding or an architectural inconsistency that must be resolved conceptually.

**What is out of scope for this page?**  
Resolution strategies, prioritization schemes, or algorithmic conflict handling.

<details>  <summary><strong>Why this page avoids implementation detail</strong></summary>  
This document defines architectural meaning and boundaries. Implementation choices are intentionally excluded so that multiple systems can conform without semantic drift. If you are looking for how a system enforces or realizes these concepts, refer to system-specific documentation.
</details>
