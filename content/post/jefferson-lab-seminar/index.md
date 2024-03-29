---
title: My talk at Jefferson National Laboratory
date: '2022-04-18'
summary: Watch the recorderd presentation for the seminar.
---

[Click here for recording](https://www.jlab.org/video/cake-seminar-ioannis-sakiotis)

# Abstract
The task of multi-dimensional numerical integration is frequently encountered in physics and other scientific fields. High computational intensity causes existing libraries to often require prohibitively long execution times on challenging integrands. Adaptive algorithms have demonstrated the best performance on serial systems, but efficient many-core utilization is difficult to achieve because the adaptive workload can vary greatly across the integration space and is impossible to predict a priori. As a result, there a shortage of efficient and robust parallel numerical integration libraries. We present PAGANI and m-Cubes, two algorithms tailored for GPU execution, based on the popular Cuhre and VEGAS algorithms. PAGANI utilizes quadrature techniques while m-Cubes is Monte Carlo based. Different integrand characteristics can make either algorithm more appropriate, but both offer high-performance solutions to multi-dimensional integrands. CUDA implementations executed on a V100 GPU show orders of magnitude speedup over the serial algorithms as well superior reliability and performance over other deterministic and probabilistic GPU implementations. Finally, a modern C++ interface header-only implementation makes both algorithms portable, allowing their utilization in complicated pipelines with easy to define stateful integrals and without requiring knowledge of either parallel or CUDA programming constructs.

