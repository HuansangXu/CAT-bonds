# Code for CAT Bond Pricing via Neual Networks and Analysis
## Julian Sester, Huansang Xu
This repository contains Jupyter Notebooks for modeling, pricing, and analyzing catastrophe (CAT) bonds using different loss distributions, including gamma and lognormal. It includes implementations of Monte Carlo simulations with and without Importance Sampling, Partial Integro-Differential Equations (PIDE), and Neural Network approximations.
## Abstract
In this paper, we propose an alternative valuation approach for CAT bonds where a pricing formula is learned by deep neural networks. Using these trained deep neural networks then allows to price CAT bonds in dependence of inputs that reflect the current market situation and the contract specifics. This has two main advantages, first, due to its expressiveness, upon being trained the neural networks allow the almost instant and accurate evaluation of the price, and second because of its fast execution the trained neural network can be easily analyzed to study its sensitivities w.r.t. changes of the underlying market conditions with direct implications for its risk management.
### Keywords: 
CAT-bonds, deep learning, importance sampling, sensitivities
## Repository Structure
| File                                        | Description                                                              |
| ------------------------------------------- | ------------------------------------------------------------------------ |
| `CAT_MC_IS_Gamma.ipynb`                     | Monte Carlo simulation with and without Importance sampling for CAT bond losses using Gamma distributions, analysis of IS parameters selection |
| `CAT_MC_IS_Lognormal.ipynb`                 | Monte Carlo simulation with and without Importance sampling for CAT bond losses using Lognormal distributions, analysis of IS parameters selection |
| `CAT_price_gamma.ipynb`                     | CAT bond pricing via MC simulation for Gamma distributed loss                       |
| `CAT_price_lognormal.ipynb`                 | CAT bond pricing via MC simulation for Lognormally distributed loss                   |
| `NN_gamma.ipynb`                            | Neural network training for CAT bond pricing with gamma losses, including optimal configuration and training results      |
| `NN_lognormal.ipynb`                        | Neural network training for CAT bond pricing with lognormal losses, including optimal configuration and training results   |
| `Computational_efficiency_gamma.ipynb`      | Efficiency tests for gamma-based simulation methods                      |
| `Computational_efficiency_lognormal.ipynb`  | Efficiency tests for lognormal-based simulation methods                  |
| `Computational_efficiency_PIDE_gamma.ipynb` | Computational efficiency analysis of PIDE method with gamma losses       |
| `Computational_efficiency_PIDE_log.ipynb`   | Computational efficiency analysis of PIDE method with lognormal losses   |
| `Sensitivity_analysis_gamma.ipynb`          | Sensitivity analysis of CAT bond pricing under gamma distribution        |
| `Sensitivity_analysis_log.ipynb`            | Sensitivity analysis of CAT bond pricing under lognormal distribution    |
## Purpose
This repository is part of a study exploring different numerical and machine learning approaches to CAT bond pricing and analysis, especially under non-Gaussian loss distributions. It includes computational comparisons and sensitivity tests.
