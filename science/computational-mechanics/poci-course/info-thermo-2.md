# Information Thermodynamics, Part II

**Lecture 37b** — Guest Lecturer: Alec Boyd
📺 [Watch on YouTube](https://www.youtube.com/watch?v=QFZdJLo_LpE)
📄 Reading: CMR article IRatchet

---

Part I established that information is physical and has thermodynamic costs. Part II answers: **what can information _do_?**

---

## Information is a Thermodynamic Fuel

Instead of erasing the demon's memory (paying kBT ln 2 in heat), write it to a hard drive.

The hard drive's entropy increases. The system's entropy decreases. Work is extracted. Total entropy: ΔStotal ≥ 0.

Information, stored on a physical medium, is a fuel that can be burned to produce work — just like a temperature difference between two reservoirs.

---

## Three Reservoirs

A **heat engine** moves energy between three reservoirs:
1. Hot thermal reservoir
2. Cold thermal reservoir
3. Work reservoir

An **information engine** moves energy and information between three reservoirs:
1. Thermal reservoir (temperature T)
2. Work reservoir
3. **Information reservoir**

The information reservoir has a crucial property: **its temperature is zero.** Every configuration has equal energy, so adding information (increasing entropy) costs no energy. It is a reservoir of pure structure.

The work reservoir has the opposite property: **its temperature is infinite.** It stores energy with no entropy.

---

## Information Reservoirs

A bit string is an information reservoir if every 0 and 1 have the same energy.

This means the string's entropy is entirely informational — it encodes structure, not thermal energy. Changing the string's content changes its information without changing its energy.

Physical realization: metastable systems with degenerate energy levels. A magnetic domain pointing up or down. A charge stored or not stored. A UTXO spent or unspent.

---

## The Information Ratchet

Mandal and Jarzynski's exactly solvable autonomous Maxwell's demon:

An input bit string feeds a ratchet mechanism coupled to a thermal reservoir. The ratchet reads each input bit, uses it to extract work, and writes an output bit.

If the input is structured (low entropy) and the output is random (high entropy), work is extracted. The information is _consumed_ — converted from structure to randomness.

The ratchet has internal states. It is a **transducer** — a machine that reads one process, transforms it, and writes another.

---

## Transducers: The Paradigm

**Input HMM → Transducer → Output HMM**

A transducer takes symbols from an input process, transforms them using its internal states, and produces an output process. This is the general framework for information processing as a physical process.

The transducer has:
- Internal states (the demon's memory)
- Input-output transition rules
- A coupling to a thermal reservoir

The input and output are both stochastic processes, each described by their own ε-machine.

---

## Thermodynamics of Transducers

The central result of information thermodynamics:

> **Asymptotic work per step:** ⟨W⟩ ≥ kBT ln 2 · (hμ − h'μ)

Where:
- hμ = entropy rate of the input process
- h'μ = entropy rate of the output process

**The minimum thermodynamic cost of transduction is proportional to the difference in entropy rates.**

If the output is more random than the input (h'μ > hμ): work is released. The transducer is an **engine** — it burns information structure to produce work.

If the output is more structured than the input (h'μ < hμ): work is consumed. The transducer is an **eraser** — it uses work to create information structure.

---

## Thermodynamic Functionality

| Function | Input → Output | Work | Example |
|----------|---------------|------|---------|
| **Engine** | Structured → Random | Extracted | Szilard engine, mining hardware |
| **Eraser** | Random → Structured | Consumed | Memory reset, block creation |
| **Transducer** | Structured → Structured (different) | Depends on entropy rate difference | Hash function, encryption |

---

## The Information Processing Second Law

The generalization of the second law to information-processing systems:

Total entropy production = thermodynamic entropy change + information entropy change ≥ 0

This is not the classical second law (which only tracks thermal entropy). It accounts for the information content of the system's computational states. A system can _decrease_ its thermal entropy if it _increases_ its informational entropy by at least as much.

### Key consequences:

1. **Modularity dissipation** — When a complex computation is broken into modules, each module boundary dissipates additional heat. The total dissipation exceeds the sum of what each module would dissipate in isolation.

2. **Pattern extraction costs** — Extracting a pattern from noisy data (reducing the data's entropy while increasing the model's entropy) has a minimum thermodynamic cost.

3. **Pattern generation costs** — Generating structured output from random input requires work proportional to the structure created.

---

## The Thermoeconomic Synthesis

This is where all six traditions converge:

**Shannon** gave us entropy — the measure of randomness.
**Landauer** proved information is physical — computation has energy costs.
**Crutchfield** gave us ε-machines — the measure of structure.
**Boyd/Crutchfield** gave us the Information Processing Second Law — the thermodynamic cost of transforming structure.

A proof-of-work miner is a transducer:
- **Input:** Random nonces + block template (structured)
- **Output:** Valid block (highly structured) + heat
- **Internal states:** The mining algorithm's computational states
- **Thermal reservoir:** The physical environment absorbing waste heat
- **Work consumed:** Electricity

The minimum cost of mining is set by the entropy rate difference between the input and output processes. This is not an engineering limit — it is a thermodynamic limit. It is the price of creating structured information in a physical universe governed by the second law.

The block reward is payment for this thermodynamic work. The difficulty adjustment ensures the work is real. The chain selection rule ensures the structure is canonical. The economic value of the token is, at bottom, the economic value of the thermodynamic transformation that produced it.

---

## Key Equations

| Equation | Meaning |
|----------|---------|
| S = kB ln 2 · H | Thermodynamic ↔ Shannon entropy |
| ⟨W⟩ = kBT ln 2 | Work from one bit of information (Szilard) |
| Qerase ≥ kBT ln 2 | Landauer's erasure cost |
| ⟨W⟩ ≥ kBT ln 2 · (hμ − h'μ) | Transducer work bound |
| ΔStotal = ΔSthermo + ΔSinfo ≥ 0 | Information Processing Second Law |

---

_This concludes the information thermodynamics sequence. Return to the [POCI Course Map](README.md) or continue to the [full lecture outline archive](../../../resources/poci-outlines.md)._

