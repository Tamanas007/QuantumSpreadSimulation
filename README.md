# Spacetime + Hilbert-Space Path-Integral Simulator

## Overview

This repository contains a simulation framework exploring **particle trajectories coupled with finite-dimensional Hilbert-space dynamics**, inspired by delayed-choice quantum eraser experiments. The core idea is:

- Particles evolve in physical spacetime while carrying an internal Hilbert-space vector.
- Coupling between Hilbert-space and trajectory influences the motion.
- Measurement is implemented as a projection in Hilbert space, post-selecting trajectories based on internal state.
- Interference patterns emerge naturally from path-integral-like weighting of all trajectories.

This framework allows studying the crossover between classical-like behavior (small Hilbert dimension) and standard quantum mechanics (large Hilbert dimension).

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

