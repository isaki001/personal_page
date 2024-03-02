
---
title: Talk at prestigious ISC22 conference, m-Cubes A Monte Carlo GPU integrator
date: '2022-05-31'
summary: m-Cubes An efficient and portable implementation of multi-dimensional integration for GPUs
---

[Link] (https://app.swapcard.com/event/isc-high-performance-2022/planning/UGxhbm5pbmdfODYyODcy)

Our work on the development of the m-Cubes GPU accelerated numerical integrator, was published at ISC22. 
I had privilege of giving a talk about our software.

# Abstract

The task of multi-dimensional numerical integration is frequently encountered in physics and other scientic elds, e.g., 
in modeling the effects of systematic uncertainties in physical systems and in Bayesian parameter estimation. 
Multi-dimensional integration is often time-prohibitive on CPUs. 
Efficient implementation on many-core architectures is challenging as the workload across the integration space cannot be predicted a priori.
We propose m-Cubes, a novel implementation of the well-known Vegas algorithm for execution on GPUs. 
Vegas transforms integration variables followed by calculation of a Monte Carlo integral estimate using adaptive partitioning of the 
resulting space. m-Cubes improves performance on GPUs by maintaining relatively uniform work- load across the processors. 
As a result, our optimized Cuda implementation for Nvidia GPUs outperforms parallelization approaches proposed in past literature. 
We further demonstrate the efficiency of m-Cubes by evaluating a six-dimensional integral from a cosmology application, 
achieving signicant speedup and greater precision than the Cuba library's CPU implementation of Vegas. 
We also evaluate m-Cubes on a standard integrand test suite. Our approach yields a speedup of at least 10 when compared 
against publicly available Monte Carlo based GPU implementations. In summary, m-Cubes can solve integrals that are prohibitively
expensive using standard libraries and custom implementations. A modern C++ interface header-only implementation makes m-Cubes portable, 
allowing its utilization in complicated pipelines with easy to dene stateful integrals. Compatibility with non-Nvidia GPUs is achieved 
with our initial implementation of m-Cubes using the Kokkos framework.
