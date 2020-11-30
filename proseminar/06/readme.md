# Assignment 6, due December 07th 2020

The goal of this assignment is to implement your parallelization and optimization plan of the n-body simulation of Assignment 5 and experiment with load imbalance.

## Exercise 1

### Tasks

- Provide an OpenMP implementation of your parallelization and optimization plan for the n-body simulation of Assignment 5.
- Measure the speedup and efficiency for multiple problem and machine sizes as in previous exercises. If your parallelization and optimization are orthogonal code modifications, try to measure the impact of your optimization separately.
- Illustrate the data in appropriate figures and discuss them. What can you observe? Did the implementation meet your expectations from Assignment 5?
- Add your best parallel wall time for 8 threads, 10000 particles, and 100 time steps into the comparison spreadsheet linked on Discord.

## Exercise 2

### Tasks

- Modify your n-body simulation to introduce spatial load imbalance.
- Try to mitigate your newly introduced load imbalance using any means discussed so far, and measure your efforts.
- Illustrate the data in appropriate figures and discuss them. What can you observe?

## General Notes

All the material required by the tasks above (e.g. code, figures, etc...) must be part of the solution that is handed in. Your experiments should be reproducible and comparable to your own measurements using the solution materials that you hand in. For source code, please provide a makefile or other, intuitive means of compiling with the required flags and settings.

**Every** member of your group must be able to explain the given problem, your solution, and possible findings. You may also need to answer detailed questions about any of these aspects.

**Please run any benchmarks or heavy CPU loads only on the compute nodes, not on the login node.**
If you want to do some interactive experimentation, use an *interactive job* as outlined in the tutorial. Make sure to stop any interactive jobs once you are done.
