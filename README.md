# Generation and Parameter Estimation of 2D Stable Distributions

## Overview
This project explores the simulation, visualization, and parameter estimation of two-dimensional stable distributions and sub-Gaussian vectors. It includes custom statistical generators and estimators to analyze the impact of the stability index $\alpha$ and spectral measure $\Gamma$ on the behavior of heavy-tailed bivariate data.

## Features
* **2D stable vector generator:** Simulates symmetric, independent, and dependent asymmetric stable vectors based on defined discrete spectral measures.
* **Sub-Gaussian vector generator:** Implements a robust generator for 2D sub-Gaussian random vectors.
* **Parameter estimation:** Estimates the stability index $\alpha$ using a log-log regression tail estimator, and estimates the spectral measure $\Gamma$ by analyzing the directional distribution of tail behavior.
* **Characteristic function analysis:** Computes and visualizes the empirical characteristic function (real and imaginary parts) and calculates the estimation error against theoretical values.
* **Codifference estimation:** Calculates the codifference $\tau$ to measure the dependency between vector components.
* **Optimal threshold selection:** Script designed to dynamically determine the optimal tail cut-off threshold $R$ for spectral measure estimation by minimizing the MSE.

## Files & Usage
* `main.qmd`: The main Quarto document containing all Python/R code, mathematical formulas, and the full analysis.
* To execute the code and generate the PDF report, run the following command in terminal:
  ```bash
  quarto render main.qmd