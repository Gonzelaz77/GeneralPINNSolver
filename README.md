# GeneralPINNSolver
Construction of a Genetic PINN Solver for Simulation.

# Python Setup
 - python environment: 3.10.8
 - torch: 2.7.1+cu118
 - matplotlib: 3.10.3

# Project list

## Basic PINN
Solving a Laplacian problem on a unit square, where top and bottom boundary are Dirchlet boundary with value 1 and left and right boundary are Neumann boundary with value 0. The weight parameter between all losses(pde, boundary) are set as 1 for pde and 100 for boundary. The points of PINN are re-sampled for every 1000 epoches, where 50000 points are sampled with in the region and 10000 points are sampled on the boundaries. The network structure are 4 sets of linear+Tanh.

The maximum value is 2.25 with source term -10. and with 2000 epoches, the solution is accurate enough.
