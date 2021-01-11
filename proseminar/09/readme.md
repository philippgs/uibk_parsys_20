# Assignment 09, due January 18th 2021

The goal of this assignment is to parallelize an unknown application using profiling and OpenMP.

## Exercise 1

### Description

The file [real.tar.gz](real.tar.gz) contains a realistic implementation of a (simple) numerical algorithm. Imagine you are tasked with making this implementation faster by parallelizing it with OpenMP, without any further information.

### Tasks

- Familiarize yourself with the code. You are not required to look at every source line, but rather profile the code using the means discussed in the lecture and get a grasp on its computational hotspots and performance characteristics (computation-heavy, memory-heavy, etc.).
- Investigate any loops that carry larger workloads and determine if and how they can be parallelized. Parallelize them with OpenMP. Ensure that any code modification does not violate program correctness with respect to its output.
- Benchmark the original, sequential program and your parallelized version for 1, 2, 4 and 8 threads on LCC2 and enter your results into the comparison spreadsheet linked on Discord..

## General Notes

All the material required by the tasks above (e.g. code, figures, etc...) must be part of the solution that is handed in. Your experiments should be reproducible and comparable to your own measurements using the solution materials that you hand in. For source code, please provide a makefile or other, intuitive means of compiling with the required flags and settings.

**Every** member of your group must be able to explain the given problem, your solution, and possible findings. You may also need to answer detailed questions about any of these aspects.

**Please run any benchmarks or heavy CPU loads only on the compute nodes, not on the login node.**
If you want to do some interactive experimentation, use an *interactive job* as outlined in the tutorial. Make sure to stop any interactive jobs once you are done.
