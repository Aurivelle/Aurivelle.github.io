---
title: 'Cryptography Engineering on Cortex-M4'
date: '2026-01-01'
summary: 'High-performance implementations of ML-KEM (post-quantum) and X25519 (ECDH) on ARM Cortex-M4.'
tags:
  - ARM Cortex-M4
  - Post-Quantum Cryptography
  - Assembly
  - ML-KEM
  - X25519
  - NTT
---

This project is the final project for **Cryptography Engineering (2025 Fall)** at National Taiwan University, lectured by Matthias J. Kannwischer. It focuses on aggressive performance optimization of two modern cryptographic primitives on resource-constrained embedded systems.

The project implements highly optimized versions of:
- **ML-KEM (FIPS 203)** — NIST's lattice-based post-quantum key encapsulation mechanism
- **X25519 (ECDH25519)** — Elliptic Curve Diffie-Hellman key exchange

**Target Platform:** ARM Cortex-M4 microcontroller  
**Constraints:** Constant-time execution, strict code-size budgets for NTT routines

### Key Optimizations

#### X25519 (ECDH25519)
* **Finite Field Arithmetic (mod p = 2^255 - 19):** Hand-optimized assembly for `fe25519_mul` (field multiplication) and `fe25519_sqr` (field squaring), achieving 81-85% cycle reduction.
* **Constant-Time Scalar Multiplication:** No secret-dependent branches or table indexing to prevent timing side-channel attacks.
* **Fixed-Base Acceleration:** Window method with precomputed tables using constant-time selection, reducing fixed-base scalar multiplication by **94.24%**.

#### ML-KEM (FIPS 203)
* **NTT/iNTT Kernels:** Optimized Number-Theoretic Transform operations with reduced memory traffic, layer fusion, and loop unrolling, achieving **2.85-3.79× speedup**.
* **Polynomial Arithmetic (mod q = 3329):** Leveraging ARMv7E-M DSP instructions (SIMD 16-bit operations) for packed polynomial addition/subtraction, **2-2.2× faster**.
* **Code-Size Budgeting:** NTT routines implemented under strict per-function size constraints while maintaining performance.


This project demonstrates deep understanding of low-level optimization, cryptographic algorithm engineering, and secure implementation practices on embedded ARM platforms.

* **[View Code on GitHub](https://github.com/Aurivelle/CryptographyEngineering)**
