# 2D Natural Convection in a Square Enclosure - MATLAB CFD Solver

This repository contains a 2D Incompressible Computational Fluid Dynamics (CFD) solver developed in **MATLAB** to simulate **Natural Convection in a Square Enclosure** driven by buoyancy forces. 

The solver integrates the **Navier-Stokes equations** with the **Energy Equation** using the **Boussinesq Approximation**, discretized on a **Staggered Grid** via the **SIMPLE Algorithm**.

### Problem Description & Physics

Natural convection in a closed square cavity with differentially heated vertical walls and adiabatic horizontal walls is a classic benchmark problem in CFD and heat transfer.
- Left Wall: Hot (T(hot))
- Right Wall: Cold ((cold))
- Top & Bottom Walls: Adiabatic
- Driving Force: Buoyancy force induced by temperature-dependent density variations (Boussinesq Approximation).

The flow behavior and heat transfer rates are dictated by the dimensionless Rayleigh Number (Ra) and Prandtl Number (Pr).

### Numerical Methodology

- Governing Equations: 2D Incompressible Navier-Stokes + Energy Equation
- Density Coupling: Boussinesq Approximation
- Grid Structure: Staggered Grid
- Algorithm: SIMPLE (Semi-Implicit Method for Pressure-Linked Equations) for pressure-velocity coupling.
- Discretization: Finite Volume Method (FVM) with Central Difference / Upwind schemes.
- Heat Transfer Analysis: Local and average Nusselt Numbers (Nu) calculated along the heated wall.

### Results & Visualization

The solver evaluates the flow fields and temperature contours at different Rayleigh numbers, whereas the benchmark study is performed only for Rayleigh = 10^4.

- Isotherms (Temperature Contours): Transition from conduction-dominated (horizontal isotherms at low Ra) to convection-dominated regimes (boundary layers and vertical stratification at high Ra).
- Streamlines & Velocity Fields: Formation of primary central circulation cell and secondary corner vortices at elevated Rayleigh numbers.
- Nusselt Number Validation: Heat transfer performance validated against benchmark literature (de Vahl Davis, 1983).

[Isotherms]<img width="821" height="751" alt="isotherms" src="https://github.com/user-attachments/assets/861aea45-1a94-4b52-b774-e754f88fba7b" />

