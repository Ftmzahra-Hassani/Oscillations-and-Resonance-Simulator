# Oscillations and Resonance Simulator

A Python-based scientific simulation of damped and forced harmonic oscillations using numerical integration and the fourth-order Runge-Kutta (RK4) method.

This project explores the dynamic behavior of a mass-spring system under external periodic forces, with a focus on oscillatory motion, energy analysis, damping, and resonance.

Project Overview

The simulator models a mass-spring-damper system governed by Newton's second law:

[
m\frac{d^2x}{dt^2}+b\frac{dx}{dt}+kx=F_0\cos(\omega t)
]

Where:

- "m" — Mass of the object (kg)
- "b" — Damping coefficient (Ns/m)
- "k" — Spring constant (N/m)
- "x" — Displacement (m)
- "F₀" — External force amplitude (N)
- "ω" — Driving angular frequency (rad/s)

The natural angular frequency is:

[
\omega_0=\sqrt{\frac{k}{m}}
]

Key Features

- Numerical simulation of forced harmonic oscillations
- Damped oscillation analysis
- Fourth-order Runge-Kutta (RK4) integration
- Position, velocity, and acceleration calculations
- Kinetic and potential energy analysis
- Frequency-response analysis
- Numerical estimation of resonance frequency
- Scientific visualization using Matplotlib

Technologies

- Python
- NumPy
- Matplotlib
- Jupyter Notebook

Project Structure

Oscillations-and-Resonance-Simulator/
│
├── Oscillations_and_Resonance.ipynb
├── README.md
├── .gitignore
├── LICENSE
│
└── images/
    ├── oscillation_analysis.png
    └── resonance_curve.png

Installation

Clone the repository:

git clone https://github.com/Ftmzahra-Hassani/Oscillations-and-Resonance-Simulator.git

Navigate to the project directory:

cd Oscillations-and-Resonance-Simulator

Install the required libraries:

pip install -r requirements.txt

Launch Jupyter Notebook:

jupyter notebook

Open "Oscillations_and_Resonance.ipynb" and run the notebook cells.

Simulation Parameters

The default simulation uses the following parameters:

Parameter| Value
Mass| 2.0 kg
Spring Constant| 40.0 N/m
Damping Coefficient| 0.5 Ns/m
Initial Position| 0.15 m
Initial Velocity| 0.0 m/s
External Force Amplitude| 5.0 N
Driving Frequency| 3.5 rad/s
Time Step| 0.01 s
Simulation Duration| 60 s

Visualizations

Oscillation and Energy Analysis

"Oscillation Analysis" (images/oscillation_analysis.png)

Resonance Curve

"Resonance Curve" (images/resonance_curve.png)

Numerical Method

The simulation uses the fourth-order Runge-Kutta method (RK4) to solve the coupled first-order differential equations derived from the original second-order equation of motion.

This numerical approach provides an approximation of the system's displacement and velocity over time.

The resonance frequency is estimated numerically by evaluating the steady-state oscillation amplitude over a range of driving frequencies.

Physical Interpretation

The simulator demonstrates how damping and external periodic forces influence the motion of a harmonic oscillator.

It also illustrates the resonance phenomenon, in which the system exhibits a large oscillation amplitude when the driving frequency approaches the resonance region.

The mechanical energy plotted in this project is the sum of the spring potential energy and kinetic energy. It is not conserved because of damping and external energy input.

Future Improvements

- Interactive parameter controls
- Animation of the mass-spring system
- Higher-resolution frequency analysis
- Comparison of different damping regimes
- Analytical versus numerical solution comparison

License

This project is licensed under the MIT License.

Author

Ftmzahra-Hassani

Engineering Physics Student | Python & Scientific Computing Enthusiast

GitHub: "@Ftmzahra-Hassani" (https://github.com/Ftmzahra-Hassani)

---

Developed for exploring classical mechanics through scientific Python.
