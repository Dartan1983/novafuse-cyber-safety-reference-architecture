# IDNA Authority Boundary

## What IDNA Is

**IDNA (Identity, Data, Networks, and AI)** defines the authoritative semantic domain
within which system states, actions, and invariants are evaluated for admissibility
in the NovaFuse architecture.

It establishes the boundary at which **identity context, data meaning, network scope,
and AI decision semantics** are normalized so that admissibility decisions are
coherent, consistent, and unambiguous.

In short, IDNA defines **where meaning applies**.

---

## Question IDNA Answers

IDNA answers the question:

> “Within what domain do identity, data, network interactions, and AI actions
have defined meaning for admissibility?”

Outside the IDNA boundary, system actions are undefined with respect to NovaFuse
semantics and cannot be evaluated for admissibility.

## Role in the Architecture

IDNA does not execute actions or evaluate invariants itself.

It provides the **semantic and contextual boundary** against which admissibility
is evaluated by architectural authorities such as **DREA**.

All admissibility decisions occur *with respect to* the IDNA boundary,
but are not performed *by* it.

## Relationship to Other Architectural Concepts

- **Core Semantics** define meaning within the IDNA domain.
- **Core Invariants** apply only to states that exist within the IDNA boundary.
- **DREA** evaluates admissibility against invariants defined in the IDNA domain.
- **Refusal** occurs only after evaluation, not at the boundary itself.

## Out of Scope / Not Claimed

IDNA does not define:
- identity mechanisms or credential formats
- data schemas or storage models
- network protocols or topologies
- AI model architectures or training methods
- implementation details for normalization or provenance handling

IDNA defines **semantic authority**, not implementation.

---

## IDNA Authority Boundary — FAQ (Localized, Comprehension‑Only)

**1. What does “IDNA” mean?**  
IDNA stands for **Identity, Data, Networks, AI**. Each component defines a dimension of the system’s **semantic authority boundary**:

- **Identity** — All uniquely identifiable entities, roles, or actors. Governs authentication, provenance, and traceable semantic claims.  
- **Data** — All system information and state representations. Defines what is authoritative, admissible, and consistent.  
- **Networks** — Communication and connectivity structures. Determines what entities can influence or observe system states.  
- **AI** — Algorithms, models, and autonomous agents. Governs admissibility of AI‑produced actions under architectural invariants.

Together, IDNA defines the **full semantic domain** where admissibility rules are enforced.

**2. What does “authority” mean in IDNA?**  
Authority refers to the legitimate source of truth for defining and asserting semantics in Identity, Data, Networks, and AI.

**3. Why must identity authority be bounded?**  
Because unbounded authority leads to conflicting identities and semantic fragmentation, undermining structural integrity.

**4. Where does the IDNA authority boundary apply?**  
At the point where identity meaning is defined, asserted, or altered across the system.

**5. What happens when the authority boundary is crossed?**  
Identity, data, or AI claims lose architectural legitimacy, even if they are technically consistent.

**6. How does this boundary relate to governance?**  
It informs governance decisions but does not prescribe organizational process, ownership, or operational procedure.

**7. What is explicitly out of scope for the authority boundary?**  
Access control, storage mechanisms, resolution services, and runtime workflows.

<details>  
<summary><strong>Why this page avoids implementation detail</strong></summary>  
This document defines architectural meaning and boundaries. Implementation choices are intentionally excluded so that multiple systems can conform without semantic drift. If you are looking for how a system enforces or realizes these concepts, refer to system-specific documentation.
</details>
