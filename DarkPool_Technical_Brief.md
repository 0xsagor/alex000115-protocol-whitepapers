# Technical Brief: ZK-Dark Pool Privacy

## The Problem
On public blockchains, order flow is transparent. Front-running bots extract value from large traders, creating a "Dark Forest" environment.

## The Solution
By using ZK-SNARKs, traders can prove they possess an asset without revealing the price or volume of their order.

### Zero-Knowledge Constraint
A trade is valid if and only if:
1. The commitment $C$ is part of the Merkle Tree $T$.
2. The nullifier $N$ has not been previously spent.
3. The price $P_{buy} \geq P_{sell}$.

$$\text{Proof} = \pi \{ (note_{in}, note_{out}, sk): \text{Verify}(sk, note) = 1 \}$$

The execution happens in a "Dark" state where only the settlement is visible to the public.
