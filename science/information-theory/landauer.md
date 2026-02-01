# Landauer (1961) — Irreversibility and Heat Generation in the Computing Process

> **Paper:** Rolf Landauer, "Irreversibility and Heat Generation in the Computing Process," *IBM Journal of Research and Development*, Vol. 5, No. 3, pp. 183–191, July 1961.
>
> **DOI:** [10.1147/rd.53.0183](https://doi.org/10.1147/rd.53.0183)

## Summary

Landauer proved that erasing information has a minimum thermodynamic cost. Specifically, erasing one bit of information at temperature *T* requires dissipating at least *kT* ln 2 joules of energy as heat, where *k* is Boltzmann's constant. This is known as **Landauer's Principle**.

## Key Concepts

**Landauer's Principle:** Information erasure is a logically irreversible operation (many-to-one mapping). By the second law of thermodynamics, this irreversibility must be accompanied by an increase in entropy of the environment — i.e., heat dissipation.

**Minimum energy per bit erasure:** *kT* ln 2 ≈ 2.87 × 10⁻²¹ joules at room temperature (300K).

**Information is physical:** This is perhaps the most important single sentence in thermoeconomics. Information is not abstract — it is encoded in physical states, and manipulating it has physical consequences.

## Connection to Thermoeconomics

Proof-of-work mining is, at its core, a massive information erasure process. Each candidate nonce that fails the difficulty check is computed and discarded — erased. A miner testing 10¹⁸ nonces per second is erasing 10¹⁸ computational states per second, each incurring at minimum the Landauer cost. The actual energy cost of real hardware is many orders of magnitude above the Landauer limit, but the principle establishes the *physical floor* — proof of work cannot be made thermodynamically free.

This is why proof of work creates "unforgeable costliness" (Szabo's phrase). The cost is not arbitrary — it is grounded in physics.

## Further Reading

- Bennett, "The Thermodynamics of Computation — A Review" (1982) — extends Landauer
- Bérut et al., "Experimental verification of Landauer's principle" (2012) — laboratory confirmation
