---
# Display name
title: David Shu-Yu Wu

# Name pronunciation (optional)
name_pronunciation:

# Full name (for SEO)
first_name: David Shu-Yu
last_name: Wu

# Pronouns (optional)
pronouns:

# Status emoji
status:
  icon:

# Is this the primary user of the site?
superuser: true

# Highlight the author in author lists? (true/false)
highlight_name: true

# Role/position/tagline
role: CS Senior · Cryptographic Engineering

# Organizations/Affiliations to display in Biography blox
organizations:
  - name: National Taiwan University Computer Science and Information Engineering
    url: https://www.csie.ntu.edu.tw/
  - name: Academia Sinica
    url: https://www.citi.sinica.edu.tw/main

# Social network links
# Need to use another icon? Simply download the SVG icon to your `assets/media/icons/` folder.
profiles:
  - icon: at-symbol
    url: "mailto:b12902036@ntu.edu.tw"
    label: E-mail Me
  - icon: brands/github
    url: https://github.com/Aurivelle
  - icon: brands/linkedin
    url: https://www.linkedin.com/in/%E8%BF%B0%E5%AE%87-%E5%90%B3-44a1b22b0/

interests:
  - Cryptography
  - Cryptographic Engineering
  - Security
  - Side-Channel Analysis
  - Data Structures and Algorithms
headings:
  about: "Summary"
  education: "Education"
  interests: "Interests"
education:
  - area: "B.S. in Computer Science and Information Engineering; Minor in Atmospheric Sciences"
    institution: National Taiwan University
    icon: ""
    date_start: 2023-09-01
    date_end:
    summary: |
      Relevant coursework: Cryptography and Network Security, Post-Quantum Cryptography, Cryptographic Engineering, Cryptanalysis, Algorithm Design and Analysis, Advanced Data Structures, Probability, Discrete Mathematics, Automata and Formal Languages, Information Theory and Coding Techniques, Operating Systems, Computer Architecture, Machine Learning, Data Structures and Algorithms, System Programming, Linear Algebra, Computer Networks.


work:
  - position: Global Connect Fellow; Remote Collaborator
    company_name: "Nanyang Technological University"
    company_url: "https://www.ntu.edu.sg/eee"
    icon: ""
    date_start: 2026-07-01
    date_end: ""
    summary: |
      Selected for the NTU Global Connect Fellowship, a competitive international summer research program with an acceptance rate below 2%; supervised by Gwee Bah Hwee and Juncheng Chen. Continued the project as a remote collaborator after the July-August 2026 fellowship.

      Designed three controlled synthetic settings: aligned traces, globally shifted traces, and traces with randomized physical leakage placement and byte-dependent amplitudes.

      Recorded predicted-clean traces across all 400 reverse diffusion stages for the aligned and shifted settings. Evaluated them with Template-attack NTGE, CPA correct-key peak and margin, and fidelity metrics including RMSE, NCC, DTW, Wasserstein-1, and Energy distance.

      Observed that attack utility can emerge before full waveform and distribution fidelity is recovered. Validated the attack pipeline on the public Mind the Portability software-AES traces, where it successfully recovered the targeted key bytes.

  - position: Research Intern, Fast Crypto Lab
    company_name: "Academia Sinica"
    company_url: "https://www.iis.sinica.edu.tw/zh/index.html"
    icon: ""
    date_start: 2025-07-01
    date_end: ""
    summary: |
      Working on Multiplying Not-So-Big Integers with FFTs, an accepted CHES 2026 poster that studies the crossover point between GMP and NTT-based multiplication on large modern out-of-order ARM CPUs.

      Developed constant-time NEON-optimized NTT-based large-integer multiplication on AArch64, including fused NTT kernels, Barrett and Montgomery arithmetic, Good's trick, CRT reconstruction, and chunking and dechunking.

      Independently developed second-generation 5,632- and 8,448-bit multiplication paths on Cortex-A76. They outperform a target-tuned variable-time GMP baseline by 6.25% and 16.66%, respectively, placing the observed crossover at or below 5,632 bits.

      Integrated NTT-based Montgomery multiplication into OpenSSL RSA. Across RSA-5120, RSA-6144, RSA-8192, and RSA-10240, end-to-end verification and encryption improve by 15.98%-51.58%.

      Formally verified optimized assembly kernels with CryptoLine for algebraic correctness, range safety, and equivalence after Slothy scheduling; used HOL Light to compose higher-level multiplication specifications.

# Skills
# Add your own SVG icons to `assets/media/icons/`
skills:
  - name: Technical Skills
    items:
      - name: C, C++, Python
        description: ""
        percent: 90
        icon:
      - name: ARM Assembly + Intrinsics
        description: "AArch64 NEON and ARMv7E-M"
        percent: 70
        icon:
      - name: Cryptography Tooling
        description: "ARM NEON intrinsics, CryptoLine, SLOTHY"
        percent: 70
        icon:

languages:
  - name: Chinese
    percent: 100
  - name: English
    percent: 90
  - name: Spanish
    percent: 50

# Awards.
#   Add/remove as many awards below as you like.
#   Only `title`, `awarder`, and `date` are required.
#   Begin multi-line `summary` with YAML's `|` or `|2-` multi-line prefix and indent 2 spaces below.
awards:
---
