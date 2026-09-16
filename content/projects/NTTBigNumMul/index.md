---
title: 'Multiplying Not-So-Big Integers with FFTs'
date: '2026-07-04'
summary: 'A research project finding the crossover point between GMP and NTT-based multiplication on large modern out-of-order ARM CPUs, with NEON-optimized kernels, OpenSSL RSA benchmarking, and formal verification.'
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

This research project studies where NTT-based multiplication becomes practical for not-so-big integer sizes on large modern out-of-order ARM CPUs. The work was accepted as a poster at **CHES 2026**.

The project compares carefully engineered NTT-based multipliers against GMP across operand sizes such as 8k-14k bits, using ARM Cortex-A76 on Raspberry Pi 5 as the main evaluation platform. The work combines algorithm design, hand-written AArch64 assembly, reproducible benchmarking, and formal verification.

### Key Features

* **NEON-optimized NTT kernels:** Developed constant-time fused NTT kernels in AArch64 assembly using ARM NEON instructions.
* **Multiplication pipeline:** Combined Barrett and Montgomery arithmetic, Good's trick, CRT reconstruction, and chunking and dechunking.
* **Reproducible benchmarking:** Built unit-testing and benchmarking harnesses to compare cycle counts against GMP across multiple operand sizes.
* **OpenSSL integration:** Integrated the multiplier into OpenSSL RSA-8192/10240, improving verification, encryption, and KEM encapsulation by **36.0%-44.7%**.
* **Formal verification:** Verified optimized assembly kernels with CryptoLine for algebraic correctness, range safety, and equivalence after Slothy scheduling, then used HOL Light to compose higher-level multiplication specifications.
