# Information Theory

Information theory is the mathematical foundation of thermoeconomics. It establishes that information is not abstract — it is physical, measurable, and subject to thermodynamic law.

Four papers define the core:

---

## The Lineage

**Shannon (1948)** defined information mathematically as entropy — the reduction of uncertainty. This gave us bits, channel capacity, and the entire framework for quantifying what a message *says*.

**Jaynes (1957)** showed that the entropy in statistical mechanics and the entropy in information theory are the same thing. Maximum entropy is not a physical law but a principle of inference — you should assign probabilities that maximize entropy subject to known constraints. This unified physics and probability theory.

**Landauer (1961)** proved that erasing one bit of information requires a minimum energy dissipation of *kT* ln 2. Information is not free. Computation has thermodynamic cost. This is the bridge between Shannon's abstract bits and the real energy consumed by computers and miners.

**Bennett (1982)** showed that computation itself can be thermodynamically reversible — it is specifically the *erasure* of information (the irreversible step) that generates heat. This clarifies exactly where the thermodynamic cost lives in any computational process, including proof of work.

---

## Why This Matters for Thermoeconomics

Every Bitcoin block header is a 80-byte message. Finding a valid nonce requires erasing astronomical numbers of failed candidates. Each erasure dissipates energy (Landauer). The surviving hash is the information created (Shannon). The difficulty adjustment ensures this information has maximum entropy subject to the protocol's constraints (Jaynes). The entire process is thermodynamically irreversible by design (Bennett).

Proof of work is applied information theory.
