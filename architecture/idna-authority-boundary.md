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
