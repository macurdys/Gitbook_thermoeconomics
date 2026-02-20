# Module 4: Blockchain Architecture

How blockchains achieve distributed consensus: fault tolerance, replicated state machines, consensus mechanisms, and the architectural choices that define each network.

🔗 **[Take this module on Wolfram U →](https://www.wolfram.com/wolfram-u/courses/finance/overview-of-blockchain-design-fin041/)**

---

## Key Concepts

**Byzantine fault tolerance** — The ability of a distributed system to reach consensus even when some participants are dishonest or faulty. The Byzantine Generals Problem (Lamport, 1982) established the theoretical limits.

**Replicated state machines** — A blockchain is a replicated state machine: every node maintains the same state, updated by the same sequence of transactions. Consensus determines which transactions enter the sequence and in what order.

**Consensus mechanisms** — The rules by which nodes agree on the next valid state. Proof of work (Nakamoto consensus) achieves this through computational expenditure. Proof of stake achieves it through economic collateral. The thermoeconomic thesis is that only proof of work is grounded in physics.

**Network topology** — How nodes connect and communicate. Affects propagation time, orphan rates, and centralization pressure. Quai's hierarchical architecture (Prime → Region → Zone) is a specific topological choice designed for throughput.

## Connection to Thermoeconomics

Architecture determines the system's thermodynamic properties. The choice of consensus mechanism determines whether the system's security is grounded in physical work (thermodynamic) or social agreement (game-theoretic). Causal invariance — independent observers converging on the same causal structure — is the physics analogue of distributed consensus.

## Further Resources

- [Causal Invariance and Consensus](../foundations/wolfram-physics/causal-invariance.md)
- [Quai Network Architecture](../quai/README.md)
