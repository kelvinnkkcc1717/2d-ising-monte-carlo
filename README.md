# 2d-ising-monte-carlo
A numerical study of the two-dimensional Ising model using the Metropolis Monte Carlo method.

## Overview

The 2D Ising model is simulated on a square lattice with spins
s = +/-1.

The Metropolis algorithm is used to study the behavior of the system
as a function of temperature.

The following quantities are calculated:

- Magnetization
- Energy
- Specific heat
- Magnetic susceptibility

## Model

The Hamiltonian of the Ising model is

H = -J sum_<ij> s_i s_j

where J is the nearest-neighbor coupling and each spin can take the
values +1 or -1.

For this simulation:

- Lattice size: 15 x 15
- J = 1
- kB = 1
- Temperature range: 1.5 to 3.5

## Method

The Metropolis algorithm is used to update the spin configuration.

For a proposed spin flip, the change in energy is calculated and the
new configuration is accepted according to the Metropolis acceptance
probability.

The simulation is first equilibrated and measurements are then
collected over subsequent Monte Carlo steps.

## Results

The simulation shows:

- Decreasing magnetization with increasing temperature.
- Increasing energy with temperature.
- A peak in the specific heat near the magnetic transition.
- A peak in the magnetic susceptibility near the transition.

The results demonstrate the use of Monte Carlo methods to study
temperature-dependent behavior and phase-transition phenomena.

## Tools

- Python
- NumPy
- Matplotlib
- Jupyter Notebook

## File

`ising montecarlo.ipynb` - Jupyter notebook containing the complete
simulation and results.

## Future Work

- Increase the lattice size.
- Increase the number of Monte Carlo steps.
- Study finite-size effects.
- Improve sampling near the critical temperature.
- Compare the numerical transition with the known 2D Ising critical
  temperature.
