# Causal Invariance and Consensus

## The Concept

A rewriting system is **causally invariant** if, regardless of the order in which rules are applied, the resulting causal structure is the same. Different observers may apply rules in different sequences, but they all arrive at the same causal graph — the same history of which events caused which other events.

In the Wolfram model, causal invariance is what gives rise to relativistic invariance: different observers (different reference frames) see events in different orders, but they agree on the causal relationships.

## The Connection to Blockchain Consensus

This is structurally identical to how proof-of-work consensus works:

- **Different miners** receive transactions in different orders
- **Different miners** construct candidate blocks with different transaction orderings
- **Despite this**, all honest miners converge on the same canonical chain — the same causal history

The longest-chain rule in proof of work is a causal invariance mechanism. It ensures that regardless of local ordering differences, the global causal structure (the blockchain) is agreed upon.

## Formal Parallel

| Wolfram Physics | Proof-of-Work Blockchain |
|---|---|
| Hypergraph rewriting rules | Transaction validation rules |
| Different rule application orders | Different miners, different mempools |
| Causal invariance | Consensus (longest chain rule) |
| Same causal graph | Same blockchain |
| Observers in different frames | Nodes in different network positions |

## Why This Isn't Just Analogy

Both systems solve the same fundamental problem: **distributed convergence without central coordination**. In physics, independent regions of space must agree on causal structure without a global clock. In blockchain, independent miners must agree on transaction ordering without a central authority.

The solution in both cases is the same: let the causal structure itself — the pattern of which events depend on which other events — determine the canonical ordering.

## Further Reading

- Gorard, "Some Quantum Mechanical Properties of the Wolfram Model" (2020) — causal invariance and quantum mechanics
- Wolfram Physics Project: Multiway Systems
- Nakamoto (2008) — the blockchain consensus implementation
