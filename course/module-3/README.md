# Module 3: Cryptography

The mathematical primitives that make blockchains possible: hash functions, public/private key pairs, digital signatures, and how they compose into secure systems.

🔗 **[Take this module on Wolfram U →](https://www.wolfram.com/wolfram-u/courses/mathematics/introduction-to-cryptography/)**

---

## Key Concepts

**Hash functions** — Deterministic, one-way functions that map arbitrary inputs to fixed-size outputs. SHA-256 is the hash function used in Bitcoin and Quai mining. Its properties (collision resistance, preimage resistance, avalanche effect) are what make proof of work possible.

**Public/private key cryptography** — Asymmetric key pairs that enable digital ownership. Your private key signs; your public key verifies. The mathematical relationship (elliptic curve discrete logarithm) is computationally irreducible in the Wolfram sense — there is no shortcut from public key to private key.

**Digital signatures** — Proofs that a message was authorized by the holder of a specific private key. ECDSA (Elliptic Curve Digital Signature Algorithm) is the standard in most UTXO blockchains.

**Merkle trees** — Hash-based data structures that enable efficient verification of large datasets. Each block header contains the Merkle root of all its transactions.

## Connection to Thermoeconomics

Cryptographic hash functions are the bridge between information theory and proof of work. Each hash operation is a physical process (Landauer) that maps many inputs to one output (Shannon). The difficulty adjustment (Jaynes) constrains how much computational work is required per valid output. The irreversibility of the hash function (Bennett) is what makes the proof unforgeable.

## Further Resources

- [Shannon — Information Theory](../foundations/information-theory/shannon.md)
- [Landauer — Physical Cost of Computation](../foundations/information-theory/landauer.md)
- [Anders Brownworth's Blockchain Demo](https://andersbrownworth.com/blockchain/) — Interactive visual tool
