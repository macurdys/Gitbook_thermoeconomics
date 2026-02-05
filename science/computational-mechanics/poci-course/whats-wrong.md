# What's Wrong with Information Theory?

**Lecture 21** — The opening lecture of Physics of Computation (256B).
📺 [Watch on YouTube](https://www.youtube.com/watch?v=NxV-Xqn9JFQ)
📄 Reading: CMR articles RURO (Intro), CAO, ROIC

---

## The Entropy Hierarchy (Review)

256A built the full information-theoretic toolkit for processes:

| Level | Quantity | What it measures |
|-------|----------|-----------------|
| 0 | Block entropy H(L) | Total uncertainty in L-length blocks |
| 1 | Entropy rate hμ(L) = ΔH(L) | Per-step randomness (converges to hμ) |
| 2 | Predictability gain Δ²H(L) | Memory at each scale |
| ∞ | Excess entropy E = Σ[hμ(L) − hμ] | Total apparent stored information |
| ∞ | Transient information T = Σ[E + hμL − H(L)] | Total synchronization cost |

### Regularities Unseen, Randomness Observed

If you ignore a process's memory (assume E = 0), you overestimate its randomness. Structure gets converted into apparent noise. The gap between the assumed entropy rate and the true rate is the _excess entropy_ — the information the process stores internally.

---

## The Inadequacy

Shannon information theory answers: **how much?**
- How much randomness? (hμ)
- How much memory? (E)
- How much can be compressed? (R = log₂|A| − hμ)

It never answers: **what kind?**

Two processes with identical entropy rates, identical excess entropies, identical transient information can have _completely different_ internal structures. Information theory cannot distinguish them.

### What's missing:
- What does the information _mean_?
- What are the hidden _states_?
- What are the _equations of motion_?
- Is there a principled way to discover them?
- What are cause and effect?

---

## The 256B Program

Computational mechanics answers all of these:

| Question | Answer |
|----------|--------|
| What are the states? | Causal states (predictive equivalence classes) |
| What is the dynamic? | ε-machine transitions |
| Is it principled? | Yes — unique, minimal, optimally predictive |
| What does information mean? | The intrinsic computation of the process |
| What are cause and effect? | Forward and reverse ε-machines, causal irreversibility |

The main idea, restated:

> **Structure = Information + Computation**
>
> How nature is structured is how nature computes.

---

_Next: [The Learning Channel](learning-channel.md) — where the actual construction begins._

