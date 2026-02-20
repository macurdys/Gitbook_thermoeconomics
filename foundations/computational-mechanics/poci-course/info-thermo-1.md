# Information Thermodynamics, Part I

**Lecture 37a** — Guest Lecturer: Alec Boyd
📺 [Watch on YouTube](https://www.youtube.com/watch?v=5OTRxg2M2cg)
📄 Reading: CMR article IRatchet

---

This lecture establishes the bridge between information theory and thermodynamics — the theoretical foundation of thermoeconomics.

---

## The Core Identity

Thermodynamic entropy and Shannon entropy are the same thing, measured in different units:

**S = kB ln 2 · H**

Where:
- S is thermodynamic entropy (Gibbs)
- H is Shannon entropy (bits)
- kB is Boltzmann's constant
- The factor kB ln 2 converts between nats and joules/kelvin

This is not an analogy. It is a mathematical identity. Every result in information theory has a thermodynamic counterpart, and vice versa.

---

## Thermodynamic Entropy: Two Faces

**As disorder:** A hot gas has high thermodynamic entropy. A cold crystal has low entropy.

**As uncertainty:** Shannon entropy measures unpredictability. A string of measurements from an unpredictable source has high entropy. A periodic string has zero entropy.

Same mathematics. Same physics. Different language.

---

## The Laws, Restated

### First Law (Energy Conservation)
Energy of each microstate specified by the Hamiltonian. Equations of motion conserve total energy: dE/dt = 0.

### Second Law (Entropy Increase)
In isolated systems: dS/dt ≥ 0, equivalently dH/dt ≥ 0.

Hot systems evolve toward maximum entropy (the microcanonical ensemble — uniform distribution over states at fixed energy).

### Temperature
Defined as the rate of entropy increase with energy:

**1/T = ∂S/∂E**

This connects the information-theoretic and thermodynamic descriptions: temperature tells you how many new microstates become accessible per unit of added energy.

---

## Heat Engines

Energy flows between hot reservoir, cold reservoir, and work output.

**Carnot efficiency:** η ≤ 1 − Tc/Th

This bound comes directly from the second law. The entropy increase of the cold reservoir must at least compensate the entropy decrease of the hot reservoir. No engine can beat this.

---

## Thermodynamics of Control

When you _control_ a thermodynamic system (manipulate its energy landscape while it's in contact with a heat bath):

- **Work decomposition:** d⟨E⟩ = ⟨dW⟩ + ⟨dQ⟩
- **Dissipated work:** ⟨Wdiss⟩ = ⟨W⟩ − ΔFNEQ
- **Nonequilibrium free energy:** FNEQ = ⟨E⟩ − TS

The key bounds:

> **⟨Q⟩ ≥ kBT ln 2 · ΔH[X]** — heat flow bounded by change in Shannon entropy
>
> **⟨W⟩ ≥ Δ⟨E⟩ − kBT ln 2 · ΔH[X]** — work bounded by energy change minus information change

Information is a thermodynamic resource. Gaining information (reducing entropy) costs work. Using information (increasing entropy) releases work.

---

## Szilard's Engine

The simplest information engine:

1. Single particle in a box
2. Insert barrier at midpoint
3. **Measure** which side the particle is on
4. Use measurement to slowly expand that side, extracting work
5. Result: **⟨W⟩ = kBT ln 2** per cycle

One bit of measurement → one kBT ln 2 of work extracted. This is the conversion rate between information and energy.

---

## Maxwell's Demon

Maxwell imagined a being that could sort fast and slow gas molecules, creating a temperature gradient from equilibrium — apparently violating the second law.

The resolution (Landauer, Bennett): the demon must _store_ measurement results. Its memory fills up. Eventually it must _erase_ that memory to continue operating.

**Landauer's Principle:** Erasing one bit of information dissipates at least kBT ln 2 of heat.

The demon's erasure cost exactly cancels its sorting gains:
- Work extracted per measurement: +kBT ln 2
- Work required for erasure: −kBT ln 2
- Net: ΔStotal ≥ 0

The second law holds. But the mechanism is informational, not energetic.

---

## The Szilard Cycle in Full

| Step | What happens | Entropy change |
|------|-------------|---------------|
| **Measure** | Demon learns particle position | Demon memory: ΔS > 0 |
| **Control** | Barrier slides, work extracted | System: ΔS < 0 |
| **Erase** | Reset demon memory | Heat dissipated: ΔS > 0 |
| **Net** | One full cycle | **ΔStotal = 0** (reversible limit) |

The average dissipated heat is exactly calculable as the work done to slide barriers:
Q = W = −TΔS[X]

---

## Why This Matters

This lecture establishes three things that are non-negotiable for thermoeconomics:

1. **Information is physical.** It occupies physical states, obeys physical laws, and has physical costs.
2. **Computation has thermodynamic costs.** Specifically, _irreversible_ computation (erasure) has a minimum energy cost of kBT ln 2 per bit.
3. **Information is a thermodynamic fuel.** It can be converted to work, stored, transmitted, and consumed — just like energy, but on different terms.

Every hash in a proof-of-work system is an irreversible computation. Every block is an erasure event. The mining cost isn't waste — it is the thermodynamic price of creating structured information.

---

_Next: [Information Thermodynamics II](info-thermo-2.md) — information engines, ratchets, transducers, and the Information Processing Second Law._

