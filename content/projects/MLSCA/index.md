---
title: 'Generative AI for High-Fidelity Side-Channel Trace Simulation'
date: '2026-07-03'
lastmod: '2026-10-05'
summary: 'A diffusion-based side-channel study separating cryptanalytic utility from waveform and distribution fidelity across controlled synthetic traces and four measured AES datasets.'
tags:
  - Research
  - ML-SCA
  - Side-Channel Analysis
  - Generative AI
  - Cryptography
  - Machine Learning
css_class: 'project-highlight'
---

This research began through the **NTU Global Connect Fellowship Program** at Nanyang Technological University and continues as a remote collaboration, supervised by Gwee Bah Hwee and Juncheng Chen. A manuscript is in preparation.

The project studies how attack-relevant leakage emerges during diffusion-based side-channel trace generation and whether cryptanalytic utility develops at the same rate as waveform and distribution fidelity.

### Experiments and Findings

* **Datasets:** Developed conditional DDPM experiments on controlled synthetic traces and four measured AES datasets.
* **Reverse-trajectory evaluation:** Evaluated predicted-clean traces across all 400 reverse-diffusion stages rather than only the final samples.
* **Attack-based evaluation:** Measured CPA-based key-recovery complexity throughout the reverse trajectory.
* **Fidelity evaluation:** Combined waveform and distribution distances with nearest-neighbor likelihood scoring.
* **Key observation:** Found that attack-relevant leakage can emerge substantially earlier than full distributional fidelity.
* **Masked traces:** Matching first-order marginals alone was insufficient to reproduce the cross-share dependence required for second-order attacks.
