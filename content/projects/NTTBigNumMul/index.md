---
title: 'Multiplying Not-So-Big Integers with FFTs'
date: '2026-07-04'
lastmod: '2026-10-05'
summary: 'Two generations of constant-time NTT-based large-integer multiplication for Cortex-A76, with a crossover at or below 5,632 bits, OpenSSL RSA integration, and formal verification.'
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

This research project, **Finding and Pushing the Crossover on Large Modern OoO ARM CPUs**, studies where NTT-based multiplication becomes practical for not-so-big integer sizes. The first-author manuscript is under revision, and the work was accepted for presentation at the **CHES 2026 Poster Session**.

The project develops two generations of constant-time NTT-based multiplication for Cortex-A76. The second generation targets smaller operand sizes through tighter range bounds, redesigned 256/512-point NTT organization, fused reconstruction, and shorter carry and instruction-dependency chains.

### Key Features

* **NEON-optimized NTT kernels:** Developed constant-time fused NTT kernels in AArch64 assembly using ARM NEON instructions.
* **Multiplication pipeline:** Combined Barrett and Montgomery arithmetic, Good's trick, CRT reconstruction, and chunking and dechunking.
* **Crossover result:** The second-generation two-unknown-input multiplier outperforms target-tuned variable-time GMP by **6.25% at 5,632 bits** and **16.66% at 8,448 bits**, placing the observed crossover at or below 5,632 bits.
* **Montgomery multiplication:** The one-known-input implementation improves over OpenSSL's Neon path by **5.19%-44.40%** across the evaluated 5,120-10,240-bit sizes.
* **OpenSSL integration:** End-to-end RSA verification and encryption improve by **15.98%-51.58%** across RSA-5120, RSA-6144, RSA-8192, and RSA-10240.
* **Formal verification:** Verified optimized assembly kernels with CryptoLine for algebraic correctness, range safety, and equivalence after Slothy scheduling, then used HOL Light to compose higher-level multiplication specifications.
