# Glossary

Key terms used throughout this knowledge base, organized by tradition.

---

## Information Theory

**Bit** — The fundamental unit of information. One bit is the information gained from a single fair coin flip. Defined by Shannon (1948).

**Channel Capacity** — The maximum rate at which information can be transmitted reliably over a noisy channel. Shannon's noisy channel coding theorem establishes this limit.

**Conditional Entropy** — H(X|Y). The remaining uncertainty about X after observing Y. Measures how much knowing Y reduces uncertainty about X.

**Entropy (Shannon)** — H(X) = −Σ p(x) log₂ p(x). The average information content (or uncertainty) of a random variable. Maximum when all outcomes are equally likely. Zero when the outcome is certain.

**Information** — The reduction of uncertainty. A message is informative to the extent it tells you something you didn't already know (Shannon, 1948).

**KL Divergence** — D(P‖Q) = Σ p(x) log₂[p(x)/q(x)]. The information cost of using distribution Q to approximate distribution P. Not a true distance (not symmetric), but measures how different two distributions are.

**Mutual Information** — I(X;Y) = H(X) − H(X|Y). The information shared between two variables. How much knowing one tells you about the other.

**Source Coding Theorem** — Data can be compressed to a rate approaching its entropy, but no further. The theoretical limit of lossless compression.

---

## Thermodynamics & Statistical Mechanics

**Boltzmann Distribution** — The probability distribution for states of a system in thermal equilibrium: P(state) ∝ exp(−E/kT). The maximum entropy distribution subject to a constraint on average energy.

**Entropy (Thermodynamic)** — S = kB ln Ω. The logarithm of the number of microstates consistent with a macrostate. Jaynes showed this is the same quantity as Shannon entropy when measured in natural units.

**Free Energy** — F = E − TS. The energy available to do work. In active inference, variational free energy is the quantity minimized by self-organizing systems.

**Generalized Boltzmann Distribution** — The distribution that maximizes Gibbs-Shannon entropy subject to known constraints. The only distribution where information-theoretic entropy equals thermodynamic entropy.

**Hamiltonian** — The energy function of a system. In thermoeconomics, the market price of a token acts as a Hamiltonian, retroactively imposing an energy function on hash space.

**IID (Independent and Identically Distributed)** — Outcomes that are statistically independent and drawn from the same distribution. Hash outputs in PoW mining are IID — each is independent of every other.

**Irreversibility** — A process is thermodynamically irreversible if it increases the total entropy of the universe. All real computations involve some irreversible steps (Landauer, Bennett).

**Landauer's Principle** — Erasing one bit of information dissipates at least kBT ln 2 of energy as heat. The minimum physical cost of information erasure.

**Maximum Entropy Principle (MaxEnt)** — When making inferences under incomplete information, assign the probability distribution that maximizes entropy subject to known constraints (Jaynes, 1957). The least biased inference given what you know.

**Partition Function** — Z = Σ exp(−E/kT). Normalizes the Boltzmann distribution. Contains all thermodynamic information about the system.

**Second Law of Thermodynamics** — The total entropy of an isolated system never decreases. Equivalently: irreversible processes always increase total entropy.

---

## Computational Mechanics

**Causal States** — Equivalence classes of histories that lead to statistically identical futures (Crutchfield). The memory states of the minimal predictor.

**Complexity** — Not randomness. Complexity is maximized between perfect order and perfect randomness — at the "edge of chaos" where structure and unpredictability coexist.

**Computational Mechanics** — James Crutchfield's framework for measuring the computational content of natural processes. Provides tools for quantifying pattern, structure, and memory in physical systems.

**Emergence** — The appearance of macroscopic structure or behavior not obviously present in microscopic rules. Crutchfield formalizes this as the difference between the entropy rate and the statistical complexity.

**Epsilon Machine (ε-Machine)** — The minimal, unique, optimal predictor of a stochastic process. Defined by causal states and probabilistic transitions between them. The canonical representation of a system's computational architecture.

**Statistical Complexity** — Cμ = H(causal states). The Shannon entropy of the causal state distribution. Measures the memory a system uses — distinct from entropy, which measures randomness.

---

## Wolfram Physics

**Causal Invariance** — The property of a rewriting system where different orderings of rule application produce the same causal structure. Gives rise to relativistic invariance in Wolfram's model and consensus in blockchain.

**Computational Irreducibility** — A computation's outcome cannot be predicted by any shortcut faster than running the computation itself. The foundation of proof-of-work security: there is no algorithm faster than brute-force search for valid hashes.

**Hypergraph** — The fundamental structure in the Wolfram model. Space, time, and matter emerge from the rewriting of hypergraph elements.

**Ruliad** — The entangled limit of all possible computations (Wolfram, 2021). The ultimate abstract structure from which all possible physical laws, observers, and mathematical truths emerge.

---

## Terrence Deacon & Active Inference

**Absential Features** — Properties of a system defined by what is absent — what could have happened but didn't. Constraint, information, and purpose are all absential. They exist because certain possibilities have been excluded.

**Active Inference** — A framework where self-organizing systems maintain themselves by acting on the world to minimize surprise (variational free energy). Extends the Free Energy Principle to include action.

**Autogen** — Deacon's minimal model of a self-creating system: autocatalysis + self-assembly. Neither alone is self-maintaining; together they form a reciprocal dependency that generates and maintains its own constraints.

**Free Energy Principle** — Any self-organizing system that persists must minimize variational free energy — an upper bound on surprise (Friston, 2010). Applied to economics: markets as inference engines.

**Markov Blanket** — The minimal set of variables that makes a system statistically independent of its environment. Defines the boundary between system and environment in active inference.

**Teleodynamics** — Deacon's term for self-creating, self-maintaining dynamics that generate and preserve their own organizing constraints. The highest level of emergent organization.

---

## Proof of Work & Blockchain

**Block** — A bundle of validated transactions, stamped with a valid proof of work. Blocks are chained together by including the previous block's hash in each new block header.

**Bernoulli Trial** — A random experiment with exactly two outcomes (success/failure). Each hash attempt in proof of work is a Bernoulli trial with success probability 1/2^d where d is the difficulty.

**Difficulty Adjustment** — The mechanism by which a PoW protocol adjusts computational cost to maintain a target block production rate, regardless of changes in total hash power. Interpretable as a MaxEnt constraint (Jaynes).

**Finality** — The assurance that a transaction cannot be reversed. In Bitcoin, finality is probabilistic (more confirmations = more final). In PoEM, finality is intrinsic (lower hash = more final).

**Hash Function** — A deterministic function that maps arbitrary inputs to fixed-size outputs. SHA-256 maps any input to a 256-bit output. Key properties: collision resistance, preimage resistance, avalanche effect.

**Hash Rate** — The number of hash operations per second performed by a miner or network. Measured in hashes/second (H/s). Directly proportional to energy expenditure.

**Hashcash** — Adam Back's proof-of-work system (1997) based on partial hash collisions. The direct ancestor of Bitcoin's mining algorithm.

**Longest Chain Rule** — Nakamoto consensus: when two valid chains compete, nodes follow the one with the most cumulative proof of work. A causal invariance mechanism.

**Merged Mining** — Mining multiple blockchains simultaneously using the same proof of work. Quai's hierarchical architecture uses merged mining across Prime, Region, and Zone chains.

**Mining** — The process of finding valid block hashes through brute-force search of nonce space. Each attempt is an irreversible computation with thermodynamic cost.

**Nonce** — A number varied by miners to change the block header's hash. The search through nonce space is the computational work in proof of work.

**Proof of Work (PoW)** — A consensus mechanism requiring participants to demonstrate computational expenditure. The thermodynamic cost makes the proof unforgeable.

**UTXO (Unspent Transaction Output)** — A discrete unit of value on a blockchain that can be consumed exactly once. The data structure used by Bitcoin, Quai, and related chains to track ownership.

---

## Quai Network

**kQuai** — The controller parameter balancing demand between Qi and Quai tokens. Increases when miners prefer Qi; decreases when they prefer Quai.

**PoEM (Proof of Entropy Minima)** — Quai's consensus mechanism. Ranks block candidates by hash value (lower = better) rather than comparing against a threshold. Extracts maximum information per computation.

**Qi** — Quai's energy token. Emission is proportional to hash rate (watts). A direct representation of the free energy supplied to the system.

**Quai** — Quai's scarcity token. Supply-constrained. Value derives from limited supply in the context of growing demand.

**Zone / Region / Prime** — The three levels of Quai's hierarchical blockchain architecture. Zones handle individual transactions; Regions aggregate zones; Prime provides final consensus across the entire network.

---

## Thermoeconomics

**Computational Thermoeconomics** — The science connecting energy, entropy, information theory, and computation to the foundations of economic value. The central thesis: proof of work is irreversible computation, and the economic properties of PoW money are consequences of the second law of thermodynamics.

**Energy Money** — A monetary system whose value is directly grounded in physical energy expenditure, not social convention or government decree. Qi is the purest implementation.

**Thermoeconomic Operator** — The formal framework (Macurdy, 2025) treating the blockchain as an operator that converts physical work into informational order, via IID hash-based Bernoulli trials and the MaxEnt principle.

**Unforgeable Costliness** — The property that producing a unit of value requires expenditure that cannot be faked, reversed, or cheaply simulated. In PoW, this follows from thermodynamic irreversibility.

---

*This glossary is actively maintained. Terms are added as new content is developed.*
