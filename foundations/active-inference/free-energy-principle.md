# Friston — The Free Energy Principle

> **Key paper:** Karl Friston, "The Free-Energy Principle: A Unified Brain Theory?" *Nature Reviews Neuroscience*, Vol. 11, pp. 127–138, 2010.
>
> **Textbook:** Parr, Pezzulo & Friston, *Active Inference* (MIT Press, 2022)

## Overview

The Free Energy Principle (FEP) states that any self-organizing system that maintains itself in a changing environment must minimize **variational free energy** — an information-theoretic quantity that bounds the surprise (negative log-probability) of the system's sensory states.

In plain terms: things that exist must be good at not being surprised by what happens to them. If they were constantly surprised, they would dissolve into their environment — they would cease to exist as distinct systems.

## Key Concepts

**Variational free energy** — An upper bound on surprise (or equivalently, a lower bound on model evidence). Minimizing free energy is equivalent to maximizing the accuracy of an internal model while minimizing its complexity. This is a formal version of Occam's razor.

**Generative model** — The internal model that a system uses to predict its sensory inputs. In a brain, this is the neural architecture. In an economic agent, this is their model of the market. In a blockchain, this is the protocol rules plus the current chain state.

**Active inference** — Systems don't just passively update their models (perception); they also act on the world to make their predictions come true (action). A thermostat doesn't just measure temperature — it turns the heater on. A miner doesn't just observe the mempool — it constructs a block and hashes it.

## Connection to Thermoeconomics

Proof-of-work mining is active inference:

1. **The generative model** — The protocol rules define what a valid block looks like. Each miner has a model of what the next block should be.
2. **Prediction** — The miner predicts that a specific nonce will produce a hash below the target.
3. **Action** — The miner hashes the candidate block (acts on the world).
4. **Surprise** — Almost every hash is "surprising" (doesn't meet the target). The miner updates and tries again.
5. **Free energy minimization** — The miner adjusts strategy (transaction selection, nonce range, hardware allocation) to minimize the expected surprise — i.e., maximize the probability of finding a valid block.

The network as a whole is an active inference system that maintains a shared generative model (the blockchain) by continuously acting on the physical world (consuming energy) to reduce uncertainty (achieving consensus on transaction ordering).

## Further Reading

- Friston, "A Free Energy Principle for Biological Systems" (2012)
- Friston et al., "Active Inference and Epistemic Value" (2015)
- [Active Inference Institute](https://www.activeinference.org/)
