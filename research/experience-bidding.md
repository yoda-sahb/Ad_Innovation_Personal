# Experience Bidding

[Portfolio](../README.md) · [Research method](../docs/research-method.md)

**Status:** Exploratory hypothesis. Evaluation below is proposed; no experimental results are published here.

> Given what advertising has already accomplished, what can the next action still add?

## Problem and intended value

An impression-level decision can miss the economic context of a customer journey. Repeated exposure may contribute less over time, while a different action may address an unmet need. Observing a journey, however, is not the same as knowing which advertising caused progress.

The intended value is better allocation of advertiser spend through estimates of the next action's incremental contribution, including the option to abstain.

## Working hypothesis

Useful economic memory across a journey could improve bidding decisions while execution continues through ordinary auctions.

That hypothesis depends on the system distinguishing credible evidence of progress from uncertain or misleading signals. A more elaborate record of exposures alone would not establish the claim.

## Illustrative scenario

A campaign can bid on another opportunity after several earlier exposures. A journey-aware policy considers whether another exposure is likely to add value, whether a different action is preferable, or whether the budget is better used elsewhere.

This is a decision example, not a description of a deployed bidder.

## Assumptions to challenge

- Available evidence can support a useful estimate of progress despite missing, delayed, or ambiguous observations.
- That estimate adds information beyond strong frequency, recency, and conversion-based baselines.
- The improvement can justify additional decision latency, operating cost, and complexity.
- Abstention can improve allocation without merely reducing delivery or selecting easier-to-convert audiences.

## Proposed evaluation

Compare a journey-aware policy with a well-tuned baseline under comparable budgets, eligible opportunities, and outcome definitions. Include a simpler frequency-and-recency policy to test whether the added complexity is necessary.

| Question | Evidence to examine |
| --- | --- |
| Does the policy improve outcomes? | Incremental outcomes and cost per incremental outcome, using a suitable controlled design |
| Is memory doing useful work? | Ablations removing journey state or varying its freshness and reliability |
| Does abstention improve allocation? | Delivery, budget reallocation, and total outcomes alongside skipped opportunities |
| Is the policy practical? | Decision latency, operating cost, and behavior with missing or contradictory evidence |

Offline replay can help inspect policy behavior. It cannot by itself establish causal improvement because outcomes for actions not taken are generally unobserved.

## Evidence that would weaken the hypothesis

A simpler baseline performs as well; gains disappear under controlled measurement; or state uncertainty and operating costs outweigh the benefit.

## Open questions

- What evidence is sufficient to change a bid?
- How should uncertain progress affect the decision?
- When should prior evidence expire?
- What observation would justify abstention rather than a lower bid?
