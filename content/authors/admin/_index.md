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

      Developed conditional DDPM experiments on controlled synthetic traces and four measured AES datasets, evaluating predicted-clean traces across all 400 reverse-diffusion stages.

      Developed complementary evaluation pipelines using CPA-based key-recovery complexity, waveform and distribution distances, and nearest-neighbor likelihood scoring.

      Found that attack-relevant leakage can emerge substantially earlier than full distributional fidelity. On masked traces, matching first-order marginals alone was insufficient to reproduce the cross-share dependence required for second-order attacks.

  - position: Research Intern, Fast Crypto Lab
    company_name: "Academia Sinica"
    company_url: "https://www.iis.sinica.edu.tw/zh/index.html"
    icon: ""
    date_start: 2025-07-01
    date_end: ""
    summary: |
      First author of [Multiplying Not-So-Big Integers with FFTs: Finding and Pushing the Crossover on Large Modern OoO ARM CPUs](https://eprint.iacr.org/2026/2366), published as IACR ePrint 2026/2366 and accepted for the CHES 2026 Poster Session.

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
