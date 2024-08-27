---
title: "Test paper"
collection: publications
category: workshops
permalink: /publication/test
excerpt: 'This work builds a core language for Kokkos'
date: 2022-11-18
venue: '2022 IEEE/ACM Sixth International Workshop on Software Correctness for HPC Applications (Correctness)'
paperurl: 'http://feiyangjin.github.io/files/minikokkos.pdf'
citation: 'F. Jin, J. Jacobson, S. D. Pollard and V. Sarkar, "MiniKokkos: A Calculus of Portable Parallelism," 2022 IEEE/ACM Sixth International Workshop on Software Correctness for HPC Applications (Correctness), Dallas, TX, USA, 2022, pp. 37-44, doi: 10.1109/Correctness56720.2022.00010.'
---

Kokkos is a C++ library and ecosystem for writing parallel programs on heterogeneous systems. One of the primary goals of Kokkos is portability: programs in Kokkos are expressed through general parallel constructs which can enable the same code to compile and execute on different parallel architectures. However, there is no known formal model of Kokkos's semantics, which must be generic enough to support current and future CPU and accelerator architectures. As a first step of formalizing Kokkos, **We introduce MiniKokkos: a small language capturing the main features of Kokkos, and then prove that MiniKokkos ensures portability across all possible parallel executions.** We also provide a case study of how MiniKokkos can help reason about Kokkos programs and help find a bug in the Kokkos implementation.