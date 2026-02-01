# Finney (2004) — Reusable Proofs of Work

> **Original site:** [rpow.net](https://nakamotoinstitute.org/finney/rpow/) (archived at Nakamoto Institute)
>
> **Announcement:** Hal Finney, RPOW announcement on the Cypherpunks mailing list, August 2004

## Summary

Hal Finney's Reusable Proofs of Work (RPOW) was the first system to make proof-of-work tokens *transferable* — the critical step from computational puzzles to digital money.

In previous proof-of-work systems (Hashcash), the proof was used once and discarded. Finney's insight: a proof of work can be exchanged for a new token, which can itself be exchanged, creating a chain of transfers. The computational cost is incurred once but the token persists.

## Key Concepts

**Transferability** — The missing piece between proof of work and money. A hashcash stamp proves work was done, but it can't be *spent twice* or *passed along*. RPOW solved this by issuing signed tokens from a trusted server that could be exchanged for new tokens of equal value.

**Trusted computing** — RPOW used IBM's trusted computing hardware to ensure the server was running the published code and not inflating the token supply. This was a centralized trust mechanism — the weakness that Nakamoto would later eliminate.

**The bridge to Bitcoin** — Finney was the recipient of the first Bitcoin transaction (from Nakamoto) and one of the earliest contributors to the Bitcoin project. His RPOW work was the conceptual bridge between proof of work as spam prevention and proof of work as money.

## Connection to Thermoeconomics

RPOW made explicit what was implicit in all previous proof-of-work systems: **if computation has cost, then proof of computation has value, and that value can be transferred**. This is the core claim of thermoeconomics stated as an engineering specification.

Finney saw that the energy spent on proof of work is not consumed — it is *transformed* into a transferable token of value. The token is a receipt for thermodynamic dissipation.

## Further Reading

- Finney's RPOW source code and documentation at [Nakamoto Institute](https://nakamotoinstitute.org/finney/rpow/)
- Szabo, "Bit Gold" (2005) — parallel development with similar goals
- Nakamoto (2008) — the decentralized successor
