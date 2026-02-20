# Key Equations

All the important equations in thermoeconomics, in one place. Reference sheet for humans and AI tutors.

---

## Information Theory

### Shannon Entropy
$$H(X) = -\sum_{i} p(x_i) \log_2 p(x_i)$$

Average information content of a random variable X. Measured in bits. Maximum when all outcomes are equally likely (uniform distribution). Zero when the outcome is certain.

**In thermoeconomics:** Measures the information content of a valid block hash. A hash at difficulty D carries approximately log₂(D) bits.

---

### Joint Entropy
$$H(X,Y) = -\sum_{x,y} p(x,y) \log_2 p(x,y)$$

Total uncertainty in X and Y together.

### Conditional Entropy
$$H(X|Y) = H(X,Y) - H(Y)$$

Remaining uncertainty about X after observing Y.

### Mutual Information
$$I(X;Y) = H(X) - H(X|Y) = H(X) + H(Y) - H(X,Y)$$

Information shared between X and Y. How much knowing one tells you about the other.

### KL Divergence
$$D_{KL}(P \| Q) = \sum_x p(x) \log_2 \frac{p(x)}{q(x)}$$

Information cost of approximating distribution P with distribution Q. Not symmetric.

---

## Thermodynamics

### Landauer's Principle
$$E_{erase} \geq k_B T \ln 2$$

Minimum energy to erase one bit of information. At room temperature (T = 300K): approximately 2.85 × 10⁻²¹ joules.

**In thermoeconomics:** The fundamental physical cost floor for proof of work. Every hash involves irreversible bit erasure.

---

### Boltzmann Entropy
$$S = k_B \ln \Omega$$

Thermodynamic entropy. Ω is the number of microstates consistent with the macrostate. kB is Boltzmann's constant (1.38 × 10⁻²³ J/K).

### Free Energy (Helmholtz)
$$F = E - TS$$

Energy available to do work. E is total energy, T is temperature, S is entropy.

**In thermoeconomics:** Qi represents the free energy supplied to the system.

---

### Boltzmann Distribution
$$P(\text{state}) = \frac{1}{Z} e^{-E/k_B T}$$

Probability of a state in thermal equilibrium. Z is the partition function. This is the MaxEnt distribution subject to a constraint on average energy.

### Partition Function
$$Z = \sum_{\text{states}} e^{-E/k_B T}$$

Normalizing constant for the Boltzmann distribution. Contains all thermodynamic information about the system.

---

## Proof of Work

### Mining as Bernoulli Trial
$$P(\text{valid hash}) = \frac{1}{2^d}$$

Each hash attempt has probability 1/2^d of producing a valid block at difficulty d. These trials are IID (independent and identically distributed).

### Information Content of a Block
$$I(\text{block}) \approx \log_2(D) \text{ bits}$$

A valid block hash at difficulty D carries approximately log₂(D) bits of information — it represents a selection from an exponentially large candidate space.

### Expected Hashes per Block
$$\langle N \rangle = 2^d$$

Average number of hash attempts to find one valid block at difficulty d.

### Mining Energy (Actual)
$$E_{mining} = N_{hashes} \times E_{per\_hash}$$

where E_per_hash depends on hardware (currently ~10⁻⁸ J for an ASIC, vs. ~10⁻¹⁸ J Landauer minimum per logical operation).

---

## Computational Mechanics

### Statistical Complexity
$$C_\mu = H(\text{causal states}) = -\sum_s p(s) \log_2 p(s)$$

Shannon entropy of the causal state distribution in an epsilon machine. Measures the memory a system uses.

- Cμ = 0 for perfectly random (IID) processes
- Cμ = 0 for perfectly periodic processes
- Cμ is maximized at the "edge of chaos"

---

## Active Inference

### Variational Free Energy
$$F = D_{KL}[q(\theta) \| p(\theta|d)] - \ln p(d)$$

Upper bound on surprise. Self-organizing systems minimize this quantity (Friston).

---

## Thermoeconomic Operator

### Generalized Boltzmann Distribution
$$P(x) = \frac{1}{Z} e^{-\beta E(x)}$$

The unique distribution where Gibbs-Shannon entropy equals thermodynamic entropy. Derived from Jaynes' MaxEnt applied to hash-based Bernoulli trials.

### kQuai Controller
$$k_{Quai}(i) = k_{Quai}(i-1) \times [1 \pm r]$$

Balances miner demand between Qi and Quai tokens. Increases when miners prefer Qi; decreases when they prefer Quai.

---

## Constants

| Symbol | Name | Value |
|---|---|---|
| kB | Boltzmann constant | 1.381 × 10⁻²³ J/K |
| kBT ln 2 (300K) | Landauer limit at room temp | 2.85 × 10⁻²¹ J |
| ln 2 | Natural log of 2 | 0.693 |
| log₂(e) | For converting nats to bits | 1.443 |
