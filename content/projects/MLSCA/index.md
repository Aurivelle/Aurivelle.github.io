---
title: 'Generative AI for High-Fidelity Side-Channel Trace Simulation'
date: '2026-07-03'
summary: 'A diffusion-based side-channel study separating cryptanalytic utility from waveform and distribution fidelity across synthetic and public real AES traces.'
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

* **Controlled simulation:** Designed three increasingly difficult settings: aligned traces (V0), globally shifted traces (V1), and randomized physical leakage placement with byte-dependent amplitudes (V2).
* **Reverse-trajectory evaluation:** Recorded predicted-clean traces at all 400 reverse diffusion stages for V0 and V1 rather than evaluating only the final sample.
* **Attack-based evaluation:** Evaluated intermediate traces with Template-attack NTGE and CPA correct-key peak and margin.
* **Fidelity evaluation:** Tracked RMSE, NCC, DTW, Wasserstein-1, and Energy distance alongside attack-independent waveform and distribution quality.
* **Key observation:** Found that strong attack-exploitable leakage can emerge before full waveform and distribution fidelity is recovered.
* **Real-trace validation:** Validated the same attack pipeline on the public Mind the Portability software-AES traces and successfully recovered the targeted key bytes.
