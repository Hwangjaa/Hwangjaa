# Rafael Satriaprima Yudianto

Jakarta, Indonesia · Cybersecurity & applied machine learning

## About

I work at the intersection of security operations and machine learning. On the operations side, that means monitoring, triage, incident response, and reading logs carefully and acting on evidence rather than the first alert. On the research side, it means building detection models that hold up against realistic conditions: imbalanced data, drifting attack distributions, and the cost of false positives.

Currently pursuing a Master's in Computer Science at BINUS University, researching adaptive anomaly-based intrusion detection for IoT networks.

## Focus areas

- **Detection engineering** — designing and evaluating anomaly-based intrusion detection systems, from dataset preparation through metric-driven evaluation
- **Security operations** — SIEM monitoring and triage, threat hunting, incident response, vulnerability assessment, and patch management
- **Applied ML for security** — generative adversarial networks for class imbalance, explainability (SHAP) as an adaptive feedback signal, DGA classification

## Notable work

### [Wordlist DGA Detection — N-Gram + Linguistic Feature Fusion](https://github.com/Hwangjaa/dga-wordlist-detection)

Published research (ICCSCI 2026, Procedia Computer Science). Wordlist-based DGAs assemble domains from real English words, so they slip past entropy and single-type n-gram detectors — the baseline I started from scored 8.81% F1 on the Matsnu family. The method fuses n-gram statistics with linguistic features (pronounceability, vowel/consonant distribution, word reputation), then filters 48 candidates down to 12 through staged correlation analysis. Across seven classifiers on a 133k-domain Tranco/DGArchive corpus, LightGBM leads every family — Matsnu goes from 8.81% to 84.75% F1, binary detection reaches 98.94% AUC-ROC. The full experimental pipeline is in the repository.

### [SaffCoz — Fragrance Boutique](https://github.com/Hwangjaa/SaffCoz-FinalProject)

Static storefront built for a Human Computer Interaction course. The constraint I set for myself: no dead controls — every interactive element does something real, and where a backend would be required, the interface routes to a real channel instead of faking success. Cart, wishlist, and search state are handled entirely client-side. The documentation maps each of Shneiderman's 8 Golden Rules to a concrete implementation decision.

### SHAP-WGAN Intrusion Detection

Master's research, in progress. An anomaly-based network IDS built around two ideas: a WGAN generator that synthesises minority-class attack traffic to counter class imbalance, and SHAP attributions wired into a closed-loop feedback path so detection adapts as attack distributions drift. Evaluated on the N-BaIoT dataset against standard baselines. The repository is private while the thesis is in progress, but I'm happy to discuss the approach.

## Education

**Bina Nusantara University**

- Master Degree (Computer Science) — 2025 to present
- Bachelor Degree (Cybersecurity) — 2022 to 2025, GPA 3.49

## Contact

The fastest way to reach me is [LinkedIn](https://www.linkedin.com/in/rafael-satriaprima-yudianto-423068317).
