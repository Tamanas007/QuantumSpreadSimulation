# Spacetime + Hilbert-Space Path-Integral Simulator

## Overview
# Core Objective

Our goal was to explore whether complex quantum behaviors like the delayed-choice experiment and interference could be intuitively understood by modeling particles as having not just a position in spacetime, but also a hidden "internal state" within an abstract Hilbert space.

Phase 1: The Basic "Delayed-Choice" Model

We began with a simple concept: what if a particle's trajectory was secretly biased by a hidden internal state?

Simulation: Particles moved randomly, but with a slight "drift" determined by a static, internal Hilbert vector. We then performed a "delayed-choice" measurement by reading this internal state after the trajectory was complete and coloring the particle's entire path based on the outcome.

# Key Insight:
We immediately saw the core illusion of retrocausality. The trajectories of different colors appeared to "know" their future measurement outcome from the very beginning. This simulation proved that no backward-in-time influence was needed. The measurement was simply post-selection—a way of sorting particles based on a bias they had all along.

Phase 2: The Role of Internal Complexity

Next, we investigated how the complexity of the internal state affected the outcome. We did this by changing the number of dimensions, N, of the Hilbert space.

Simulation: We ran the same experiment but varied N from a very small number (like 1) to a large one (like 50).

Key Insight: This revealed a profound connection to the classical world.

Low N: The internal state provided a strong, simple signal, leading to highly biased trajectories.

High N: The many random components of the internal state averaged out to nearly zero (a consequence of the Central Limit Theorem). This canceled out the drift, and the particle's motion became simple, classical diffusion. This showed how increasing hidden complexity can "wash out" quantum effects and lead to classical behavior.

Phase 3: Introducing True Interference

To go beyond simple sorting, we needed to simulate the wave-like nature of particles.

Simulation: We upgraded the internal state to use complex numbers, analogous to the amplitudes of a quantum wavefunction. We then calculated a final "interference pattern" not by counting particles, but by creating a weighted histogram. Each particle's weight was the squared magnitude of the sum of its internal complex amplitudes (|sum(amplitudes)|²).

# Key Insight: 
This was a breakthrough. The resulting plots showed clear interference fringes—peaks and valleys that were completely absent in the raw position data. We had successfully modeled interference as an effect emerging from the addition and cancellation of hidden, internal amplitudes.

Phase 4: The Path Integral & Dynamic Feedback

Our final and most advanced model introduced a dynamic, two-way coupling between the particle's position and its internal state.

# Simulation: 
The particle's position now influenced its internal state, and the internal state influenced its position, creating a feedback loop. The trajectories became complex and oscillatory. We then used a measurement of the internal state at an intermediate time to weight each particle's contribution to the final interference pattern.

# Key Insight:
This simulation became a beautiful analogy for Feynman's Path Integral. Each trajectory was a single "path," and its weight represented the "phase" contribution of that path to the final outcome. Summing all these weighted paths produced our most intricate and realistic interference pattern yet, showing how interference arises from the history of interaction between a particle's external path and its internal state.

# Overall Conclusion

Across these simulations, we built a consistent and intuitive framework. Quantum phenomena can be viewed not as spooky actions in spacetime, but as the observable consequences of a richer reality: a combined manifold of spacetime and an internal Hilbert space. A "measurement" is simply a projection—a partial glimpse into this internal space—that allows us to sort through spacetime events and reveal the profound correlations that were encoded within this higher-dimensional structure all along.

---

## Features

- **Coupled evolution:** Simulate spacetime + Hilbert-space dynamics.
- **Measurement & post-selection:** Project internal Hilbert state to assign measurement outcomes.
- **Interference visualization:** Weighted histograms produce interference-like patterns.
- **Parameter sweep:** Explore how Hilbert-space dimension \(N\) affects trajectories and final distributions.
- **Convergence analysis:** Observe deviations from standard QM at small \(N\) and convergence for large \(N\).

---

## Installation

Requires Python 3.9+ and common scientific libraries:


# git clone <repo-url>
cd spacetime-hilbert-simulator
pip install -r requirements.txt


# Usage
Run the simulation

This script will:

Initialize particles with random spacetime positions and Hilbert vectors.

Evolve trajectories over time with Hilbert-space coupling.

Perform measurement projections at specified times.

Generate plots of:

Trajectories colored by measurement outcome

Interference patterns weighted by Hilbert-space amplitudes

Hilbert dimension 
𝑁
N sweep to visualize convergence to QM

Example plots

Trajectory Plot: Particle paths in spacetime, colored by projected measurement outcome.

Interference Histogram: Weighted final x-positions showing constructive and destructive interference.

N-Sweep Comparison: Shows how small Hilbert-space dimensions produce deviations, while large dimensions converge to standard QM behavior.

# Scientific Notes

The simulation does not attempt to explain wavefunction collapse. It demonstrates how post-selection and Hilbert-space coupling can generate interference patterns.

Small Hilbert dimensions exhibit classical-like behavior; large dimensions converge to standard QM predictions.

This framework is useful for exploring finite-dimensional approximations of quantum systems, visualizing path-integral contributions, and testing new conceptual ideas in quantum foundations.

# References

Delayed-choice quantum eraser and post-selection literature

Path-integral formulation (Feynman, 1948)

Hilbert-space dynamics in finite-dimensional approximations of QM

