# OBJECTIVE 
To show entanglement appears nonlocal in low dimensions, but is fully causal in high-dimensional Hilbert-space dynamics.(for more theoritical info see phy.pdf)
# SIMULATION 0
(IGNORE , GRIFFITHS QM EXERCISE BUT ITS REALLY AN INTERESTING ONE )
# Simulation 1: Hilbert-Space Guided Trajectories
This model establishes the core concept: a particle's trajectory is biased by a hidden internal state, which is only revealed by a later measurement.

Code Analysis:

The script initializes particles with a 2D complex internal state (psi) in a superposition.

In each time step, the particle's position x is pushed by a "drift" force proportional to the difference in the squared magnitudes of its internal state components (|psi[0]|² - |psi[1]|²).

The internal state psi also evolves randomly at each step.

After the evolution is complete, a "delayed-choice" measurement collapses the state, and the particle's entire path is colored based on this final outcome.

Results & Interpretation:

The plot shows two sets of trajectories (red and blue) that begin to separate long before the measurement is made.

This is a perfect visual demonstration of post-selection. There is no backward-in-time causation. The measurement simply sorts the particles based on a bias that was present and evolving throughout their entire history. The internal state psi guided the trajectory all along.

# Simulation 2: A Simplified Quantum Eraser Model
This version simplifies the dynamics to make the post-selection effect even more stark and clear.

Code Analysis:

This model uses real-valued amplitudes (psi0, psi1) that remain static throughout the simulation.

The drift force is simplified to be directly proportional to the difference in these initial amplitudes (psi0 - psi1).

The simulation again performs a delayed measurement based on the initial hidden state to color the trajectories.

Results & Interpretation:

The resulting plot shows an extremely clean and dramatic separation of the red and blue trajectories.

By removing the random evolution of the internal state, the bias is constant. This makes the simulation a clearer, albeit less physical, analogy for how sorting data based on hidden "which-path" information reveals distinct groups.

# Simulation 3: The Double-Slit Quantum Eraser Analogy
This simulation shifts from tracking trajectories to modeling the final pattern in a double-slit experiment.

Code Analysis:

The code simulates particles passing through one of two slits. The choice of slit is determined by hidden amplitudes (psi0, psi1), acting as a "which-path" tag.

The simulation generates two plots: one showing the combined positions of all particles, and a second showing the positions sorted and colored by a delayed measurement of their hidden "which-path" tag.

Results & Interpretation:

The unsorted plot shows two broad clumps, representing the classical expectation for particles passing through two slits—no interference.

The sorted plot perfectly separates these two clumps, revealing the distinct distributions from each slit.

This brilliantly illustrates the quantum eraser concept. When you have which-path information (i.e., you can sort the data), you see distinct particle-like behavior. In a true quantum experiment, "erasing" this information would make an interference pattern emerge from the combined data.

# Simulation 4: The Effect of Internal Complexity (Dimensionality N)
This model introduces a critical new variable: the dimensionality N of the internal Hilbert space, exploring how hidden complexity affects observable motion.

Code Analysis:

A particle's 1D motion is coupled to an N-dimensional internal state. The drift force is proportional to the sum of all N components.

A delayed measurement sorts particles based on the sign of this sum. The entire simulation is run for different values of N.

Results & Interpretation:

The final position histograms show that as N increases, the separation between the two measured groups becomes much clearer.

A more complex internal state (higher N) can store more information, creating a stronger and more consistent drift signal. This allows the post-selection measurement to sort the particles much more effectively.

# Simulation 5: Modeling True Interference with Complex Amplitudes
This was a major leap, incorporating the mathematics needed to simulate wave-like interference.

Code Analysis:

The internal state is upgraded to use complex numbers, like the amplitudes of a quantum wavefunction.

The key innovation is the final plot: a weighted histogram. Each particle's contribution is weighted by |sum(amplitudes)|², mimicking the Born rule for calculating quantum probabilities.

Results & Interpretation:

The resulting plot shows a clear interference pattern with peaks and valleys. This pattern is completely absent in the raw position data and only emerges when weighted by the internal state's constructive and destructive interference.

# Simulation 6: The Classical Limit from High Complexity
This experiment combines the N-sweep with the interference calculation to ask a new question: how does internal complexity affect the interference pattern itself?

Code Analysis:

The script generates weighted interference patterns for N = 1, 5, 10, and 50.

Results & Interpretation:

The results show a remarkable trend: as N increases, the interference pattern becomes narrower, eventually collapsing into a single central peak at N=50.

This is a beautiful analogy for the emergence of classical behavior. Due to the Central Limit Theorem, the sum of many random internal components averages to zero. The "quantum" drift signal washes out, the particle's motion is dominated by classical diffusion, and the interference vanishes.

# Simulation 7: The Path Integral & Dynamic Feedback
This final, most sophisticated model introduces a dynamic, two-way coupling between spacetime and the internal Hilbert space.

Code Analysis:

A feedback loop is created: the particle's position x influences its internal state h, and h in turn influences x.

The measurement is a continuous weight calculated by projecting the internal state at an intermediate time.

Results & Interpretation:

The feedback loop creates complex oscillatory motion in the trajectories.

The final weighted histogram is an analogy for Feynman's Path Integral. Each trajectory is a "path," its weight is its "phase," and the final plot is the interference pattern from the sum over all possible paths. It shows how interference arises from the entire history of interaction between a particle's observable path and its evolving internal state.

# USAGE
just open colab or jupyter and run one by one scripts to get visualizations.
