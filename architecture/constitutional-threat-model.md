# Constitutional Threat Model

## What the Constitutional Threat Model Is

The **Constitutional Threat Model** defines **hazardous system states and conditions** that could violate safety, mission, or operational constraints.  

Unlike traditional threat models that focus on adversaries or attack techniques, NovaFuse treats **threats as hazards**—conditions that **could cause inadmissible or unsafe system states**.  
The architecture constrains system behavior such that these hazardous states **cannot occur**, independent of attack origin.

> In NovaFuse, threat modeling is **structural and semantic**, not probabilistic.

---

## Constraint Enforced
Only threats capable of violating defined invariants or bypassing admissibility boundaries are considered in scope.

## Enforcement Mechanism
Threats are mitigated structurally through invariant enforcement at the IDNA authority boundary and DREA execution gate. Any condition that compromises admissibility results in execution refusal prior to materialization.

## Failure & Refusal Semantics
If threat conditions invalidate admissibility, execution is refused immediately. No compensating controls, runtime overrides, or post-execution remediation paths are permitted.

## Evidence Produced
Threat-relevant refusal outcomes are recorded in the admissibility evidence stream when they directly influence execution decisions.

## Out of Scope / Not Claimed
This model does not enumerate operational vulnerabilities, implementation defects, supply-chain risks, or non-admissibility-related attack surfaces.

---

## Constitutional Threat Model FAQ

**What does “constitutional” mean in this threat model?**  
It refers to threats that undermine the fundamental guarantees and constraints of the architecture, not individual systems.

**Why model threats at the architectural level?**  
Some failures compromise the architecture’s integrity even when systems appear to function correctly.

**What qualifies as a constitutional threat?**  
Anything that weakens semantic integrity, invariant adherence, or authority boundaries at a structural level.

**How is this different from a security threat model?**  
Security models focus on attacks and vulnerabilities; this model focuses on architectural erosion and semantic decay.

**Where does this threat model apply?**  
Across all architectural decisions that could weaken core guarantees, regardless of domain or system.

**What does this model explicitly not attempt to do?**  
It does not enumerate exploits, attackers, mitigations, or operational responses.

<details>  <summary><strong>Why this page avoids implementation detail</strong></summary>  
Architectural Scope Reminder
> This document defines **architectural authority and invariants**.
> It does not describe how decisions are executed or enforced.
> Descriptions of *how* belong in system, implementation, or assurance documentation—not here. 
> This document defines architectural meaning and boundaries. 
> Implementation choices are intentionally excluded so that multiple systems can conform without semantic drift. 
> If you are looking for how a system enforces or realizes these concepts, refer to system-specific documentation.
</details>
