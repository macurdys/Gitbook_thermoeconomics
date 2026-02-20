# Crutchfield POCI Course — Complete Lecture Outlines
## Physics of Information (256A) & Physics of Computation (256B)
### UC Davis — Jim Crutchfield
#### Source: https://csc.ucdavis.edu/~chaos/courses/poci/Lectures/

---

# PART I: PHYSICS OF INFORMATION (256A, Winter)

---

## Lecture 1: Overview

Readings: Chaos (Crutchfield, Farmer, Packard, Shaw, SciAm 1986); Odds (Stanislaw Lem, New Yorker 1978)

Topics:
1. Introduction and motivations
   1. The Industrial Age and the development of thermodynamics
   2. The Information Age and what?
   3. Information ≠ energy
   4. Deterministic chaos — Nature actively produces information
   5. What is randomness? Where does it come from?
   6. Pattern discovery (versus pattern recognition)
   7. Causality
   8. Logic of the course:
      1. Complex systems: order and chaos
      2. Self-organization: emergence of complexity
      3. Natural computation: how nature stores and processes information
   9. Goals:
      1. You can quantify unpredictability
      2. You can quantify structure
      3. These both are related to computation
   10. Applications: Novel Computation, Nanotechnology, Automated scientific inference
2. Class survey: Interests, background, and abilities
3. Course logistics
4. Homework, exam, and project
5. Software tools and program development

---

## Lecture 2: The Big Picture

Reading: NDAC, Chapters 1 and 2.

Topics:
1. Discuss Chaos and Odds readings and homework
2. Pendulum demo
3. Qualitative Dynamics: A geometric view of behavior
4. State space
5. Dynamic
6. Flows
7. Attractors
8. Basins
9. Submanifolds
10. Concrete, but simple example: One-dimensional flows

---

## Lecture 3: Example Dynamical Systems

Reading: NDAC, Sections 6.0-6.4, 7.0-7.3, and 9.0-9.4.

Topics:
1. Review last lecture.
2. Continuous-time ODEs
   1. 1D Flows: Fixed points and their stability (Ch. 2)
   2. 2D Flows: Fixed points and their stability (Sec. 6.0-6.4) (eigensystems)
   3. 2D Flows: Limit cycles (Sec. 7.0-7.3)
   4. 3D Flows: Chaos in Lorenz (Sec. 9.0-9.4)
   5. Simulation Demo
3. From continuous to discrete time (Sec. 9.4)
   1. Poincaré Maps and Sections
   2. Lorenz ODE to Cusp Map
   3. Rössler ODE to Logistic Map (pp. 376–379)
   4. Discrete-time Maps

---

## Lecture 4: The Big, Big Picture (Bifurcations) I

Reading: NDAC, Chapter 3

Topics:
1. Qualitative dynamics: Space of all dynamical systems
2. Example: Bifurcations of one-dimensional flows
   1. Saddle node
   2. Transcritical
   3. Pitchfork
3. Catastrophe theory
   1. Catastrophes: Fixed point to fixed point bifurcation
   2. Example: Cusp Catastrophe
   3. Catastrophe theory classification of fixed point bifurcations

---

## Lecture 5: The Big, Big Picture (Bifurcations) II

Reading: NDAC, Chapter 8 and Sec. 10.0-10.4.

Topics:
1. Review last lecture.
2. Bifurcations in ODEs (Simulation demos):
   1. Hopf bifurcation
   2. Limit cycle to torus
   3. Torus to chaos
   4. Chaos to chaos
   5. Period-doubling route to chaos
3. Return maps return
4. Logistic map
5. Fixed point to limit cycle
6. Phenomenon and calculation
7. Limit cycle to limit cycle
8. Phenomenon and calculation
9. Routes to chaos: Period-doubling cascade
10. Phenomenon and calculation
11. Band-merging
12. Periodic windows and intermittency

---

## Lecture 6: Mechanism of Chaos: Stable Instability

Reading: NDAC, Sec. 12.0-12.3, 9.3, and 10.5.

Topics:
1. Review last lecture.
2. Chaotic mechanisms: Stretch and fold
3. Baker's map
4. Cat map (and stretch demo)
5. Henon map: stretch-fold and self-similarity
6. Roessler attractor branched manifold
7. Dot spreading: Roessler and Lorenz ODEs
8. Lyapunov characteristic exponents (LCEs)
9. Time to unpredictability
10. Dissipation rate
11. Attractor LCE classification
12. Chaos defined

---

## Lecture 7: Example Chaotic Maps (that you can analyze)

Reading: NDAC, Sections 10.5-10.7.

Topics:
1. Review last lecture.
2. Shift Map
3. LCEs for Maps
4. Tent Map
5. Logistic Map
6. LCE view of period-doubling route to chaos
7. Period-doubling self-similarity
8. Renormalization group analysis of scaling

---

## Lecture 8: Pattern Formation I (Deterministic)

Reading: Lecture Notes.

Topics:
1. Review last lecture.
2. Deterministic spatially extended dynamical systems
   1. How to make
   2. State space
   3. What does dynamical systems have to say?
3. Cellular Automata
   1. Definitions
   2. Mathematical properties
   3. 1D CAs
   4. Behavior Survey
   5. Simulation examples
4. Nonlinear Map Lattices
   1. Definitions
   2. Mathematical properties
   3. 1D LDSs
   4. Simulation examples
   5. Period-doubling?
   6. Quasi-periodicity

---

## Lecture 10: Probability Theory of Dynamical Systems

Reading: Lecture Notes.

Topics:
1. Review last lecture.
2. Probability theory review
3. Dynamical evolution of distributions
4. Invariant measures
5. Examples

---

## Lecture 11: Stochastic Processes

Reading: Lecture Notes.

Topics:
1. Review last lecture.
2. Processes: Markov, Order-R, Block
3. Markov chains
4. Statistical equilibrium
5. Hidden Markov processes
6. Examples: Fair coin, Periodic, Multi-Recurrent, Golden Mean, Even Processes

---

## Lecture 12: Measurement Theory I

Reading: Lecture Notes.

Topics:
1. Review last lecture.
2. State-space partitioning
3. Orbit and sequence spaces
4. Good instruments and informative measurements
5. Markov partitions in 1D

---

## Lecture 13: Measurement Theory II

Reading: Lecture Notes.

Topics:
1. Review last lecture.
2. Markov partitions in 2D
3. Example: 2D Cat map
4. Generating partitions in 1D
5. Example: 1D maps
6. Non-generating partitions in 1D
7. Almost generating partitions in 2D
8. General partitions and problems

---

## Lecture 14: Entropies

Reading: EIT, Chapters 1 and 2.

Topics:
1. Review last lecture.
2. Motivation: Information ≠ Energy
3. Probability theory review
4. Information as uncertainty and surprise
5. Information sources: Ignorance of forces or initial conditions, deterministic chaos, and ...?
6. Axioms for a measure of information
7. Entropy function
8. Convexity
9. Joint and Conditional Entropy
10. Mutual information
11. Examples

---

## Lecture 15: Information in Processes I

Reading: EIT, Sec. 5-5.4 and 7.1-7.7.

Topics:
1. Review last lecture.
2. Communication channels
3. Codes
4. Kraft Inequality
5. Data Compression Theorem
6. Redundancy
7. Noisy Channels
8. Equivocation
9. Channel Capacity
10. Channel Coding Theorem

---

## Lecture 16: Information in Processes II

Reading: EIT Chapter 4.

Topics:
1. Entropies for time series
2. Entropy growth
3. Entropy rates for Markov chains
4. Connection to dynamics
   1. Partitioning revisited
   2. Ergodicity and mixing
   3. Metric and topological entropies
   4. Entropy rate and LCEs

---

## Lecture 17: Memory in Processes I

Reading: CMR article RURO.

Topics:
1. Review last lecture.
2. Entropy convergence
3. Process redundancy
4. Predictability gain
5. Total predictability
6. Excess entropy
7. Examples

---

## Lecture 18: Memory in Processes II

Reading: CMR article RURO.

Topics:
1. Classes of excess entropy
2. Finitary and infinitary processes
3. Non-Markov case: Even Process
4. Infinitary examples: Morse-Thue and Simple Nonunifilar Source
5. Generalized synchronization
6. Transient information
7. Examples
8. Disorder as the price of ignorance
9. Predictability and instantaneous synchronization
10. Assumed synchronization implies reduced apparent memory
11. The Entropy hierarchy

---

## Lecture 19: Information Measures and Information Diagrams

Reading: CMR articles Yeung and Anatomy.

Topics:
1. Recall One- and Two-Variable Informations
2. Algebra of Shannon Information Measures
3. Information Diagrams
4. Process I-Diagram
5. Three random variables
6. Negative Mutual Information
7. Multivariate Mutual Informations
8. Multivariate Informations

---

## Lecture 20: Anatomy of a Bit

Reading: CMR articles Yeung and Anatomy.

Topics:
1. Past, Present, and Future: I-diagrams
2. New measures: Ephemeral, Bound, ...
3. Alternative Decompositions
4. Application of Entropy Rate Decomposition: Tent and Logistic Maps
5. Course summary
6. Preview of Physics 256B

---

# PART II: PHYSICS OF COMPUTATION (256B, Spring)

---

## Lecture 21: What's Wrong with Information Theory?

Readings: CMR articles Chance and Order (Lem, New Yorker 1984), Revealing Order in the Chaos (Buchanan, New Scientist 2005), RURO (Intro), CAO, ROIC.

Topics:
1. Recall Physics 256A
2. Introduction and motivations
3. Inadequacy of Information Theory
4. Structure and Learning
5. Survey interests, background, and abilities
6. Course logistics
7. CMPy Labs
8. Projects
9. Software and program development

---

## Lecture 22: The Learning Channel

Reading: CMR articles RURO (Intro), BOAC, CMPPSS (first sections).

Topics:
1. Review last lecture.
2. The Learning Channel
3. The Prediction Game
4. Space of histories
5. Predictive equivalence relation
6. Causal States
7. Causal State Transitions
8. ε-Machines
9. CMPy — Computational Mechanics in Python

---

## Lecture 23: ε-Machine Reconstruction

Reading: Lecture Notes.

Topics:
1. Review last lecture.
2. Causal states
3. ε-Machines
4. Simple Processes: Predictable (Period-One Process) and Fair and Biased Coins
5. Complex Processes: Period-Two, Golden Mean, and Even Processes

---

## Lecture 24: ε-Machine Optimalities

Reading: CMR article CMPPSS.

Topics:
1. The ε-machine as a Model
2. Optimal Prediction
3. Minimality
4. Uniqueness
5. Minimal Stochasticity
6. Minimal Sufficient Statistic

---

## Lecture 25: Measures of Structural Complexity

Reading: CMR articles CMPPSS and RURO.

Topics:
1. Review last lecture.
2. Entropy rate
3. Statistical complexity
4. Excess entropy
5. Why we must model
6. Bounds
   1. Excess entropy versus statistical complexity
   2. Predictability versus statistical complexity
7. Pattern
8. Measurement semantics

---

## Lecture 26: Information Diagrams for Processes

Reading: CMR articles Yeung, TBA, PRATISP.

Topics:
1. Projects
2. Prediction versus retrodiction
3. Time symmetry
4. Time asymmetry
5. Causal irreversibility
6. Information diagram for processes
7. ε-Machine information diagram for processes
8. Unpredictability
9. The mystery wedge
10. Distance between the past and the future

---

## Lecture 27: States of States of Knowledge I

Reading: CMR articles TBA and Yeung.

Topics:
1. Review
2. Conditional random variables
3. Evolution of internal-state distributions
4. Mixed-state presentations
5. Unifilarity
6. Minimization
7. Transient states
8. Examples
9. From mixed-state presentations to ε-machines
10. Complexity measures
11. Fast calculations of block entropies

---

## Lecture 28: States of States of Knowledge II

Reading: CMR articles TBA, PRATISP, and IACP.

Topics:
1. Review
2. How to calculate mixed states
3. From mixed-state presentations to ε-machines
4. Complexity measures
5. Fast calculations of block entropies
6. Synchronization information

---

## Lecture 29: Directional Computational Mechanics I

Reading: CMR articles TBA, PRATISP, IACP, and IACPLCOCS.

Topics:
1. Forward and reverse processes
2. Forward and reverse computational mechanics
3. Time-reversal symmetric: Predictability
4. Causal irreversibility
5. Information diagram
6. Process lattice
7. Calculating reverse ε-machine given the forward one

---

## Lecture 30: Directional Computational Mechanics II

Reading: CMR articles TBA, PRATISP, IACP, and IACPLCOCS.

Topics:
1. Bidirectionality
2. Excess entropy from ε-machine
3. Forward and reverse crypticities
4. Information diagram for processes using ε-machine
5. Bidirectional machines
6. Bidirectional complexities
7. Summary of generalized computational mechanics

---

## Lecture 31: Length Scales in Complex Time Series: Markov and Cryptic Orders
*Guest Lecturer: Ryan James*

Reading: CMR articles MRS and SAC.

Topics:
1. Background: Processes and ε-machines
2. Definitions
3. Approach 1: Block entropy and block-state entropy
4. Approach 2: Synchronizing words
5. Approach 3: Synchronizing automata
6. Survey of 6-state binary machines

---

## Lecture 32: The Role of the Future in the Analysis of Chaotic Dynamical Systems
*Guest Lecturer: Ryan James*

Reading: CMR article Anatomy.

Topics:
1. Background: What is a process?
2. Dissection of the present
3. Decomposition of the present
4. Computing rates
5. Example decompositions: Logistic, Tent and Lozi maps
6. Scaling behavior in the Tent map
7. Computing the bound information analytically

---

## Lecture 33: Bayesian Inference for Known Model Structures
*Guest Lecturer: Chris Strelioff*

Reading: CMR articles IMC and OIMNC.

Topics:
1. Goals of statistical inference
2. Introduction to Bayesian inference
3. Example 1: Biased Coin
4. Unifilar HMMs and ε-machines
5. Example 2: Even-Odd Process
6. Infer transition probabilities and start state

---

## Lecture 34: Bayesian Methods for Structural Inference
*Guest Lecturer: Chris Strelioff*

Reading: CMR article BSI.

Topics:
1. Inferring structure (aka model topology)
   1. Enumeration and model comparison for topological ε-machines
2. Example 3: Infer structure of EvenOdd process
3. Example 4: Survey of inferring Golden Mean, Even, Simple Nonunifilar Source
4. Complications: Out-of-class, nonstationary processes

---

## Lecture 35: Complex Materials I — Power Spectra and ε-Machine Spectral Reconstruction
*Guest Lecturer: Dowman Varn*

Reading: CMR articles BTFM1 and BTFM2.

Topics:
1. Power spectra
2. ε-Machine spectral reconstruction

---

## Lecture 36: Intrinsic Computation in Complex Materials
*Guest Lecturer: Dowman Varn*

Reading: CMR articles BTFM1 and BTFM2.

Topics:
1. One-Dimensional materials: Physics of polytypes
2. Planar disorder
3. Diffraction Spectra
4. ε-Machine Spectral Reconstruction
5. Fault Structures and Causal State Cycles
6. Zinc-Sulfide
7. Intrinsic Computation

---

## Lecture 37a: Thermodynamics of Information, Part I
*Guest Lecturer: Alec Boyd*

Reading: Lecture Notes.

Topics:
1. Thermodynamics Review
2. Heat Engines
3. Control
4. Particle in a Box
5. Szilard's Engine
6. Maxwell's Demon
7. Cost of Information Processing

---

## Lecture 37b: Thermodynamics of Information, Part II
*Guest Lecturer: Alec Boyd*

Reading: Lecture Notes.

Topics:
1. Information is a Thermodynamic Fuel
2. Information Engines
3. Information Reservoirs
4. Energy Production
5. Information Ratchet
6. Thermodynamics of Transducers
7. Work
8. Thermodynamic Functionality: Engines versus Erasers
9. Nonequilibrium, Memoryful Ratchets
10. Types of Order
11. Physical Computation
12. Modularity Dissipation
13. Pattern Extractors
14. Pattern Generators
15. Information Processing Second Law

---

## Lecture 41: Spectral Methods for Complex Systems I
*Guest Lecturer: Paul Riechers*

Reading: CMR article EC.

Topics:
1. Visualizing Relaxation Modes and Formalizing those Intuitions
2. What to Expect
3. HMMs as Mathematical Objects
4. Motivating Example: Ion Channel Dynamics
5. An Operator and Its Spectrum
6. Eigenvalues and Projection Operators
7. Functions of Square Matrices
8. Restrictions on Eigenvalues: Perron-Frobenius Theorem
9. Autocorrelation Function
10. Power Spectrum
11. Examples

---

## Lecture 42: Spectral Methods for Complex Systems II
*Guest Lecturer: Paul Riechers*

Reading: CMR article EC.

Topics:
1. Review: Processes, Models, Mixed State Presentations
2. Information Measures From MSPs
   1. Word Distributions
   2. Entropy Rates
   3. Statistical Complexity
   4. Synchronization Information
3. Spectral Decomposition of Functions of Nondiagonalizable Dynamics
4. Projection Operators
5. Exact Complexities
   1. Autocorrelation Function and Power Spectra
   2. Finite-Length and Asymptotic Entropy Rates
   3. Excess Entropy
   4. Synchronization Information
   5. Transient Information
6. Diagonalizable and Almost Diagonalizable Dynamics
7. Examples

---

## Lectures 50–51: Quantum Complexity I & II
*Guest Lecturer: John Mahoney*

Reading: CMR articles OQS and EQC.

### Part I Topics:
1. Review of basic quantum mechanics
2. Bloch sphere
3. Generalized measurements
4. How to calculate things

### Part II Topics:
1. Quantum channels
2. Quantum complexity
3. Quantum synchronization
4. Prediction versus generation
5. Quantum compression
6. Ambiguity of simplicity

---

## Infinite-State ε-Machines I & II (Lectures AMJ1 & AMJ2)
*Guest Lecturer: Alex Jurgens*

Reading: CMR article SERHMP.

---

## Last Lecture: What Was Not Covered — The Present and Future

Topics:
1. What was not covered
   1. ε-Machine Enumeration
   2. Infinite ε-Machines and Generalized Hidden Markov Models
   3. Hierarchical ε-Machine Reconstruction
   4. Complex Materials and ε-Machine Spectral Reconstruction
   5. Quantum Processes and Quantum Machines
   6. Rate Distortion Theory and Optimal Causal Inference
   7. Interactive Learning
   8. Cellular Automata Computational Mechanics
   9. Spin Systems in 1D and 2D
   10. Optimal Instrument Design
   11. Complexity-Entropy Diagrams
2. Applications
   1. Chaotic Dynamical Systems
   2. Symbolic Dynamics
   3. Statistical Mechanical Models: Spin systems (Ising, glasses, ...)
   4. Molecular Dynamics
   5. Cellular Automata
   6. Hidden Markov Models
   7. Crystallography
   8. Hydrodynamics: dripping faucet, turbulence
   9. Quantum Dynamical Systems
3. Research Directions
   1. Intrinsic computation
   2. Statistical inference
   3. Quantum chaotic dynamics and measurement effects
   4. Continuous processes
   5. Spatiotemporal processes
   6. Network dynamics
   7. Neurobiological processes
   8. Multiagent systems
   9. Distributed robotics
   10. Evolutionary dynamics
4. Recall course narrative

---

*All materials © James P. Crutchfield 2006-2025*

