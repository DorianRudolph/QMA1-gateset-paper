# Towards a universal gateset for QMA₁

This repository contains a preprint of my upcoming paper.

## Errata

The argument containment of the clique homology problem in PSPACE in the paper is insufficient. Instead, we can check whether the homology is trivial by computing the rank of the Laplacian in NC(poly)=PSPACE using Chistov's algorithm:
- Chistov, A.L. (1985). Fast parallel calculation of the rank of matrices over a field of arbitrary characteristic. In: Budach, L. (eds) Fundamentals of Computation Theory. FCT 1985. Lecture Notes in Computer Science, vol 199. Springer, Berlin, Heidelberg. https://doi.org/10.1007/BFb0028792

## Supplementary material

- [gadget_2local.py](gadget_2local.py): Verify gadgets of the 2-local QMA1-complete Hamiltonian
- [gadget_4sat.py](gadget_4sat.py): Verify gadgets of the 4-SAT construction
- [gadget_homology.py](gadget_homology.py): Verify 2-local clique homology gadgets *algebraically* (and 3-local standard basis state)
- [clique_homology_gadgets_cpp/](clique_homology_gadgets_cpp/) Verify clique homology gadgets *numerically* and verify Euler characteristic.

The scripts require [SageMath](https://www.sagemath.org/) (tested with version 10.4).
The code was tested on macOS using the SageMath distribution [Sage_macOS](https://github.com/3-manifolds/Sage_macOS) and on Arch Linux using the `sagemath` package.
