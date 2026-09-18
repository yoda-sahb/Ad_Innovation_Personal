# Agentic Advertising Operating System

[Portfolio](../README.md) · [Research method](../docs/research-method.md)

**Status:** Exploratory hypothesis and working name. This repository does not publish an operating system or production agent framework.

> When an agent spends money, who authorized the decision, and who can explain or stop it?

## Problem and intended value

An agent may have the technical ability to plan, negotiate, activate, or optimize advertising without a sufficiently clear mandate for each action. Access to an API does not fully describe the objectives, limits, or responsibilities attached to its use.

The intended value is autonomous execution whose authority and accountability remain understandable to the parties involved.

## Working hypothesis

Advertising agents may need an explicit operating framework for mandates, constraints, evidence, and revocation in addition to ordinary API permissions.

The research question is whether advertising introduces requirements that existing access controls, workflow approvals, and audit logs do not adequately address.

## Illustrative scenario

An agent proposes moving campaign budget. Before execution, the system must establish whose budget is involved, whether the move is within the mandate, which constraints apply, and whether that authority is still valid. After execution, the responsible party needs enough evidence to understand what occurred.

## Assumptions to challenge

- A mandate can be expressed clearly enough to check before consequential action.
- Constraints remain meaningful as actions cross organizational or agent boundaries.
- Revocation can prevent future actions even when some work is already in progress.
- Decision evidence can support accountability without exposing unnecessary sensitive information.

## Proposed evaluation

Compare ordinary role-based permissions and approval workflows with an explicit mandate-based approach using a bounded set of simulated advertising tasks.

| Scenario | Behavior to examine |
| --- | --- |
| In-scope action | Completes with an identifiable mandate and responsible owner |
| Conflicting instructions | Detects the conflict and applies a defined resolution or escalation |
| Delegation | Preserves applicable constraints without expanding authority |
| Revoked mandate | Blocks subsequent unauthorized action and accounts for work already in flight |
| Disputed outcome | Produces enough evidence to reconstruct authorization and execution |

Measure unauthorized actions, unnecessary blocks, execution delay, and completeness of the decision record. These are proposed checks, not a compliance certification.

## Evidence that would weaken the hypothesis

Existing permissions and workflows address the same cases with comparable reliability and less complexity, or the proposed mandate cannot be interpreted consistently enough to enforce.

## Open questions

- Which constraints must be checked before execution?
- Who resolves conflicts between advertiser, publisher, and platform objectives?
- What responsibility remains with a delegating party?
- Which evidence is necessary for explanation, and how long should it be retained?
