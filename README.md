# Measurement-Induced Phase Transition (MIPT) Simulator

A high-performance Julia library for simulating Measurement-Induced Phase Transitions using Matrix Product States (MPS). This project was developed to analyze entanglement entropy scaling in hybrid quantum circuits.

## Key Features
* **MPS & Exact Simulation:** Supports both Matrix Product State (via `ITensors.jl`) and exact statevector simulation modes.
* **Parallelized:** Implements `Threads.@threads` for parallel Monte Carlo trials.
* **Stabilizer Rényi Entropy:** Includes (experimental) support for SRE calculation.

## Dependencies
* Julia 1.9+
* ITensors.jl
* JLD2 (for data serialization)

## Usage
To run a parameter sweep:
```julia
julia --threads auto run_experiment.jl
