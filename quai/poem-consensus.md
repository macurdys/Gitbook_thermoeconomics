# Proof of Entropy Minima (PoEM)

> **Paper:** Karl Kreder, "Proof of Entropy Minima," 2023. [arXiv](https://arxiv.org/pdf/2303.04305)

## The Problem with Threshold Difficulty

In Bitcoin, a miner finds a valid block by discovering a hash below a target threshold. Any hash below the threshold counts equally — whether it's 1% below or 99% below. This is **lossy compression**: the system discards information about how far below the threshold the hash fell.

From an information-theoretic perspective, this is wasteful. The miner did the work to find an exceptionally low hash, but the protocol treats it the same as a barely-qualifying one.

## The PoEM Solution

Proof of Entropy Minima ranks every hash output by its absolute distance from zero. Lower hash values represent greater entropy reduction — more information extracted from the hash space per computation.

The block with the lowest hash value wins. Always. No threshold. No wasted information.

### Why This Matters

| Property | Bitcoin (Threshold) | Quai (PoEM) |
|---|---|---|
| Information per hash | Binary (pass/fail) | Continuous (ranked) |
| Surplus work | Discarded | Counted |
| Finality | Probabilistic (6 blocks) | Intrinsic (lower = more final) |
| Forks | Common (equal-threshold blocks) | Rare (ties nearly impossible) |

PoEM achieves **instant finality in the information-theoretic limit**: the probability that a competing block has a lower hash than the current winner decreases exponentially with the magnitude of the hash value.

## Connection to Thermoeconomics

PoEM is the MaxEnt principle (Jaynes) applied to consensus. The difficulty adjustment constrains the rate of entropy reduction. Within that constraint, PoEM selects the block that reduced entropy the most — the maximum information extraction per unit of computation.

This is why Qi emission can be strictly proportional to hash rate: PoEM ensures that all computational work is counted, not just the work above an arbitrary threshold.

## Further Reading

- [The Thermoeconomic Operator](../foundations/synthesis/thermoeconomic-operator.md) — formal framework
- [Jaynes — Maximum Entropy Principle](../foundations/information-theory/jaynes.md) — the physics
- [Shannon — Information Theory](../foundations/information-theory/shannon.md) — information content of a hash
