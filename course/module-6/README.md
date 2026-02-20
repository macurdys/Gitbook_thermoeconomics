# Module 6: Thermoeconomics

*The capstone module.* This is where everything converges.

---

## Overview

Modules 1–5 built your understanding of blockchains from the ground up: what they are, how to program them, the cryptography that secures them, the architectures that scale them, and the components they're made of.

Module 6 asks: **why does any of this work?**

The answer is thermodynamics. Proof of work is not an arbitrary engineering choice — it is the natural expression of a deep physical structure. The economic properties of proof-of-work money (scarcity, unforgeable costliness, objective measurability) are consequences of the second law of thermodynamics applied to computation.

## Prerequisites

Before this module, you should be comfortable with:
- Blockchain fundamentals (Modules 1–5)
- [Information Theory](../foundations/information-theory/README.md) — especially Shannon, Jaynes, and Landauer
- [Proof of Work as Thermodynamic Process](../foundations/proof-of-work/pow-thermodynamics.md)

## Curriculum

### 6.1 — Information Is Physical
Shannon entropy. Landauer's principle. The minimum energy cost of computation. Why erasing a bit costs kT ln 2 joules and why this matters for blockchain.

### 6.2 — Mining as Irreversible Computation
SHA-256 as a many-to-one function. Each hash discards information. Bennett's erasure principle. The difficulty adjustment as a MaxEnt constraint (Jaynes).

### 6.3 — The Thermoeconomic Operator
The formal framework: IID Bernoulli trials → MaxEnt → Generalized Boltzmann Distribution. The blockchain as an operator that converts physical work into informational order.

### 6.4 — PoEM: Maximum Information Extraction
Why threshold-based difficulty is lossy compression. How Proof of Entropy Minima ranks every hash output, extracting maximum information per computation.

### 6.5 — Energy Money
Qi as a direct representation of free energy supplied to the system. The dual-token system (Qi/Quai) as the economic expression of the energy/entropy duality.

### 6.6 — The Bigger Picture
Proof of work as the latest expression of the thermodynamic process that drives all complex systems — from stellar nucleosynthesis to metabolism to markets.

---

## Reading

- [The Thermoeconomic Operator](../foundations/synthesis/thermoeconomic-operator.md) — the paper
- [From Big Bang to Blockchain](../foundations/synthesis/from-big-bang.md) — the conversations
- [PoW as Thermodynamic Process](../foundations/proof-of-work/pow-thermodynamics.md) — the nine-step argument
- [PoEM Consensus](../quai/poem-consensus.md) — the implementation

*Full module content is under active development.*
