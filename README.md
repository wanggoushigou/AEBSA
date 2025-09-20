# README: High-Precision Parameter Estimation of Photovoltaic Models via AEBSA

## Abstract

This repository supports the paper *"High-Precision Parameter Estimation of Photovoltaic Models via a Novel Adaptive Elite Biased Backtracking Search Algorithm"*, which introduces the **Adaptive Elite Biased Backtracking Search Algorithm (AEBSA)** for accurate and efficient parameter identification in photovoltaic (PV) models. AEBSA enhances the standard BSA by integrating an elite-guided mutation strategy, Gaussian perturbation, and adaptive step-size adjustment, significantly improving convergence speed and avoiding local optima.

## Algorithm Overview

AEBSA is designed to address challenges in PV parameter estimation, such as high dimensionality, nonlinearity, and multiple local optima. Key features include:

- **Improved Mutation Strategy**: Uses optimal individual feedback to guide population evolution.
- **Elite-Guided Weighted Gaussian Perturbation**: Enhances local exploitation accuracy.
- **Experience Adjustment Strategy**: Dynamically balances exploration and exploitation.

## Implementation Details

- **Platform**: MATLAB 2023b
- **Hardware**: Intel® Core™ Processor (2.60 GHz, 16 GB RAM)
- **Population Size**: 20
- **Max Function Evaluations**: 20,000
- **Independent Runs**: 30

| Algorithm | Parameter setting                                            |
| --------- | ------------------------------------------------------------ |
| MLBSA     | NP=20                                                        |
| CLPSO     | NP=20, inertia weight w:0.9-0.2, acceleration coefficient c=1.49445,  refreshing gap m=5 |
| RLDE      | NP=20, CR=0.9, =0.1, =0.9                                    |
| ATLDE     | NP=20, CR=0.9, F=rand                                        |
| IJAYA     | NP=20                                                        |
| PGJAYA    | NP=20                                                        |
| AHJAYA    | NP=20, Q=0.3                                                 |
| CJAYA     | NP=20                                                        |
| BSA       | NP=20, mix rate=1                                            |
| AEBSA     | NP=20, mix rate=1                                            |