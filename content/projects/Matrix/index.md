---
title: 'C-Based Thread Pool for Matrix Multiplication'
date: '2024-12-01' # <--- (1) 請改成您做這個專案的大致日期
summary: 'A systems programming project to build a high-performance thread pool from scratch in C using pthreads (mutexes, condition variables) to parallelize matrix operations.'
tags:
  - C
  - Systems Programming
  - Concurrency
  - pthreads
  - HPC
---

This project is a high-performance, general-purpose **Thread Pool** built from scratch in C, designed to parallelize computationally intensive tasks.

The core of the project is the `tpool` (thread pool) module, which manages a set of worker threads to execute tasks from a concurrent work queue.

### Key Features

* **Built From Scratch:** Implemented a complete thread pool library (`tpool.c`, `tpool.h`) using POSIX Threads (pthreads).
* **Complex Synchronization:** Utilized low-level synchronization primitives, including **mutexes (`pthread_mutex_t`)** and **condition variables (`pthread_cond_t`)**, to create a thread-safe, blocking task queue.
* **Application & Benchmarking:** Applied the thread pool to accelerate a real-world problem—matrix multiplication—by distributing the computational load across multiple threads, verified by a custom judge (`judge.c`).

You can view the complete source code from the link below:

* **[View Code on GitHub](https://github.com/Aurivelle/multithreaded-matrix-machine)**