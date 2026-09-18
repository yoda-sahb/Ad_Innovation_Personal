# Research method

[Portfolio](../README.md)

This repository organizes questions into hypotheses that can be assessed. The proposed tests are starting points for criticism, not a committed delivery roadmap.

## Structure of a research brief

1. **Problem:** identify the decision or constraint that causes difficulty.
2. **Intended value:** identify who benefits and what outcome should improve.
3. **Hypothesis:** state what might work and under which conditions.
4. **Assumptions:** expose the dependencies most likely to fail.
5. **Evaluation:** compare against a credible, simpler alternative.
6. **Disconfirmation:** specify evidence that would weaken or reject the idea.

## Evidence and maturity

Use the following labels when updating a brief. Status reflects evidence published in this repository; it does not imply anything about private work.

| Status | Required public material |
| --- | --- |
| Exploratory hypothesis | A defined question, assumptions, and proposed evaluation |
| Evaluation specified | A concrete baseline, protocol, measures, and decision criteria |
| Prototype published | Inspectable implementation with setup instructions and limitations |
| Results published | Reproducible method, results, comparison, and limitations |
| Revised or retired | An explanation of which evidence changed the hypothesis |

All four current briefs are exploratory hypotheses.

## Standards for future evaluation

- Compare against the strongest practical simpler solution.
- Define outcomes, guardrails, and thresholds before running an experiment.
- Distinguish prediction, attribution, and causal improvement.
- Include operating costs, latency, failure behavior, and integration effort.
- Report negative results and cases where benefits disappear.
- Mark synthetic examples, assumptions, and estimates explicitly.
- Support empirical claims with traceable sources or reproducible evidence.

## Current evidence boundary

The repository publishes concepts and proposed tests. It currently includes no public literature review, benchmark dataset, implementation, or experimental results. It therefore does not establish novelty, superiority, or production readiness.

Relevant prior work should be added with a source, the specific finding it supports, and an explanation of how it strengthens or challenges a brief.

## Choosing the next test

Prefer the smallest test that can disprove a consequential assumption. A useful first contribution might show that a simpler existing method already solves the problem, or that the information needed for a decision is unavailable.
