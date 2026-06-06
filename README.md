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

## How to Run the Notebook
1. Open the `CIR_Yield_Curve_Project.ipynb` file.
2. You can click the **"Open in Colab"** badge at the top of the notebook to run it interactively in your browser.
3. Ensure that `train_data.csv`, `test_data.csv`, and `test_data_3M.csv` are uploaded to your default `/content/` directory in Colab before executing the cells.

**Submitted by:** [Your Name] | [Your Roll Number/ID]
