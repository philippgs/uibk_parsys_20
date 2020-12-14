# Assignment 8, due January 11th 2021

The goal of this assignment is to implement and optimize two types of dwarfs using OpenMP.

## Exercise 1

### Tasks

- Use OpenMP to develop a parallel matrix multiplication program. In order to facilitate verification:
    - initialize matrix A with `a(i,j) = i * j`,
    - make matrix B the identity matrix (`b(i,j) = (i == j) ? 1 : 0`), 
    - use `double` as the element type, and 
    - only consider the actual matrix multiplication for your time measurements, not the initialization or any verification.
- Measure the execution time of your OpenMP program for several matrix sizes and for 1 and 8 threads.
- Illustrate the data in appropriate speedup/efficiency figures and discuss them. What can you observe?
- Try to maximize the performance by considering all sequential and parallelism-related optimizations we discussed so far. Which did you choose and why?
- Add your best wall times for 1 and 8 threads for `N = 3000` into the comparison spreadsheet linked on Discord.

## Exercise 2

### Description

N-queens is a popular branch-and-bound problem. The goal is to compute the number of possible ways to place N chess queens on a NxN chess board without them attacking each other. See https://en.wikipedia.org/wiki/Eight_queens_puzzle for further information.

### Tasks

- Implement a sequential version of the n-queens problem. Benchmark your program for several problem sizes (e.g. 8, 10, and 12). What can you observe?
- Parallelize your program using OpenMP. Which OpenMP constructs are suitable candidates and why?
- Benchmark your problem for several numbers of threads. What can you observe?
- Optional: Try to maximize the performance by considering all sequential and parallelism-related optimizations we discussed so far. Which did you choose and why?
- Add your best wall times for 1 and 8 threads for `N = 13` into the comparison spreadsheet linked on Discord.

## General Notes

All the material required by the tasks above (e.g. code, figures, etc...) must be part of the solution that is handed in. Your experiments should be reproducible and comparable to your own measurements using the solution materials that you hand in. For source code, please provide a makefile or other, intuitive means of compiling with the required flags and settings.

**Every** member of your group must be able to explain the given problem, your solution, and possible findings. You may also need to answer detailed questions about any of these aspects.

**Please run any benchmarks or heavy CPU loads only on the compute nodes, not on the login node.**
If you want to do some interactive experimentation, use an *interactive job* as outlined in the tutorial. Make sure to stop any interactive jobs once you are done.
