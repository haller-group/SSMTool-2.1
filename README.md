# SSMTool-2.0: Computation of invariant manifolds in high-dimensional mechanics problems
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4614201.svg)](https://doi.org/10.5281/zenodo.4614201)

This package computes invariant manifolds in high-dimensional dynamical systems using the Parametrization Method with special attention to the computation of Spectral Submanifolds (SSM) and forced response curves in finite element models. 

These invariant manifolds are computed in the physical coordinates using only the master modes resulting in efficient and feasible computations for high-dimensional finite-element problems. Additionally, the user has an option to choose among the graph or normal form style of parametrization. The computational methodology is described in the following article:

**S. Jain, G. Haller (2021) How to Compute Invariant Manifolds and their Reduced Dynamics in High-Dimensional Finite-Element Models? Preprint:** https://arxiv.org/abs/2103.10264

In this version, we demonstrate the computational methodology over small academic examples as well high-dimensional finite element problems using the FE package [4]. 
We have included a demonstration of SSM computation over the following finite element examples to compute forced response curves.

- Oscillator chain: two, three and n degrees of freedom. 
- Bernouli beam: modeled using linear finite elements with localized nonlinearity in the form of a cubic spring
- von Karman straight beam in 2D: geometrically nonlinear finite element model with and without **internal resonances** (IR)
- von Karman plate in 3D: geometrically nonlinear finite element model of a flat plate with and without **parallel computing**  
- von Karman shell-based shallow curved panel in 3D: geometrically nonlinear finite element model
- Prismatic beam: nonlinear beam PDE discretized using Galerkin method onto a given number of modes.
- NACA airfoil based aircraft wing model: shell-based nonlinear finite element model containing more than 100,000 degrees of freedom. 

This package uses the following external open-source packages:

1. Continuation core (coco) https://sourceforge.net/projects/cocotools/
2. Sandia tensor toolbox: https://gitlab.com/tensors/tensor_toolbox
3. Combinator: https://www.mathworks.com/matlabcentral/fileexchange/24325-combinator-combinations-and-permutations
4. YetAnotherFECode: Zenodo http://doi.org/10.5281/zenodo.4011281

In order to install the program, simply run the install.m file in the main folder. The examples can be found in the examples directory.
Note: When running the examples in the livescript files (workbooks), please ensure that the MATLAB 'Current Folder' is the directory of the specific example.

Please report any issues/bugs to Shobhit Jain shjain@ethz.ch

