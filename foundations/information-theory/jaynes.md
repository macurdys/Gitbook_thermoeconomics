# Jaynes (1957) — Maximum Entropy Principle

> **Paper:** Edwin T. Jaynes, "Information Theory and Statistical Mechanics," *Physical Review*, Vol. 106, No. 4, pp. 620–630, May 1957.
>
> **PDF:** [bayes.wustl.edu](https://bayes.wustl.edu/etj/articles/brandeis.pdf)

## Summary

Jaynes demonstrated that statistical mechanics — the physics of systems with many particles — is best understood as a form of statistical inference. The probability distributions of thermodynamics (Boltzmann, Gibbs) are not physical laws but the *maximally uninformative* distributions consistent with known macroscopic constraints (energy, volume, particle number).

## Key Concepts

**Maximum Entropy Principle:** When making inferences under incomplete information, assign the probability distribution that maximizes Shannon entropy subject to known constraints. This is the *least biased* choice — it introduces no information beyond what is actually known.

**Unification of Entropies:** The Shannon entropy of information theory and the Gibbs entropy of statistical mechanics are the same quantity applied in different contexts. This is not analogy — it is identity.

**Constraints as Information:** What we know about a system is expressed as constraints. What we don't know is expressed as entropy. The maximum entropy distribution is the honest answer to "what do we expect, given only what we know?"

## Connection to Thermoeconomics

The proof-of-work difficulty adjustment is a maximum entropy mechanism. It constrains the rate of block production (one block per target interval) while leaving the specific hash values maximally random — maximum entropy subject to the difficulty constraint. Miners collectively sample the nonce space, and the protocol accepts only results that satisfy the constraint. This is Jaynes' principle instantiated in hardware.

## Further Reading

- Jaynes, *Probability Theory: The Logic of Science* (posthumous textbook, 2003)
- [Wikipedia: Maximum Entropy Principle](https://en.wikipedia.org/wiki/Principle_of_maximum_entropy)
