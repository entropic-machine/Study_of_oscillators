# Study of Oscillators

This repository explores the dynamics of **linear and non-linear oscillators** through both analytical derivations and computational simulations. Unlike standard literature that often presents solutions as *fait accompli*, this project focuses on the underlying motivations and the physical intuition behind the assumptions used to solve these differential equations.

---

## Project Philosophy
Most textbooks introduce the Simple Harmonic Oscillator (SHO) by assuming a solution of the form $x(t) = A\cos(\omega t + \phi)$. While mathematically sound, this often skips the "why." 

**This study aims to:**
* **Deconstruct** the transition from physical systems to mathematical models.
* **Explain** why specific ansatzes (assumptions) are chosen for linear systems.
* **Explore** where linear approximations fail and how non-linearities (like the Duffing or Van der Pol oscillators) introduce chaotic or limit-cycle behavior.

---

## Key Areas of Study

### 1. Linear Oscillators
We examine the classical damped-driven oscillator. The project focuses on the derivation of the characteristic equation and the physical meaning of the discriminant in underdamped, overdamped, and critically damped cases.

$$\ddot{x} + 2\zeta\omega_n\dot{x} + \omega_n^2 x = F(t)$$

### 2. Non-Linear Dynamics
In the real world, restoring forces are rarely perfectly linear. This section investigates:
* **The Duffing Oscillator:** Modeling systems with "stiffening" or "softening" springs.
* **The Van der Pol Oscillator:** Studying self-sustaining oscillations and limit cycles.
* **Phase Space Analysis:** Moving beyond time-series plots to understand stability and attractors.

---

## Computational Tools & Visualizations
Theory is supplemented by numerical integrations (using Python/SciPy). All scripts used to generate the project's visuals are organized for reproducibility.

* **Plotting:** High-fidelity phase portraits and time-domain signals.
* **Location:** All source code for the visual analysis can be found in the `/plots` folder.
* **Numerical Methods:** Implementation of Runge-Kutta (RK4) methods to solve non-linear equations that lack closed-form analytical solutions.

---

## Directory Structure
```text
.
├── analytical_notes/   # LaTeX/PDF notes on the "true motivation" of assumptions
├── simulations/        # Main scripts for solving ODEs
├── plots/              # Code for generating figures and animations
└── README.md           # Project overview
