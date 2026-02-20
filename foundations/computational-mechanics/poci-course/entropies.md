# Entropies

**Lecture 14** — The information theory toolkit.
📺 [Watch on YouTube](https://youtu.be/Ys2XCfrmDHY)
📄 Reading: Elements of Information Theory, Chapters 1 & 2

---

## Information ≠ Energy

This is the starting point. Information and energy are two different accountings of the same physical system. They are related (via S = kB ln 2 · H) but they are not the same thing.

Sources of information:
- **Uncontrolled initial conditions** — apparent randomness from ignorance
- **Deterministic chaos** — actively generated randomness from dynamics
- **Hidden regularity** — ignorance of forces or limited modeling capacity

---

## Shannon Entropy

Derived from axioms (Khinchin or Shannon). The unique measure of uncertainty satisfying continuity, maximum at uniform distribution, and additivity for independent systems:

**H(X) = −Σ p(x) log₂ p(x)**

| Property | Statement |
|----------|-----------|
| Positivity | H(X) ≥ 0 |
| Predictable | H(X) = 0 iff one event has probability 1 |
| Maximally random | H(X) = log₂ k iff uniform over k events |

**Interpretation:** The minimum average number of yes/no questions needed to identify the outcome. The optimal compression rate. The degree of surprise.

---

## Joint, Conditional, Mutual

**Joint entropy** — uncertainty in X and Y together:
H(X,Y) = −Σ p(x,y) log₂ p(x,y)

**Conditional entropy** — uncertainty in X, knowing Y:
H(X|Y) = H(X,Y) − H(Y)

**Mutual information** — information shared between X and Y:
I(X;Y) = H(X) − H(X|Y) = H(X) + H(Y) − H(X,Y)

**KL divergence** — information cost of approximating P with Q:
D(P‖Q) = Σ p(x) log₂[p(x)/q(x)]

**Information distance** — a true metric:
d(X,Y) = H(X|Y) + H(Y|X)

---

## The I-Diagram

```
H(Y|X)  |  I(X;Y)  |  H(X|Y)
←—— H(Y) ——→        ←—— H(X) ——→
←————————————— H(X,Y) ——————————————→
```

This diagram encodes all relationships between entropy quantities for two variables. Every information measure is an area in this diagram.

---

## Key Inequalities

- **Conditioning reduces entropy:** H(X|Y) ≤ H(X)
- **Independence bound:** H(X₁,...,Xₙ) ≤ Σ H(Xᵢ)
- **Data Processing Inequality:** X→Y→Z ⇒ I(X;Y) ≥ I(X;Z)

The Data Processing Inequality is fundamental: **manipulation cannot increase information about the source.** No amount of post-processing can recover information lost in transmission.

---

## Chain Rules

**Entropy:** H(X₁,...,Xₙ) = Σ H(Xᵢ | Xᵢ₋₁,...,X₁)

**Mutual Information:** I(X₁,...,Xₙ; Y) = Σ I(Xᵢ; Y | Xᵢ₋₁,...,X₁)

These decompose complex joint quantities into sums of conditional quantities — essential for analyzing sequential processes like blockchain state transitions.

---

_This is the vocabulary. The grammar comes in [Lectures 15-20](README.md), where these measures are applied to stochastic processes._

