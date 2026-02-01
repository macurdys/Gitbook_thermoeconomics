# Dwork & Naor (1993) — Pricing via Processing

> **Paper:** Cynthia Dwork and Moni Naor, "Pricing via Processing, or Combating Junk Mail," *Advances in Cryptology — CRYPTO '92*, Lecture Notes in Computer Science, Vol. 740, pp. 139–147, 1993.

## Summary

The first formal proposal to use computational puzzles as a pricing mechanism. Dwork and Naor proposed requiring email senders to solve a moderately hard computational problem before their message would be accepted. The cost in computation (and therefore time and energy) would be negligible for legitimate senders but prohibitive for spammers sending millions of messages.

## Key Concepts

**Computational pricing function** — A function that is moderately hard to compute but easy to verify. The sender proves they have "paid" a computational cost.

**The foundational insight** — Computation has a real cost (time, energy, hardware). This cost can serve as a substitute for monetary payment in contexts where traditional payment is impractical. This is the conceptual origin of proof of work.

## Connection to Thermoeconomics

Dwork and Naor identified the core principle: **computation is a physical resource that can be used as a cost mechanism**. They did not frame it in thermodynamic terms, but the underlying logic is Landauer's: computation costs energy, and that cost is inescapable.

Every subsequent development — Hashcash, RPOW, Bitcoin — is an elaboration of this insight.

## Further Reading

- Back (1997) — the practical implementation
- Jakobsson & Juels, "Proofs of Work and Bread Pudding Protocols" (1999) — formalization of the concept
