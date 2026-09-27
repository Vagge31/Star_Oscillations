# Star Oscillations — Interactive Mode Visualizer

An interactive browser-based visualizer for Newtonian stellar oscillations in an $n=3$ polytrope, built using vanilla HTML5 Canvas and JavaScript. 

The tool directly plots the numerical eigenfunctions $\xi_r(r)$ and $\xi_h(r)$ and animates the corresponding stellar cross-section deformations using exact numerical data obtained via the shooting method.

## Physics & Numerical Background

The simulation demonstrates small adiabatic oscillations of a Newtonian star modeled with an $n=3$ Lane-Emden polytropic background[cite: 3]. The oscillation modes are classified by their restoring forces and spatial structure:

- **Radial Mode ($l=0$):**
  - **Fundamental Radial Mode ($f, l=0$):** Homologous volume breathing ($\omega^2 \approx 9.2638$) without radial nodes.
- **Non-Radial Modes ($l=2, m=0$):**
  - **Gravity Modes ($g_1, g_2$):** Buoyancy-driven oscillations dominated in the deep core.
  - **Fundamental Surface Mode ($f, l=2$):** Surface gravity wave resulting in quadrupolar spheroidal deformation ($\omega^2 \approx 9.5157$).
  - **Pressure / Acoustic Modes ($p_1, p_2$):** Compressional acoustic modes dominated in the outer stellar envelope.

## Features

- **Interactive Cross-Section Deformation:** Real-time meridional mesh showing fluid element displacements ($\xi_r, \xi_h$) modulated by Legendre polynomials $P_l(\cos\theta)$.
- **Live Eigenfunction Profiles:** Simultaneous plotting of the radial displacement $\xi_r(x)$ and horizontal displacement $\xi_h(x)$ across the dimensionless stellar radius $x = r/R$.
- **Interactive Controls:** Dynamic playback, speed adjustment, and amplitude scaling.
- **Zero Dependencies:** Pure HTML5 Canvas and JavaScript without external libraries or frameworks.

## Live Demo

Run the visualization directly in your browser:  
👉 **[https://Vagge31.github.io/Star_Oscillations/](https://Vagge31.github.io/Star_Oscillations/)**

## Usage

Simply clone the repository and open `index.html` in any modern web browser:

```bash
git clone https://github.com/Vagge31/Star_Oscillations.git
cd Star_Oscillations
# Open index.html directly or host locally
