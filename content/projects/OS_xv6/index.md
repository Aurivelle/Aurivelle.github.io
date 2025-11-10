---
title: 'Operating System Machine Problems (xv6)'
date: '2025-04-01' 
summary: 'A series of systems programming assignments involving C programming directly within the xv6 (RISC-V) kernel, implementing core OS features like threading, memory management, and file system extensions.'
tags:
  - C
  - Operating Systems
  - Kernel
  - Systems Programming
  - xv6
---

This project demonstrates core systems programming skills by modifying and extending the `xv6` educational operating system (RISC-V version).

As you noted, the task was not to build an OS from scratch, but to navigate the existing kernel codebase and implement complex features in the designated files—a challenge in managing kernel-space code, memory, and concurrency.

### Key Features Implemented

* **MP1 (User-level Threading):** Implemented a complete user-space threading library (`threads.c`), including thread creation, scheduling, and context switching.
* **MP2 (Kernel Memory Management):** Implemented a **Slab Allocator** (`slab.c`) directly within the kernel, providing an efficient memory allocation mechanism for kernel objects.
* **MP3 (Thread Scheduling):** Implemented a thread scheduler (`threads_sched.c`) to manage the execution order of user-level threads.
* **MP4 (File System Extension):** Added **Symbolic Link (symlink)** functionality to the xv6 file system by modifying kernel-level file system code, submitted as a `.patch` file.

You can view all my code contributions and modifications from the link below:

* **[View Code on GitHub](https://github.com/Aurivelle/operating-systems)**