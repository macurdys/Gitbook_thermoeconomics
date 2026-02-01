# Back (1997) — Hashcash

> **Paper:** Adam Back, "Hashcash — A Denial of Service Counter-Measure," August 1997, revised 2002.
>
> **URL:** [hashcash.org](http://www.hashcash.org/papers/hashcash.pdf)

## Summary

Hashcash is a proof-of-work system originally designed to combat email spam and denial-of-service attacks. The sender must find a partial hash collision — an input whose SHA-1 hash (later SHA-256) starts with a required number of zero bits. This is computationally expensive to produce but trivial to verify.

## Key Concepts

**Partial hash collision** — The core mechanism. Finding an input *x* such that SHA(x) has *k* leading zeros requires on average 2^*k* hash operations. Verification requires exactly one.

**Asymmetric cost** — The defining property of proof of work: expensive to create, cheap to verify. This asymmetry is what makes the system useful as a cost mechanism.

**Tunable difficulty** — By adjusting the number of required leading zeros, the cost can be set to any desired level. Nakamoto would later make this adjustment automatic via the difficulty algorithm.

## Connection to Thermoeconomics

Hashcash is the direct ancestor of Bitcoin's mining algorithm. It established the core mechanism: brute-force search through a computationally irreducible hash function, with the difficulty of the search as the tunable parameter. The energy cost of this search is the thermodynamic foundation of everything that follows.
