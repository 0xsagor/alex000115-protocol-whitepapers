# Lightpaper: Decentralized Freelance Escrow

## Abstract
Traditional freelance platforms extract 10-20% value. The **Alex000115 Escrow Protocol** reduces this to 0% by replacing central oversight with a decentralized jury and milestone-based smart contracts.

## Economic Mechanism
We define the safety of a job $J$ as a function of the locked collateral $C$ and the reputation $R$ of the participants.

$$S(J) = \sum_{i=1}^{n} M_i + (R_f \times \delta)$$

Where:
* $M_i$: Value of milestone $i$.
* $R_f$: Staked reputation of the freelancer.
* $\delta$: Slashing coefficient.

## Dispute Resolution
When a dispute is raised, $k$ jurors are selected from a staked pool. Jurors are rewarded for consensus and slashed for divergence, following the Shelling Point theory of decentralized oracles.
