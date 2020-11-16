# Assignment 4, due November 23rd 2020

The goal of this assignment is to parallelize several applications with OpenMP.

## Exercise 1

### Tasks

- Use OpenMP to parallelize the Monte Carlo computation of π of Assignment 2.
- Measure the execution time for several problem sizes and for 1 to 8 threads.
- Illustrate the data in appropriate speedup/efficiency figures and discuss them. What can you observe? How does the performance compare to your MPI implementation of Assignment 2?
- Vary between the use of `atomic`, `critical`, and `reduction`, and vary between aggregating the intermediate `int` and final `float`/`double` data. What can you observe?
- Consider the performance-related topics discussed in the lecture so far. What optimization strategies would you choose and why?
- Add your best wall times for 10^8 samples for 1 and 8 threads in the comparison spreadsheet linked on Discord.

## Exercise 2

### Tasks

- Use OpenMP to parallelize the 2D heat stencil simulation of Assignment 3.
- Measure the execution time for several problem sizes and for 1 to 8 threads.
- Illustrate the data in appropriate speedup/efficiency figures and discuss them. What can you observe? How does the performance compare to your MPI implementation of Assignment 3?
- Consider the performance-related topics discussed in the lecture so far. What optimization strategies would you choose and why?
- Add your best wall times for N=4000x4000 and T=100 for 1 and 8 threads in the comparison spreadsheet linked on Discord.

## General Notes

All the material required by the tasks above (e.g. code, figures, etc...) must be part of the solution that is handed in. Your experiments should be reproducible and comparable to your own measurements using the solution materials that you hand in. For source code, please provide a makefile or other, intuitive means of compiling with the required flags and settings.

**Every** member of your group must be able to explain the given problem, your solution, and possible findings. You may also need to answer detailed questions about any of these aspects.

**Please run any benchmarks or heavy CPU loads only on the compute nodes, not on the login node.**
If you want to do some interactive experimentation, use an *interactive job* as outlined in the tutorial. Make sure to stop any interactive jobs once you are done.
