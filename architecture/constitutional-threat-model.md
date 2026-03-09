# Constitutional Threat Model

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
