# cir-yield-curve-modeling
Implementation and critical analysis of the CIR and CIR++ short-rate models for yield curve reconstruction
# Stochastic Interest Rate Modelling (CIR & CIR++)

## Overview
This repository contains the implementation, calibration, and critical analysis of the Cox-Ingersoll-Ross (CIR) and CIR++ short-rate models. The objective of this project is to reconstruct the global yield curve (3M to 30Y) utilizing only the 3-Month instantaneous short rate as an observable input.

## Key Features
* **Data Engineering:** Robust forward/backward interpolation of historical yield data.
* **Base CIR Calibration:** Object-Oriented implementation using L-BFGS-B optimization to extract structural parameters ($\kappa, \theta, \sigma$) while strictly enforcing the Feller condition.
* **CIR++ Extension:** Implementation of the Brigo-Mercurio deterministic shift to exactly fit the initial term structure.
* **Critical Analysis:** Comparative backtesting demonstrating the 1-factor limitations of the model on the 5Y-30Y curve (Level, Slope, Curvature) and proving the out-of-sample overfitting trap of the CIR++ extension.

