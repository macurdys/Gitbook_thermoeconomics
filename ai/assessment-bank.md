# Assessment Bank

Questions for testing understanding, organized by topic and difficulty. Use these for self-assessment or give them to an AI tutor to quiz you.

---

## Information Theory

**Beginner**
1. In your own words, what does Shannon entropy measure?
2. A fair coin has entropy H = 1 bit. What is the entropy of a fair six-sided die?
3. Why is a completely predictable message (e.g., all zeros) said to have zero information?

**Intermediate**
4. Compute the entropy of a source that outputs A with probability 0.9 and B with probability 0.1. Is this more or less than 1 bit? Why?
5. Explain the difference between entropy and mutual information. Give an example of each in a blockchain context.
6. What does it mean to say that a valid block hash at difficulty D carries approximately log₂(D) bits of information?

**Advanced**
7. Explain Jaynes' Maximum Entropy Principle. How does it connect to the Boltzmann distribution?
8. The difficulty adjustment maintains a constant block production rate regardless of hash rate. Explain this as a MaxEnt constraint in Jaynes' framework.
9. Shannon entropy and Boltzmann entropy have the same mathematical form. Is this a coincidence? Explain, citing Jaynes.

---

## Thermodynamics of Computation

**Beginner**
10. What is Landauer's Principle? State it in one sentence.
11. Why does erasing information produce heat?
12. Is the energy cost of Bitcoin mining above or below the Landauer limit? By how much (order of magnitude)?

**Intermediate**
13. Bennett showed that computation can be thermodynamically reversible. If that's true, why does mining have an irreducible energy cost?
14. Calculate the Landauer limit energy cost to erase one bit at room temperature (T = 300K, kB = 1.38 × 10⁻²³ J/K).
15. A miner performs 2⁷⁰ hash operations to find a valid block. Each SHA-256 hash involves approximately 25,000 logical operations. Estimate the minimum Landauer energy cost.

**Advanced**
16. Explain the relationship between logical irreversibility and thermodynamic irreversibility. Why is hash computation logically irreversible?
17. If all computation can be made reversible (Bennett), and only erasure costs energy (Landauer), where exactly in the mining process does the irreversible erasure occur?
18. Explain why no future engineering improvement can eliminate the thermodynamic cost of proof of work.

---

## Proof of Work

**Beginner**
19. What is a nonce? What role does it play in mining?
20. Explain the longest-chain rule in one paragraph.
21. Why can't a miner just claim they did the work without actually doing it?

**Intermediate**
22. Each hash attempt in PoW mining is a Bernoulli trial. What is the success probability at difficulty D?
23. Explain why the difficulty adjustment is necessary. What would happen without it?
24. Compare proof of work and proof of stake. What does PoW provide that PoS cannot, from a thermoeconomic perspective?

**Advanced**
25. Walk through the nine-step argument that PoW is a thermodynamic process (one sentence per step, citing the relevant tradition).
26. Explain "unforgeable costliness" using Landauer's principle and computational irreducibility.
27. Why is the Landauer limit important even though actual mining costs are orders of magnitude above it?

---

## Computational Mechanics

**Intermediate**
28. What is an epsilon machine? Why is it called "minimal and unique"?
29. What is statistical complexity (Cμ)? How is it different from entropy?
30. SHA-256 output has high entropy but low statistical complexity. The mining process has lower entropy but higher statistical complexity. Explain why.

**Advanced**
31. Explain what causal states are and why they are defined as equivalence classes of histories.
32. Where is complexity maximized — in perfectly ordered systems, perfectly random systems, or somewhere in between? Why?

---

## Wolfram Physics

**Intermediate**
33. What is computational irreducibility? Give an example outside of blockchain.
34. Explain causal invariance. Why is it analogous to blockchain consensus?

**Advanced**
35. Fill in the parallels: Hypergraph rewriting rules → ___. Different rule application orders → ___. Causal invariance → ___. Same causal graph → ___.

---

## Deacon & Active Inference

**Intermediate**
36. What is an autogen? Explain the two components and why neither works alone.
37. Explain how a PoW blockchain is an autogenic system.
38. What is the Free Energy Principle in one sentence?

**Advanced**
39. Explain "absential features" — how can something that doesn't exist do causal work?
40. How does the mining process function as active inference? What is the "generative model," what is the "surprise," and what is the "action"?

---

## Quai Network & Thermoeconomic Operator

**Intermediate**
41. What is the difference between Bitcoin's threshold difficulty and Quai's PoEM?
42. Explain the dual-currency system: what does Qi represent? What does Quai represent?
43. Why is PoEM described as "lossless" compared to threshold difficulty's "lossy compression"?

**Advanced**
44. Explain the Market-Induced Hamiltonian. How does the market price retroactively impose an energy function on hash space?
45. Why can Qi emission be strictly proportional to hash rate? What property of PoEM makes this possible?
46. Explain the kQuai controller mechanism. What economic equilibrium does it seek?

---

## Synthesis

**Essay Questions (Expert Level)**

47. In 500 words, explain why proof of work is the only known physical basis for unforgeable digital scarcity. Reference at least three of the six foundational traditions.

48. Explain the full arc from Landauer's Principle to Qi emission. What chain of reasoning connects the minimum energy cost of erasing a bit to the creation of energy money?

49. "Proof of stake replaces physics with game theory." Evaluate this claim using the thermoeconomic framework.

50. The actual energy cost of mining is ~10¹⁰ times the Landauer limit. Does this undermine or support the thermoeconomic thesis? Argue both sides, then give your answer.
