# PK-PD-Tutorial-and-Python-Implementation

I had used the slides provided by Dr. Matthias König of Humboldt-University Berlin Systems Medicine of the Liver
koenigmx@hu-berlin.de
https://livermetabolism.com
To understand the concept of Pk/PD modeling.
In addition to this, I have also followed the textbook Applied Biopharmaceutics and PHARMACOKINETICS by LEON SHRGEL, ANDREW B.C. YU of MC GRAW Hil EDUCATION



# Population PK/PD Modeling and Exposure–Response Simulation
https://github.com/pawanthapaliya01/PK-PD-Tutorial-and-Python-Implementation/blob/main/population-pkpd-modeling.ipynb

## Overview

This project demonstrates a reproducible pharmacometric-style modeling
workflow using synthetic data.

The project was developed as a quantitative modeling portfolio project
to demonstrate concepts in pharmacokinetics, pharmacodynamics,
population variability, simulation, parameter estimation, and
exposure–response analysis.

## Objectives

- Develop a one-compartment pharmacokinetic model
- Simulate a virtual patient population
- Incorporate inter-individual variability
- Simulate residual unexplained variability
- Estimate population PK parameters
- Evaluate model predictions
- Calculate exposure metrics
- Implement an Emax pharmacodynamic model
- Perform exposure–response analysis
- Perform Monte Carlo population simulation
- Evaluate dose-exposure-response relationships

## Methods

### Pharmacokinetic model

A one-compartment IV bolus model was used:

dA/dt = -kA

where:

k = CL/V

and:

C(t) = A(t)/V

### Population variability

Individual clearance and volume were simulated using log-normal
inter-individual variability:

CL_i = CL_pop × exp(η_CL)

V_i = V_pop × exp(η_V)

### Pharmacodynamic model

An Emax exposure-response model was implemented:

E = E0 + Emax × AUC / (EC50 + AUC)

## Software

- Python
- NumPy
- Pandas
- SciPy
- Matplotlib
- Scikit-learn
- Seaborn

## Outputs

The project generates:

- Individual PK profiles
- Population PK profile
- Observed vs predicted diagnostics
- Residual diagnostics
- AUC distributions
- Cmax distributions
- Half-life distributions
- Exposure-response curves
- Dose-response simulations
- Monte Carlo exposure simulations

## Important Note

All datasets in this project are synthetic and generated for educational
and portfolio purposes. No clinical trial or patient data are used.

## Author

Pawan Kumar Thapaliya
