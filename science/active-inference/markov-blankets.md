# Markov Blankets and System Boundaries

> **Key paper:** Friston, "Life as We Know It," *Journal of the Royal Society Interface*, 2013
>
> **Formal treatment:** Pearl, *Probabilistic Reasoning in Intelligent Systems* (1988), Chapter 3

## The Concept

A **Markov blanket** is the minimal set of variables that makes a system statistically independent of its environment. If you know the state of the Markov blanket, knowing more about the environment gives you no additional information about the internal states of the system (and vice versa).

In simpler terms: the Markov blanket is the boundary of a system — the interface through which all interaction with the outside world must pass.

## Structure

A Markov blanket consists of:
- **Sensory states** — variables influenced by the environment
- **Active states** — variables that influence the environment
- **Internal states** — variables shielded from direct environmental influence by the blanket

The free energy principle says that any system with a Markov blanket that persists over time must appear to minimize free energy — it must behave *as if* it has a model of its environment and acts to confirm that model.

## Markov Blankets in Blockchain Architecture

Blockchain networks have natural Markov blanket structures:

**Individual node:**
- Sensory states: incoming transactions, block announcements, peer messages
- Active states: outgoing transaction broadcasts, mined blocks, peer responses
- Internal states: mempool, local chain state, mining computations

**The network as a whole:**
- Sensory states: new transactions from users, price signals from exchanges
- Active states: confirmed transactions, block rewards, difficulty adjustments
- Internal states: the consensus chain, pending transactions, mining competition

**Nested structure:** Nodes are Markov-blanketed systems nested within the network, which is itself a Markov-blanketed system within the broader economy. This nesting of scales — from individual hash computations to global monetary properties — is a hallmark of complex self-organizing systems.

## Why This Matters

The Markov blanket formalism gives us a precise way to define system boundaries in blockchain networks. This matters for:

- **Security analysis** — What information crosses the blanket? What is shielded?
- **Scalability** — How do nested Markov blankets (shards, layers, subnets) maintain coherence?
- **Economic analysis** — What signals does the network sense, and how does it act on them?

Quai Network's hierarchical architecture (Prime → Region → Zone) is an explicit engineering of nested Markov blankets — each level has its own boundary, its own sensory and active states, and its own internal dynamics.

## Further Reading

- Friston, "Life as We Know It" (2013)
- Kirchhoff et al., "The Markov Blankets of Life" (2018)
- Clark, "Whatever Next? Predictive Brains, Situated Agents, and the Future of Cognitive Science" (2013)
