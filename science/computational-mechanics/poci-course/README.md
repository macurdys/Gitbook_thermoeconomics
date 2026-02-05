# Crutchfield's Physics of Information & Computation

**Course:** Physics 256A+B, UC Davis
**Instructor:** Jim Crutchfield, Director, Complexity Sciences Center
**Source:** [csc.ucdavis.edu/~chaos/courses/poci](http://csc.ucdavis.edu/~chaos/courses/poci/)

---

This is the foundational graduate course in computational mechanics — the mathematical framework that connects information theory, dynamical systems, and intrinsic computation. It is the theoretical backbone of thermoeconomics.

The course runs in two parts across two quarters:

**Part I — Physics of Information (256A, Winter)**
Dynamical systems, chaos, measurement theory, Shannon entropy, entropy rates, excess entropy, and the full information hierarchy. Establishes _what_ information is in physical systems and _how much_ of it there is.

**Part II — Physics of Computation (256B, Spring)**
Causal states, ε-machines, structural complexity, irreversibility, crypticity, directional computational mechanics, Bayesian inference, information thermodynamics. Establishes _what the information means_ — the structure, the states, the computation.

The central thesis, stated plainly:

> **Structure = Information + Computation.**
> **How nature is structured is how nature computes.**

---

## Why This Matters for Thermoeconomics

Crutchfield's framework answers the question Shannon never asked: _what is the structure of the information a process produces?_ Shannon tells you _how much_ randomness. Computational mechanics tells you _what kind_ of organization sits behind that randomness.

For proof-of-work systems, this is the missing link. A blockchain is a process that converts energy into structured information. The ε-machine formalism gives you the tools to quantify that structure — the causal states, the statistical complexity, the excess entropy — and connect them directly to thermodynamic costs via the Information Processing Second Law.

---

## Course Map

### Part I: Physics of Information

| # | Topic | Video | Key Concepts |
|---|-------|-------|-------------|
| 1 | [Overview](overview.md) | [YouTube](https://youtu.be/knjDJ5nyxtY) | Information ≠ Energy, deterministic chaos, pattern discovery |
| 2 | The Big Picture | [YouTube](https://youtu.be/nnaq5eyoAGk) | State space, flows, attractors, basins |
| 3 | Example Dynamical Systems | [YouTube](https://youtu.be/K9rkMfO17_A) | ODEs, Lorenz, Poincaré maps |
| 4 | Bifurcations I | [YouTube](https://youtu.be/7Q59SpXA_Qs) | Saddle node, transcritical, pitchfork, catastrophe theory |
| 5 | Bifurcations II | [YouTube](https://youtu.be/Ry3F2E3ul_M) | Hopf, period-doubling, routes to chaos |
| 6 | Mechanism of Chaos | [YouTube](https://youtu.be/OIeR-pFYs6w) | Stretch-and-fold, Lyapunov exponents, chaos defined |
| 7 | Chaotic Maps | [YouTube](https://youtu.be/a3jKP0QHP_U) | Shift map, tent map, logistic map, renormalization |
| 8 | Pattern Formation | [YouTube](https://youtu.be/-QXGsS4n17w) | Cellular automata, map lattices |
| 10 | Probability Theory of Dynamical Systems | [YouTube](https://youtu.be/MJK8R_FfFlY) | Evolution of distributions, invariant measures |
| 11 | Stochastic Processes | [YouTube](https://youtu.be/J6qPU70ESmo) | Markov chains, HMMs, Golden Mean process |
| 12 | Measurement Theory I | [YouTube](https://youtu.be/x0iofsbV8iY) | State-space partitioning, Markov partitions |
| 13 | Measurement Theory II | [YouTube](https://youtu.be/4yY7gNPa_mE) | Generating partitions, 2D cat map |
| 14 | [Entropies](entropies.md) | [YouTube](https://youtu.be/Ys2XCfrmDHY) | Shannon entropy, joint/conditional, mutual information, KL divergence |
| 15 | Information in Processes I | [YouTube](https://youtu.be/R5BFYmjZyKQ) | Channels, codes, Kraft inequality, channel capacity |
| 16 | Information in Processes II | [YouTube](https://youtu.be/N6WQFgqeV34) | Entropy rates, ergodicity, metric entropy |
| 17 | Memory in Processes I | [YouTube](https://youtu.be/SGZSdEckaWY) | Entropy convergence, excess entropy, predictability |
| 18 | Memory in Processes II | [YouTube](https://youtu.be/5HW2KuMfwGA) | Finitary/infinitary processes, transient information |
| 19 | Information Diagrams | [YouTube](https://youtu.be/KWJpvmX5_yQ) | I-diagrams, negative mutual information, multivariate |
| 20 | Anatomy of a Bit | [YouTube](https://youtu.be/htsQui1oP7k) | Ephemeral/bound information, entropy rate decomposition |

### Part II: Physics of Computation

| # | Topic | Video | Key Concepts |
|---|-------|-------|-------------|
| 21 | [What's Wrong with Information Theory?](whats-wrong.md) | [YouTube](https://www.youtube.com/watch?v=NxV-Xqn9JFQ) | Inadequacy of Shannon, entropy hierarchy review |
| 22 | [The Learning Channel](learning-channel.md) | [YouTube](https://www.youtube.com/watch?v=GwLrDSCZUTA) | Causal states, predictive equivalence, ε-machines |
| 23 | ε-Machine Reconstruction | [YouTube](https://www.youtube.com/watch?v=PD3ntQv5chM) | Constructing ε-machines from processes |
| 24 | ε-Machine Optimalities | [YouTube](https://www.youtube.com/watch?v=L00HZkooGVI) | Optimal prediction, minimality, uniqueness |
| 25 | Measures of Structural Complexity | [YouTube](https://www.youtube.com/watch?v=B8DIMaHin3g) | Statistical complexity, excess entropy, bounds |
| 26 | Information Diagrams for Processes | [YouTube](https://www.youtube.com/watch?v=dfv7V6Ddb_8) | Causal irreversibility, the mystery wedge |
| 27 | States of States of Knowledge I | [YouTube](https://www.youtube.com/watch?v=K0FsKILsYy8) | Mixed-state presentations, unifilarity |
| 28 | States of States of Knowledge II | [YouTube](https://www.youtube.com/watch?v=lM_R0kYw_1M) | Block entropies, synchronization information |
| 29 | Directional Computational Mechanics I | [YouTube](https://www.youtube.com/watch?v=FCiA2PgzcJs) | Forward/reverse ε-machines, causal irreversibility |
| 30 | Directional Computational Mechanics II | [YouTube](https://www.youtube.com/watch?v=Fh8z9sXs0Vo) | Bidirectional machines, crypticity |
| 31 | Markov & Cryptic Orders | [YouTube](https://www.youtube.com/watch?v=f854MWoQ-B4) | Length scales, synchronizing words _(Ryan James)_ |
| 32 | Role of the Future in Chaotic Systems | [YouTube](https://www.youtube.com/watch?v=AKQlB9jYNt4) | Entropy rate decomposition _(Ryan James)_ |
| 33 | Bayesian Inference for Known Models | [YouTube](https://www.youtube.com/watch?v=soiGUZAngC4) | Bayesian ε-machine inference _(Chris Strelioff)_ |
| 34 | Bayesian Structural Inference | [YouTube](https://www.youtube.com/watch?v=JMfIa4H9idk) | Model topology inference _(Chris Strelioff)_ |
| 35 | Complex Materials I | [YouTube](https://www.youtube.com/watch?v=dvcrB1I4z58) | Power spectra, spectral reconstruction _(Dowman Varn)_ |
| 36 | Complex Materials II | [YouTube](https://www.youtube.com/watch?v=UfxPTzMA9KM) | Zinc-sulfide, intrinsic computation _(Dowman Varn)_ |
| 37a | [Information Thermodynamics I](info-thermo-1.md) | [YouTube](https://www.youtube.com/watch?v=5OTRxg2M2cg) | Szilard engine, Maxwell's demon, Landauer _(Alec Boyd)_ |
| 37b | [Information Thermodynamics II](info-thermo-2.md) | [YouTube](https://www.youtube.com/watch?v=QFZdJLo_LpE) | Info ratchets, transducers, Info Processing 2nd Law _(Alec Boyd)_ |
| 41 | Spectral Methods I | [YouTube](https://www.youtube.com/watch?v=cr3TDYWMNzU) | Eigenvalues, Perron-Frobenius _(Paul Riechers)_ |
| 42 | Spectral Methods II | [YouTube](https://www.youtube.com/watch?v=5mEb4wdydEg) | Exact complexities, spectral decomposition _(Paul Riechers)_ |
| — | Last Lecture | [YouTube](https://www.youtube.com/watch?v=tVncNx54WhE) | What we didn't cover, research directions |

---

## Playlists

- **Physics of Information** — [YouTube Playlist](https://www.youtube.com/playlist?list=PLruYjYJ_iWUCUqQL-XQdx4E7tp6vm8_ba)
- **Physics of Computation** — [YouTube Playlist](https://www.youtube.com/playlist?list=PLruYjYJ_iWUCR4XDjumliTSjATNUwdI3g)

## Textbooks

- **[NDAC]** _Nonlinear Dynamics and Chaos_, Strogatz, 2nd Ed (2015)
- **[EIT]** _Elements of Information Theory_, Cover & Thomas, 2nd Ed (2006)
- **[CMR]** Computational Mechanics Reader (articles on [course website](http://csc.ucdavis.edu/~chaos/courses/poci/Readings/Readings.html))

---

_All course materials © James P. Crutchfield 2006-2025_

