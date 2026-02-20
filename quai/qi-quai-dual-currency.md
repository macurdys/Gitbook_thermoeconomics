# Qi & Quai — Dual Currency System

## Two Tokens, Two Sides of Value

Quai Network operates with two native tokens that represent complementary aspects of economic value:

**Qi** — Proportional to hash rate. When a miner finds a valid block, Qi emission scales with the computational work performed (measured in entropy reduction). Qi is *energy money*: its supply directly reflects the physical work input to the system.

**Quai** — Supply-constrained, like Bitcoin. Its scarcity is enforced by the emission schedule and the thermodynamic cost of block production. Quai is *scarcity money*: its value derives from limited supply in the context of growing demand.

## The kQuai Controller

Miners choose whether to receive Qi or Quai for each block they mine. The protocol uses a controller parameter, **kQuai**, to balance demand between the two tokens:

- When more miners choose Qi → kQuai increases (making Quai more attractive)
- When more miners choose Quai → kQuai decreases (making Qi more attractive)

The controller equation: **kQuai(i) = kQuai(i−1) × [1 ± r]**

This creates a dynamic equilibrium between the two tokens, mediated by miner behavior and market prices.

## Thermodynamic Interpretation

The dual-currency system expresses the energy/entropy duality at the heart of thermoeconomics:

| Token | Thermodynamic Analogue | Economic Role |
|---|---|---|
| Qi | Energy (work performed) | Unit of account for computational work |
| Quai | Free energy (useful work) | Store of value with enforced scarcity |

Qi maps to **belief in the system** (energy input). Quai maps to **belief in belief in the system** (the market's valuation of that energy input). The relationship between them is analogous to the relationship between energy and free energy in thermodynamics.

## Further Reading

- [PoEM Consensus](poem-consensus.md) — how mining works in Quai
- [Research: Qi Quai Controller Report](../research/qi-quai-controller.md) — formal analysis
- [Active Inference and Economic Systems](../foundations/active-inference/economic-systems.md) — the Free Energy Principle interpretation
