# Nakamoto (2008) — Bitcoin: A Peer-to-Peer Electronic Cash System

> **Paper:** Satoshi Nakamoto, "Bitcoin: A Peer-to-Peer Electronic Cash System," October 31, 2008.
>
> **PDF:** [bitcoin.org/bitcoin.pdf](https://bitcoin.org/bitcoin.pdf)

## Summary

Nakamoto's paper describes a system for electronic transactions that does not rely on trust in third parties. It combines proof of work, a peer-to-peer network, and a chain of cryptographic hashes to create a decentralized ledger that is secure as long as honest nodes control a majority of the network's computational power.

## Key Innovations

**Proof of work for consensus** — Previous systems used proof of work to prevent spam or create tokens. Nakamoto used it to solve the Byzantine Generals Problem: how to achieve agreement among untrusted parties without a central coordinator. The longest chain represents the most computational work, and therefore the consensus view.

**The difficulty adjustment** — The protocol adjusts the difficulty of the proof-of-work puzzle to target a fixed block production rate (one block per ~10 minutes) regardless of total hash power. This is the thermodynamic governor of the system.

**The UTXO model** — Transactions consume unspent outputs and create new ones. This model (explored in detail in the UTXO Architectures section) provides natural parallelism, privacy, and auditability.

**The block reward halving** — New coins are created as block rewards, halving approximately every four years. This creates a disinflationary supply schedule that asymptotically approaches 21 million coins.

## Connection to Thermoeconomics

Bitcoin is the first system to explicitly ground economic value in thermodynamic work. The security of the network, the scarcity of the tokens, and the cost of attack are all direct functions of energy expenditure. This is not a design choice that could have been made differently — it is a consequence of the physics.

The difficulty adjustment is particularly significant: it ensures that the information production rate (bits of proof per unit time) remains constant regardless of total computational power. This makes Bitcoin a constant-entropy-rate system — a thermodynamic steady state maintained far from equilibrium by continuous energy input.

## Further Reading

- Back (1997) — the proof-of-work mechanism Bitcoin uses
- Finney (2004) — the concept of transferable proofs of work
- Szabo (2005) — "Bit Gold," the closest conceptual predecessor
- [bitcoin.org/bitcoin.pdf](https://bitcoin.org/bitcoin.pdf)
