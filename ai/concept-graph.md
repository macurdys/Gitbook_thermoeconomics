# Concept Graph

A dependency map showing what must be understood before what. Give this to an AI tutor so it can sequence your learning correctly.

---

## How to Read This

Each concept lists its **prerequisites** (what you need first), what it **teaches**, what it **connects to**, and its **difficulty level**. If something doesn't make sense, check whether you've covered the prerequisites.

---

## Level 1: Foundations (No Prerequisites)

### Probability Basics
- **Teaches:** Random variables, probability distributions, expected value, variance
- **Connects to:** Shannon entropy, Bernoulli trials
- **Difficulty:** Beginner
- **Time:** 30 min

### What Is a Blockchain?
- **Teaches:** Blocks, chains, transactions, consensus, decentralization
- **Connects to:** Proof of work, UTXO, difficulty adjustment
- **Difficulty:** Beginner
- **Time:** 30 min

---

## Level 2: Information Theory Core

### Shannon Entropy
- **Prerequisites:** Probability basics
- **Teaches:** Information content, entropy formula, source coding theorem, channel capacity
- **Connects to:** Jaynes MaxEnt, Landauer, PoW information content, statistical complexity
- **Difficulty:** Intermediate
- **Time:** 45 min

### Jaynes — Maximum Entropy Principle
- **Prerequisites:** Shannon entropy
- **Teaches:** MaxEnt principle, Lagrange multipliers, partition function, Boltzmann distribution derivation
- **Connects to:** Difficulty adjustment, Generalized Boltzmann Distribution, Thermoeconomic Operator
- **Difficulty:** Advanced
- **Time:** 60 min

### Landauer's Principle
- **Prerequisites:** Shannon entropy, basic thermodynamics (kBT)
- **Teaches:** Physical cost of erasure, kBT ln 2 limit, irreversibility
- **Connects to:** Bennett, PoW thermodynamics, mining energy cost
- **Difficulty:** Intermediate
- **Time:** 30 min

### Bennett — Thermodynamics of Computation
- **Prerequisites:** Landauer's principle
- **Teaches:** Reversible computation, irreversible erasure, logical vs thermodynamic irreversibility
- **Connects to:** PoW as irreversible computation, nonce erasure
- **Difficulty:** Advanced
- **Time:** 45 min

---

## Level 3: Proof of Work

### Dwork & Naor (1993)
- **Prerequisites:** What is a blockchain? (optional: hash functions)
- **Teaches:** Proof of work as anti-spam, computational puzzles, pricing via processing
- **Connects to:** Hashcash, Nakamoto
- **Difficulty:** Beginner
- **Time:** 20 min

### Hashcash (Back, 1997)
- **Prerequisites:** Dwork & Naor, hash functions
- **Teaches:** Partial hash collisions, practical PoW, difficulty parameter
- **Connects to:** Bitcoin mining, difficulty adjustment
- **Difficulty:** Intermediate
- **Time:** 30 min

### Finney — Reusable Proofs of Work (2004)
- **Prerequisites:** Hashcash
- **Teaches:** Transferable proofs, token creation from computation
- **Connects to:** Bitcoin, energy money concept
- **Difficulty:** Intermediate
- **Time:** 20 min

### Nakamoto — Bitcoin (2008)
- **Prerequisites:** Hashcash, what is a blockchain
- **Teaches:** PoW consensus, longest chain rule, difficulty adjustment, emission schedule
- **Connects to:** Everything — this is the central case study
- **Difficulty:** Intermediate
- **Time:** 45 min

### Difficulty Adjustment
- **Prerequisites:** Nakamoto, Shannon entropy, Jaynes MaxEnt
- **Teaches:** Target block time, hash rate adaptation, MaxEnt interpretation
- **Connects to:** Thermoeconomic Operator, PoEM
- **Difficulty:** Advanced
- **Time:** 30 min

---

## Level 4: Deeper Frameworks

### Computational Irreducibility (Wolfram)
- **Prerequisites:** Hash functions, basic computation concepts
- **Teaches:** No shortcut to answer, must run the computation, security foundation of PoW
- **Connects to:** PoW security, causal invariance
- **Difficulty:** Intermediate
- **Time:** 30 min

### Causal Invariance (Wolfram)
- **Prerequisites:** Computational irreducibility, Nakamoto consensus
- **Teaches:** Order-independent convergence, structural analogy to consensus
- **Connects to:** Longest chain rule, distributed agreement
- **Difficulty:** Advanced
- **Time:** 45 min

### Crutchfield — Computational Mechanics
- **Prerequisites:** Shannon entropy
- **Teaches:** Epsilon machines, causal states, statistical complexity
- **Connects to:** Mining process structure, edge of chaos, emergence
- **Difficulty:** Advanced
- **Time:** 60 min

### Epsilon Machines
- **Prerequisites:** Crutchfield, conditional entropy
- **Teaches:** Minimal predictors, causal state equivalence, Cμ measurement
- **Connects to:** Blockchain as structured process vs. hash as random output
- **Difficulty:** Advanced
- **Time:** 45 min

### Deacon — Autogenic Theory
- **Prerequisites:** Basic thermodynamics, self-organization concepts
- **Teaches:** Constraint as cause, autogens, teleodynamics
- **Connects to:** PoW as self-maintaining system, mining incentive loops
- **Difficulty:** Intermediate (conceptual) / Advanced (formal)
- **Time:** 45 min

### Friston — Free Energy Principle
- **Prerequisites:** Shannon entropy, Bayesian inference basics
- **Teaches:** Surprise minimization, variational free energy, Markov blankets
- **Connects to:** Active inference in economic systems, Qi/Quai dynamics
- **Difficulty:** Advanced
- **Time:** 60 min

---

## Level 5: Synthesis

### PoW as Thermodynamic Process
- **Prerequisites:** ALL of Levels 2-4
- **Teaches:** The nine-step argument connecting all six traditions
- **Connects to:** Thermoeconomic Operator, PoEM, energy money
- **Difficulty:** Advanced
- **Time:** 45 min

### Thermoeconomic Operator
- **Prerequisites:** PoW as Thermodynamic Process, Jaynes MaxEnt, Boltzmann distribution
- **Teaches:** IID Bernoulli trials → MaxEnt → Generalized Boltzmann, information as rank, market-induced Hamiltonian
- **Connects to:** PoEM, Qi emission, energy money
- **Difficulty:** Expert
- **Time:** 90 min

### PoEM Consensus
- **Prerequisites:** Nakamoto, difficulty adjustment, Thermoeconomic Operator
- **Teaches:** Ranked hashes, instant finality, maximum information extraction
- **Connects to:** Qi emission, dual currency
- **Difficulty:** Advanced
- **Time:** 45 min

### Qi/Quai Dual Currency
- **Prerequisites:** PoEM, Free Energy Principle, Thermoeconomic Operator
- **Teaches:** Energy token (Qi), scarcity token (Quai), kQuai controller, energy/entropy duality
- **Connects to:** Energy money, active inference in economics
- **Difficulty:** Advanced
- **Time:** 45 min
