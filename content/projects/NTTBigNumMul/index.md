---
title: 'Multiplying Not-So-Big Integers with FFTs'
date: '2025-07-01'
summary: 'An ongoing research project finding the crossover point between GMP and NTT-based multiplication on large modern out-of-order ARM CPUs, with NEON-optimized kernels, OpenSSL RSA benchmarking, and formal verification.'
tags:
  - Research
  - Arm Neon
  - ARM Cortex-A76
  - Assembly
  - NTT
  - OpenSSL
  - CryptoLine
css_class: 'project-highlight'
---

This ongoing research project studies where NTT-based multiplication becomes practical for not-so-big integer sizes on large modern out-of-order ARM CPUs.

The project compares carefully engineered NTT-based multipliers against GMP across operand sizes such as 8k-14k bits, using ARM Cortex-A76 on Raspberry Pi 5 as the main evaluation platform. The work combines algorithm design, hand-written AArch64 assembly, reproducible benchmarking, and formal verification.

### Key Features

* **NEON-optimized NTT kernels:** Implemented NTT kernels and modular reduction routines using AArch64 assembly and ARM NEON instructions.
* **Reduction engineering:** Used Barrett and Montgomery reduction with careful register allocation and range-bound reasoning.
* **Reproducible benchmarking:** Built unit-testing and benchmarking harnesses to compare cycle counts against GMP across multiple operand sizes.
* **OpenSSL integration:** Integrated an NTT-based multiplier into OpenSSL RSA and benchmarked RSA-8192/10240 operations, improving public-key operations such as verification, encryption, and KEM encapsulation.
* **Formal verification:** Verified optimized large integer multiplication subroutines with CryptoLine and HOL Light, including algebraic correctness, range bounds, and equivalence to optimized implementations.

To be continued...
