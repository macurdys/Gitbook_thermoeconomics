# Shannon (1948) — A Mathematical Theory of Communication

> **Paper:** Claude E. Shannon, "A Mathematical Theory of Communication," *Bell System Technical Journal*, Vol. 27, pp. 379–423, 623–656, July & October 1948.
>
> **PDF:** [bell-labs.com](https://people.math.harvard.edu/~ctm/home/text/others/shannon/entropy/entropy.pdf)

## Summary

Shannon established the mathematical framework for quantifying information. His key insight: information is the *reduction of uncertainty*. A message is informative to the extent that it tells you something you didn't already know.

## Key Concepts

**Entropy (H):** The average information content of a message source, measured in bits. For a source with possible messages of probability *p_i*:

$$H = -\sum p_i \log_2 p_i$$

This is identical in form to Boltzmann-Gibbs entropy in statistical mechanics — a connection that Jaynes would later prove is not coincidental.

**Channel Capacity:** Every communication channel has a maximum rate at which information can be transmitted reliably. Noise sets the limit.

**Source Coding Theorem:** Data can be compressed to a rate approaching its entropy, but no further.

## Connection to Thermoeconomics

Shannon entropy measures the information content of a proof-of-work solution. A valid block hash at difficulty *D* carries approximately log₂(*D*) bits of information — it represents a selection from an exponentially large space of possibilities. The difficulty adjustment ensures that the information produced per block remains constant regardless of total hash power, which is a constraint on entropy production rate.

## Further Reading

- Shannon's original paper (linked above)
- Cover & Thomas, *Elements of Information Theory* (textbook)
- [Wolfram MathWorld: Shannon Entropy](https://mathworld.wolfram.com/Entropy.html)
