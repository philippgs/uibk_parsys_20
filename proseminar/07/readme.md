# Assignment 7, due December 14th 2020

The goal of this assignment is to explore shared memory MPI and hybrid parallelization.

## Exercise 1

### Tasks

- Implement a hybrid parallel version of any of the 1D/2D/3D heat stencil implementations, using MPI+OpenMP. For simplicity, you can assume periodic boundary conditions.
- Vary your rank and thread setup (e.g. one rank per node, one rank per CPU, etc.). What performance effects did you expect and what effects can you observe? How does the performance compare to your MPI-only implementation?
- Add error handling to your code by checking all return values of MPI function calls.

## Exercise 2

- Modify your implementation of exercise 1 using MPI one-sided shared memory communication instead of OpenMP for intra-node parallelism.
- Is there any performance difference to your implementation of exericse 1? How do the implementations compare in terms of effort?

## General Notes

All the material required by the tasks above (e.g. code, figures, etc...) must be part of the solution that is handed in. Your experiments should be reproducible and comparable to your own measurements using the solution materials that you hand in. For source code, please provide a makefile or other, intuitive means of compiling with the required flags and settings.

**Every** member of your group must be able to explain the given problem, your solution, and possible findings. You may also need to answer detailed questions about any of these aspects.

**Please run any benchmarks or heavy CPU loads only on the compute nodes, not on the login node.**
If you want to do some interactive experimentation, use an *interactive job* as outlined in the tutorial. Make sure to stop any interactive jobs once you are done.
