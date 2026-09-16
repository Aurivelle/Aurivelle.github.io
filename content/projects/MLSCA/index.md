---
title: 'Generative AI for High-Fidelity Side-Channel Trace Simulation'
date: '2026-07-03'
summary: 'A research project on using generative AI and synthetic trace generation to augment profiling datasets and evaluate robustness in machine-learning-based side-channel analysis.'
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

The project studies how attack-relevant leakage emerges during diffusion-based side-channel trace generation and whether cryptanalytic utility develops at the same rate as waveform fidelity.

### Experiments and Findings

* **Controlled simulation:** Built synthetic side-channel datasets and conditional DDPM experiments spanning a 400-stage reverse diffusion process.
* **Attack-based evaluation:** Evaluated intermediate traces with Template-attack NTGE and CPA correct-key peak and margin.
* **Fidelity evaluation:** Tracked RMSE, NCC, DTW, Wasserstein-1, and Energy distance alongside attack-independent waveform and distribution quality.
* **Key observation:** Found that attackability can peak before full waveform fidelity is recovered, revealing a temporal separation between cryptanalytic utility and trace fidelity.
