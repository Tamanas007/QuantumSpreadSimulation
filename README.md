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

```bash
git clone <repo-url>
cd spacetime-hilbert-simulator
pip install -r requirements.txt

numpy
matplotlib
scipy
tqdm



