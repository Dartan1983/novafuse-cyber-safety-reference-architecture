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

---

## Core Semantics FAQ 

**1. What are Core Semantics?**  
Core Semantics define the fundamental meaning of system **states, actions, and composition**. They determine under what conditions a system action is allowed to exist.

**2. Why are Core Semantics necessary?**  
They ensure that all actions are **deterministic, invariant-driven, and enforceable**, preventing unsafe states from ever arising.

**3. Where do Core Semantics apply?**  
At every point where system actions, transitions, or compositions are defined across the architecture.

**4. How do Core Semantics relate to Core Invariants?**  
Core Semantics provide the **meaning and rules**, while Core Invariants are the **non-negotiable properties** derived from that meaning.

**5. What happens if semantics are violated?**  
Any inadmissible or undefined action is **immediately refused** before execution, with evidence generated. No partial execution or override is allowed.

**6. What is evaluated to enforce Core Semantics?**  
All relevant invariants are checked under **logical AND composition**, ensuring full coherence before any action proceeds.

**7. What is out of scope for Core Semantics?**  
Implementation details, syntax, tooling, compilers, runtime behavior, model outputs, or ethical evaluation mechanisms are not included; only structural meaning is defined.

<details>  
<summary><strong>Why this page avoids implementation detail</strong></summary>  
This document defines the **meaning of system actions and constraints**. Enforcement is intentionally left to system-specific mechanisms to prevent semantic drift.
</details>
