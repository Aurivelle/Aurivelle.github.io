---
title: 'Big Integer Multiplication in NTT'
date: '2025-11-01' 
summary: 'An ongoing research project aiming to find the crossover point between GMP’s flexible algorithms and our NTT  implementation on Arm A-profile CPUs. Employing engineering procedure such as unit tests and benchmarking on our implementation, also doing pipelining and optimization using hand-written assembly without compiler.'
tags:
  - Arm Neon
  - Assembly
  - NTT
  - Engineering
css_class: 'project-highlight'
---

Multiplication on big integers is one of the most important operations in classical or post-quantum cryptography engineering. However, recent researches focus mainly on those resource-constraint microcontrollers such as ARM M-profile CPUs.
On the other hand, although with desirable asymptotic complexity, Number-Theoretic Transform(NTT) performs surprisingly worse in practical than Karatsuba or naive quadratic complexity Schoolbook. It is important to find where do theory and practice match in reality.
Our goal is to combine previous concepts, algorithm techniques, and NTT variants on ARM A-profile CPUs to find and help optimize multiplication above certain bounds, and lay a solid foundation for future performance improvement on these processors.

### Key Features

* **Parameters Selection:** Carefully choosing parameters and bound estimation for primes and polynomial length in the convenient of lazy reduction to achieve a more efficient multiplication scheme.
* **Reductions:** Employing efficient Montgomery and Barrett reductions with clever register usage.
* **Zero Skipping:** Despite the permutation by Good's trick, we take advantage of half 0s to do efficient vectorized operations with post-processing using twist factors.

The repo is private for now.
