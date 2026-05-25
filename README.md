# An optimal first-order method for smooth and strongly convex composite optimization and its stationary limit

This repository contains code for reproducing and verifying the main results of:

> [1] Manu Upadhyaya, Daniel Berg Thomsen, Aymeric Dieuleveut, and Adrien Taylor.
> "[An optimal first-order method for smooth and strongly convex composite optimization and its stationary limit](https://arxiv.org/abs/2605.22929),"
> arXiv:2605.22929, 2026.

## Authors

- [Manu Upadhyaya](https://manuupadhyaya.github.io/)
- [Daniel Berg Thomsen](https://bergthomsen.com/)
- [Aymeric Dieuleveut](http://www.cmap.polytechnique.fr/~aymeric.dieuleveut/)
- [Adrien Taylor](https://www.di.ens.fr/~ataylor/)

## Repository Organization

- `numerical_validation/prox_item_tmm_pepit.ipynb`: PEPit worst-case analyses for finite-step Prox-ITEM and Prox-TMM bounds.
- `numerical_validation/prox_item_autolyap.ipynb`: AutoLyap iteration-dependent validation of the finite-horizon Prox-ITEM distance bound.
- `numerical_validation/prox_tmm_autolyap.ipynb`: AutoLyap iteration-independent validation of the stationary Prox-TMM rate.
- `symbolic_verification/prox_item_lyapunov_sympy.ipynb`: SymPy verification of the Prox-ITEM Lyapunov simplification.
- `symbolic_verification/prox_tmm_lyapunov_sympy.ipynb`: SymPy verification of the stationary Prox-TMM Lyapunov simplification.
- `symbolic_verification/prox_item_proof_mathematica.nb`: Mathematica verification of the Prox-ITEM proof reformulation.

## Requirements

The Python notebooks require Jupyter with the packages used in each notebook:

- [SymPy](https://www.sympy.org/en/index.html) for symbolic verification.
- [PEPit](https://github.com/PerformanceEstimation/PEPit/) and NumPy for PEPit numerical validations.
- [AutoLyap](https://autolyap.github.io/), NumPy, and Matplotlib for AutoLyap numerical validations.

The Mathematica notebook was created with Mathematica 13.3.
