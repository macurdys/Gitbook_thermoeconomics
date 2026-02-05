# Crutchfield POCI Course — Extracted Slide Content
## Physics of Information (256A) & Physics of Computation (256B)
### UC Davis — Jim Crutchfield
#### Text extracted from PDF slide decks

---

# Lecture 1 Slides: Overview
## Copyright © 2025 J. P. Crutchfield

### Core Thesis
- The Industrial Age → Thermodynamics
- The Information Age → ???
- Physics to date: energy book-keeping (storage, transduction)
- **Information is not Energy**
- The role of information in causality

### Mechanism Revived
- Deterministic chaos: Nature actively produces information
- What is randomness? Where does it come from?
- Self-Organization: Nature actively produces structure (aka "stores" information)
- What is structure? Order? Regularity?

### Course Logic
1. Complex systems: order and chaos
2. Self-organization: Emergence of chaos, Emergence of order
3. Intrinsic Computation: How nature stores & processes information

### Main Idea
**Structure = Information + Computation**
**How Nature is Structured is How Nature Computes**

### The Learning Channel
```
...001011101000...
System → Instrument → Process
         ↓
       Modeller
```
- Goals: Quantify unpredictability, Quantify structure, Both related to computation

### Applications
- Intrinsic Computation (Analog, Classical, Quantum, Neural, Evolution, DNA)
- Nanotechnology, Biology, Machine Learning, Automated Scientific Inference

### Materials
- [NDAC] Nonlinear Dynamics and Chaos, Strogatz, 2nd Ed
- [EIT] Elements of Information Theory, Cover & Thomas, 2nd Ed
- [CMR] Computational Mechanics Reader (articles on course website)

### Presage: "Between Order and Chaos" (Nature Physics 2012)
- Poincaré: determinism and randomness are essential and unavoidable twins
- "Statistical mechanics" and "deterministic chaos" express this duality
- Shannon: surprise = negative log of probability (self-information: Iᵢ = log₂pᵢ)
- Source entropy rate H[X] determines compressibility
- Communication channel: mutual information I[X;Y] = H[X] − H[X|Y]

---

# Lecture 14 Slides: Entropies (Information Theory)
## Reading: EIT, Chapters 1 & Sections 2.1-2.8

### Sources of Information
- Apparent randomness: Uncontrolled initial conditions
- Actively generated: Deterministic chaos
- Hidden regularity: Ignorance of forces, Limited capacity to model structure

### History
- Boltzmann (19th C): Equilibrium, large-scale systems
- Hartley-Shannon-Wiener (Early 20th): Communication & Cryptography
- Current: Coding, Statistics, Dynamics, and Learning

### Information as Uncertainty
- Observe something unexpected → Gain information
- Bateson: "A difference that makes a difference"
- Shannon: measure of surprise ∝ −log Pr(event)

### Khinchin/Shannon Axioms → Shannon Entropy
H(X) = −Σᵢ pᵢ log₂ pᵢ

Properties:
- H(X) ≥ 0
- H(X) = 0 iff p(x) = 1 for exactly one x (predictable)
- H(X) = log₂ k iff p(x) = 1/k (maximally random)

### Joint & Conditional Entropy
- H(X,Y) = −Σ p(x,y) log₂ p(x,y)
- H(X|Y) = H(X,Y) − H(Y)
- Independent: X⊥Y → H(X,Y) = H(X) + H(Y)

### Mutual Information
I(X;Y) = Σ p(x,y) log₂[p(x,y)/(p(x)p(y))]
- I(X;Y) = H(X) − H(X|Y) = H(X) + H(Y) − H(X,Y)
- Symmetric: I(X;Y) = I(Y;X)
- Self-information: I(X;X) = H(X)

### Relative Entropy (KL Divergence)
D(X||Y) = Σ p(x) log₂[p(x)/q(x)]
- D(X||Y) ≥ 0, = 0 iff P = Q
- Not symmetric, not a distance

### Information Distance
d(X,Y) = H(X|Y) + H(Y|X) = H(X,Y) − I(X;Y)
- IS a true metric (positive, symmetric, triangle inequality)

### I-Diagram
H(Y) = H(Y|X) + I(X;Y) + H(X|Y) = H(X)
      ←————————— H(X,Y) ——————————→

### Key Inequalities
- Conditioning reduces entropy: H(X|Y) ≤ H(X)
- Independence bound: H(X₁,...,Xₙ) ≤ Σ H(Xᵢ)
- Data Processing Inequality: X→Y→Z ⇒ I(X;Y) ≥ I(X;Z)

### Chain Rules
- Entropy: H(X₁,...,Xₙ) = Σ H(Xᵢ|Xᵢ₋₁,...,X₁)
- MI: I(X₁,...,Xₙ;Y) = Σ I(Xᵢ;Y|Xᵢ₋₁,...,X₁)

---

# Lecture 21 Slides: What's Wrong with Information Theory? (256B Overview)
## Copyright © 2025 J. P. Crutchfield

### Physics of Information Review
- Information-Entropy Roadmap for a Stochastic Process
- Block Entropy H(L), Entropy Rate hμ, Excess Entropy E

### Entropy Hierarchy (Discrete-Time Derivatives & Integrals)
| Level | Gain (Derivative) | Information (Integral) |
|-------|------------------|----------------------|
| 0 | Block Entropy H(L) | Transient Information T |
| 1 | Entropy Rate hμ(L) = ΔH(L) | Excess Entropy E |
| 2 | Predictability Gain Δ²H(L) | Total Predictability G = −R |

### "Regularities Unseen, Randomness Observed"
- Structure converted to apparent randomness (E & T → hμ)
- Ignoring process memory → over-estimate true randomness

### What is Information? (Depends on the question!)
- Uncertainty, surprise, randomness: H(X)
- Compressibility: hμ
- Transmission rate: R = log₂|A| − hμ
- "Memory", apparent stored information: E
- Synchronization: T
- Ephemeral: rμ
- Bound: bμ

### Inadequacies of Information Theory
- Never tells you WHAT information content is
- Only measures AMOUNTS of information
- No direct measure of structure or organization

### Preview of 256B: Physics of Computation
**Structure = Information + Computation**
**How Nature is Structured is How Nature Computes**

---

# Lecture 22 Slides: The Learning Channel (Causal States & ε-Machines)

### 256B Topic List
Core: Effective States & Dynamic, ε-Machines, Measures of Complexity, Irreversibility, Crypticity, Meaning & Measurement Semantics, Information Measures Redux, Directional Computational Mechanics, Intrinsic Semantics of Information

Optional: Structurally Complex Materials, Information Thermodynamics, CA Computational Mechanics, Rate Distortion Theory, Computation at Phase Transitions, Quantum Information & Dynamics, Evolution and Self-Organization

### The Prediction Game
Central questions: What are the states? What is the dynamic?
- Rules: Given data stream (observed past), predict future, give model (states & transitions)

### Effective States = Partitions of History Space
- Histories leading to same predictions are equivalent
- η: ←S → R maps histories to partition elements
- Effective prediction error: hμ(R) = H[→S₁|R]
- Data Processing Inequality: hμ(R) ≥ hμ (models can't beat using full histories)

### Causal States (The Key Definition)
**Predictive equivalence relation:**
←s' ~ ←s'' ⟺ Pr(→S|←S=←s') = Pr(→S|←S=←s'')

Causal State = Set of pasts with same future morph
- Sᵢ = {←s' : ←s' ~ ←s}
- Partition of histories: ←S = ∪ᵢ Sᵢ
- Set of causal states: S = ←S/~ = {S₀, S₁, S₂, ...}

### Causal State Dynamic
- Observe symbol s ∈ A
- Transition: Sᵢ →ˢ Sⱼ
- T(s)ᵢⱼ = Pr(Sⱼ, s|Sᵢ)

### The ε-Machine
**M = {S, {T(s), s ∈ A}}**
- A type of hidden Markov model
- Unique start state (condition of total ignorance)
- Recurrent states: the process's intrinsic computation
- Transient states: how one comes to know the process

### Statistical Complexity
Cμ(R) = H[R] = Shannon entropy of state distribution
- Model "size", historical memory used

### Occam's Pool
- Model Space R = space of all partitions
- Word models (histograms): partition by last L symbols
- Causal states: minimal, optimally predictive partition

### CMPy (Computational Mechanics in Python)
- Probability theory, Information theory, Process analysis
- ε-Machine calculations, Statistical inference, Data generation

---

# Lecture 37a Slides: Thermodynamics of Information, Part I
## Guest Lecturer: Alec Boyd

### Thermodynamics Review
Relevant quantities: Energy, Work, Heat, Temperature, Entropy

### Thermodynamic vs Shannon Entropy
- Gibbs: S[Xₜ] = kB Σ Pr(Xₜ=x) ln Pr(Xₜ=x)
- Shannon: H[Xₜ] = −Σ Pr(Xₜ=x) log₂ Pr(Xₜ=x)
- **Connection: S[Xₜ] = kB ln 2 · H[Xₜ]**
- Thermodynamic entropy: measure of disorder
- Shannon entropy: measure of uncertainty/unpredictability

### Laws of Thermodynamics
- 1st Law: Energy conservation (Hamiltonian dynamics)
- 2nd Law: Entropy increases in isolated systems: dS/dt ≥ 0, dH/dt ≥ 0
- Microcanonical ensemble: maximum entropy at fixed energy
- Temperature: 1/T = ∂S/∂E

### Heat Engines
- Carnot efficiency: η ≤ 1 − Tc/Th
- Energy redirected to produce work, constrained by entropy increase

### Thermodynamics of Control
- Control of energy landscape: d⟨E⟩ = ⟨dW⟩ + ⟨dQ⟩
- Dissipated work: ⟨Wdiss⟩ = ⟨W⟩ − ΔFNEQ
- Nonequilibrium free energy: FNEQ = ⟨E[X]⟩ − TS[X]
- **Heat bound: ⟨Q⟩ ≥ kBT ln 2 · ΔH[X]**
- **Work bound: ⟨W⟩ ≥ Δ⟨E[X]⟩ − kBT ln 2 · ΔH[X]**

### Szilard's Information Engine
1. Particle in a box
2. Insert barrier at halfway
3. Measure which side particle lands on
4. Slide barrier away from particle (extracting work)
5. **⟨W⟩ = kBT ln 2** per cycle

### Maxwell's Demon
- Feedback/Control extracts work: ⟨W⟩ = ⟨Q⟩ = kBT ln 2
- ΔH[X] = 0 after measurement
- Apparent 2nd law violation: ΔStotal = −kB ln 2 < 0 ???

### Landauer's Principle (Resolution)
- **Qerase ≥ kBT ln 2** (minimum heat cost of erasing one bit)
- Erasure restores ΔStotal ≥ 0
- Cost of information processing: work and heat dissipation

### Szilard Engine Cycle (Complete)
Measure → Control → Erase → Repeat
- Extract kBT ln 2 work per cycle
- Pay kBT ln 2 for erasure
- Net: ΔStotal = 0 (exactly calculable via Q = W = −TΔS[X])

---

# Lecture 37b Slides: Thermodynamics of Information, Part II
## Guest Lecturer: Alec Boyd

### Information is a Thermodynamic Fuel
- Instead of erasing, write to a hard drive
- W > 0, Q < 0, ΔShard drive > 0 → ΔStotal ≥ 0

### Information Engines
- Energy and information flow between three reservoirs: Thermal, Work, Information
- Compare to heat engines (Hot Thermal, Cold Thermal, Work)
- **Information reservoir at T = 0, Work reservoir at T = ∞**

### Information Reservoirs
- Bit string where every 0 and 1 have same energy
- Every configuration has equal energy
- Metastable systems with equal energies

### Information Ratchet (Mandal & Jarzynski)
- Autonomous Maxwellian demon
- HMM Input Generator with bias b
- Ratchet interaction: joint Markov transition M
- **Work per step: ⟨W⟩ = kBT ln 2** (for pure input)

### Transducers: Paradigm for Information Processing
Input HMM → Transducer → Output HMM
- Memoryful channel with hidden states
- State-to-state transitions with input/output symbols

### Thermodynamics of Transducers
- Work invested bounded by non-equilibrium free energy
- **Asymptotic: ⟨W⟩ ≥ kBT ln 2 · (hμ − h'μ)** (difference in entropy rates)
- Work cost determined by difference between input and output process randomness

### Key Concepts
1. Information Processing Second Law
2. Thermodynamic Functionality: Engines vs Erasers
3. Nonequilibrium, Memoryful Ratchets
4. Modularity Dissipation
5. Pattern Extractors & Pattern Generators
6. Physical Computation = Transduction

---

# YOUTUBE CHANNELS
## Physics of Information: https://www.youtube.com/playlist?list=PLruYjYJ_iWUCUqQL-XQdx4E7tp6vm8_ba
## Physics of Computation: https://www.youtube.com/playlist?list=PLruYjYJ_iWUCR4XDjumliTSjATNUwdI3g

---

# MASTER INDEX OF ALL LECTURE PDFs

## PDFs FULLY EXTRACTED (text available above):
1. Lecture1Slides.pdf — Overview
2. Lecture14Slides.pdf — Entropies
3. Lecture21Slides.pdf — What's Wrong with Info Theory
4. Lecture22Slides.pdf — The Learning Channel / ε-Machines
5. Lecture37aSlides.pdf — Thermodynamics of Information Part I
6. Lecture37bSlides.pdf — Thermodynamics of Information Part II

## PDFs NOT YET EXTRACTED (available at source URLs):
- Lecture2Slides.pdf — The Big Picture
- Lecture3Slides.pdf — Example Dynamical Systems
- Lecture4Slides.pdf — Bifurcations I
- Lecture5Slides.pdf — Bifurcations II
- Lecture6Slides.pdf — Mechanism of Chaos
- Lecture7Slides.pdf — Example Chaotic Maps
- Lecture8Slides.pdf — Pattern Formation
- Lecture10Slides.pdf — Probability Theory of Dynamical Systems
- Lecture11Slides.pdf — Stochastic Processes
- Lecture12Slides.pdf — Measurement Theory I
- Lecture13Slides.pdf — Measurement Theory II
- Lecture15Slides.pdf — Information in Processes I
- Lecture16Slides.pdf — Information in Processes II
- Lecture17Slides.pdf — Memory in Processes I
- Lecture18Slides.pdf — Memory in Processes II
- Lecture19Slides.pdf — Information Measures & I-Diagrams
- Lecture20Slides.pdf — Anatomy of a Bit
- Lecture23Slides.pdf — ε-Machine Reconstruction
- Lecture24Slides.pdf — ε-Machine Optimalities
- Lecture25Slides.pdf — Measures of Structural Complexity
- Lecture26Slides.pdf — Information Diagrams for Processes
- Lecture27Slides.pdf — States of States of Knowledge I
- Lecture28Slides.pdf — States of States of Knowledge II
- Lecture29Slides.pdf — Directional Computational Mechanics I
- Lecture30Slides.pdf — Directional Computational Mechanics II
- Lecture31Slides.pdf — Markov & Cryptic Orders
- Lecture32Slides.pdf — Role of Future in Chaotic Systems
- Lecture33Slides.pdf — Bayesian Inference for Known Models
- Lecture34Slides.pdf — Bayesian Structural Inference
- Lecture35Slides.pdf — Power Spectra & ε-Machine Spectral Reconstruction
- Lecture36Slides.pdf — Intrinsic Computation in Complex Materials
- Lecture41Slides2015.pdf — Spectral Methods I
- Lecture42Slides.pdf — Spectral Methods II
- Lecture50Slides.pdf — Quantum Complexity I
- Lecture51Slides.pdf — Quantum Complexity II
- LastLectureSlides.pdf — What We Didn't Cover
- POCILecture_0520.pdf — Infinite-State ε-Machines I
- POCILecture_0522.pdf — Infinite-State ε-Machines II
- Jurgens.9jan24.POCILecture.pdf — Alex Jurgens guest lecture

---

*All materials © James P. Crutchfield 2006-2025*
*Source: https://csc.ucdavis.edu/~chaos/courses/poci/Lectures/*
