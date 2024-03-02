---
title: Talk at prestigious ISC23 conference
date: '2023-05-24'
summary: m-Cubes An efficient and portable implementation of multi-dimensional integration for GPUs
---

[Link to Talk](https://app.swapcard.com/event/isc-high-performance-2023/planning/UGxhbm5pbmdfMTIyMTA2Mw==)

# Abstract

We present our experience in porting optimized CUDA implementations to oneAPI. We focus on the use case of numerical integration, 
particularly the CUDA implementations of PAGANI and m-Cubes. 
We faced several challenges that caused performance degradation in the oneAPI ports. 
These include differences in utilized registers per thread, compiler optimizations,
and mappings of CUDA library calls to oneAPI equivalents. After addressing those challenges, we tested both the PAGANI and m-Cubes integrators on numerous integrands of various characteristics. To evaluate the quality of the ports, we collected performance metrics of the CUDA and oneAPI implementations on the Nvidia V100 GPU. 
We found that the oneAPI ports often achieve comparable performance to the CUDA versions, and that they are at most 10% slower.
