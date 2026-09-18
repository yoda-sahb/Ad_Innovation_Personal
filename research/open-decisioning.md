# OpenDecisioning

[Portfolio](../README.md) · [Research method](../docs/research-method.md)

**Status:** Exploratory hypothesis. Evaluation below is proposed; no protocol or validated implementation is published here.

> Can useful conclusions travel while underlying data, models, and authority remain with their owners?

## Problem and intended value

A publisher, retailer, buyer, and specialist model may each know something relevant to the same advertising decision. Combining that intelligence can require integrations or centralization that limit participation.

The intended value is to let independent sources contribute bounded, interpretable conclusions to a decision. This is the distinction explored here between transaction interoperability and decision interoperability.

## Working hypothesis

Independent parties could contribute useful conclusions without centralizing all of their underlying data or models, provided the receiving system can interpret their meaning, scope, limitations, and permitted use.

Keeping raw data local does not by itself establish privacy. Conclusions can disclose sensitive information or enable inference; that risk remains part of the research question.

## Illustrative scenario

A publisher contributes an assessment of contextual suitability, while a buyer supplies an objective and constraints. The decision uses those contributions without requiring the publisher to transfer its full source data or proprietary model.

The example leaves the representation and transport mechanism open.

## Assumptions to challenge

- Contributors can express conclusions precisely enough for another system to use.
- The receiver can assess reliability, freshness, and applicability.
- Conflicting conclusions can be handled without silently overriding the responsible party's authority.
- Participation creates sufficient value to justify integration and evaluation costs.

## Proposed evaluation

Start with a narrowly defined decision and compare a single-source baseline, a simple bilateral integration, and an approach that accepts independent contributions.

| Question | Evidence to examine |
| --- | --- |
| Does combining contributions improve the decision? | Outcome quality relative to the strongest simpler baseline |
| Can a contribution be interpreted correctly? | Agreement on meaning, scope, freshness, and permitted use |
| What happens when contributors disagree? | Conflict handling, abstention, and traceability |
| What happens when a contributor fails? | Behavior under timeout, stale evidence, and missing inputs |
| Is participation economical and safe? | Latency, integration effort, incentive conflicts, and disclosure risks |

Use synthetic or appropriately shareable examples for public work. A successful demonstration would support feasibility, not prove broad ecosystem adoption.

## Evidence that would weaken the hypothesis

Useful conclusions require nearly as much source data as centralization; interpretation costs exceed the gains; or straightforward bilateral integrations solve the selected problem equally well.

## Open questions

- What is the smallest useful conclusion?
- How should uncertainty and limitations be communicated?
- Who resolves conflicting objectives?
- Why would each participant contribute honestly and continue participating?
