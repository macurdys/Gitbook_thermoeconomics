# Bennett (1982) — The Thermodynamics of Computation: A Review

> **Paper:** Charles H. Bennett, "The Thermodynamics of Computation — A Review," *International Journal of Theoretical Physics*, Vol. 21, No. 12, pp. 905–940, 1982.
>
> **DOI:** [10.1007/BF02084158](https://doi.org/10.1007/BF02084158)

## Summary

Bennett extended Landauer's work to show that *computation itself* can be thermodynamically reversible — it is specifically the *erasure* of information that generates heat. A logically reversible computation (one-to-one mapping from input to output) can in principle be performed with arbitrarily little energy dissipation. Only when information must be discarded does the Landauer cost apply.

## Key Concepts

**Reversible computation:** Any computation can be made logically reversible by keeping a record of intermediate steps. This record can later be "uncomputed" to recover the input, leaving no net entropy increase.

**The cost of forgetting:** The thermodynamic cost of computation comes not from the computing but from the cleanup — erasing the scratch work. This is a profound clarification of where irreversibility lives.

**Maxwell's Demon resolved:** Bennett showed that Maxwell's Demon doesn't violate the second law because the demon must erase its memory of which molecules it sorted, and this erasure dissipates at least as much entropy as was reduced by the sorting.

## Connection to Thermoeconomics

Proof-of-work mining is *deliberately irreversible* computation. The protocol does not merely tolerate the thermodynamic cost — it *requires* it. A miner cannot reversibly "uncompute" a failed nonce attempt; the failed attempt must be discarded and a new one tried. This forced erasure is what makes the work *proof* — it creates a physical record (energy dissipated, entropy produced) that cannot be faked.

Bennett's framework makes precise exactly what proof of work proves: that a certain quantity of logically irreversible computation — and therefore a certain quantity of thermodynamic dissipation — has occurred.

## Further Reading

- Landauer (1961) — the predecessor paper
- Zurek, "Algorithmic Randomness and Physical Entropy" (1989)
- Feynman, *Lectures on Computation* (1996), Chapter 5
