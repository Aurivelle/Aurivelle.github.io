---
# Display name
title: David Wu

# Name pronunciation (optional)
name_pronunciation:

# Full name (for SEO)
first_name: David
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
  - name: Academia Sinica Research Center for Technology Innovation
    url: https://www.citi.sinica.edu.tw/main
  - name: Nanyang Technological University, EEE
    url: https://www.ntu.edu.sg/eee

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
  - area: BS Computer Science
    institution: National Taiwan University
    icon: ""
    date_start: 2023-06-15
    date_end:
    summary: |
      Relevant coursework: Cryptography and Network Security, Post-Quantum Cryptography, Cryptographic Engineering, Cryptanalysis, Algorithm Design and Analysis, Advanced Data Structures, Probability, Discrete Mathematics, Automata and Formal Languages, Information Theory and Coding Techniques, Operating Systems, Computer Architecture, Machine Learning, Data Structures and Algorithms, System Programming, Linear Algebra, Computer Networks.


work:
  - position: Research Intern, NTU Global Connect Fellowship
    company_name: "Nanyang Technological University"
    company_url: "https://www.ntu.edu.sg/eee"
    icon: ""
    date_start: 2026-07-01
    date_end: 2026-08-31
    summary: |
      Working on generative AI for high-fidelity side-channel trace simulation under the supervision of Gwee Bah Hwee.

      Reviewing profiling side-channel analysis literature, including masking, desynchronization, leakage modeling, data augmentation, and synthetic trace generation for cryptographic implementations.

      Studying how synthetic side-channel traces can augment profiling datasets and evaluate attack robustness in machine-learning-based side-channel analysis.

  - position: Research Intern, Fast Crypto Lab
    company_name: "Academia Sinica"
    company_url: "https://www.iis.sinica.edu.tw/zh/index.html"
    icon: ""
    date_start: 2025-07-01
    date_end: ""
    summary: |
      Working on Multiplying Not-So-Big Integers with FFTs, a project finding the crossover point between GMP and NTT-based multiplication on large modern out-of-order ARM CPUs.

      Implemented NEON-optimized NTT kernels and Barrett/Montgomery modular reduction in AArch64 assembly on ARM Cortex-A76, with reproducible unit tests and benchmarking harnesses.

      Integrated an NTT-based multiplier into OpenSSL RSA and benchmarked RSA-8192/10240 operations, improving public-key operations such as verification, encryption, and KEM encapsulation.

      Formally verified optimized large integer multiplication subroutines using CryptoLine and HOL Light.

# Skills
# Add your own SVG icons to `assets/media/icons/`
skills:
  - name: Technical Skills
    items:
      - name: C, C++, Python, Java
        description: ""
        percent: 90
        icon:
      - name: ARM Assembly + Intrinsics
        description: "AArch64 NEON and ARMv7E-M"
        percent: 70
        icon:
      - name: Cryptography Tooling
        description: "GMP, OpenSSL, CryptoLine"
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
