# Rafael Satriaprima Yudianto

Jakarta, Indonesia · Cybersecurity & applied machine learning

## About

I work on two sides of security. In operations, I did monitoring, triage, and incident response during a year in a SOC, where I learned that reading logs carefully beats trusting the first alert. In research, I build detection models and try to make them hold up under realistic conditions: imbalanced data, attack patterns that drift over time, and the real cost of false positives.

I'm now pursuing a Master's in Computer Science at BINUS University, researching adaptive anomaly-based intrusion detection for IoT networks.

## Focus areas

- Detection engineering: building and evaluating anomaly-based intrusion detection systems, from dataset preparation to metric-driven evaluation
- Security operations: SIEM monitoring, threat hunting, incident response, vulnerability assessment, patch management
- Applied ML for security: GANs for class imbalance, SHAP explainability as a feedback signal, DGA classification

## Notable work

### [Wordlist DGA Detection](https://github.com/Hwangjaa/dga-wordlist-detection)

My first published paper (ICCSCI 2026, Procedia Computer Science). Modern wordlist DGAs build domains out of real English words, so entropy and plain n-gram detectors barely notice them. The baseline I started from scored 8.81% F1 on the Matsnu family. My method fuses n-gram statistics with linguistic features like pronounceability and vowel/consonant distribution, then cuts 48 candidate features down to 12 through staged correlation analysis. Tested on a 133k-domain corpus from Tranco and DGArchive across seven classifiers. LightGBM came out on top for every family; Matsnu went from 8.81% to 84.75% F1 and binary detection reached 98.94% AUC-ROC. The full pipeline is in the repository.

### [SaffCoz, a fragrance storefront](https://github.com/Hwangjaa/SaffCoz-FinalProject)

Built for a Human Computer Interaction course. The rule I set for myself was simple: no dead controls. Every interactive element does something real, and where a real backend would be needed (payment, order database), the site routes to an actual channel like WhatsApp instead of faking a successful checkout. Cart, wishlist, and search all work client-side. The README maps each of Shneiderman's 8 Golden Rules to a concrete decision I made while building it.

### SHAP-WGAN Intrusion Detection

My master's thesis, still in progress. The idea is an anomaly-based network IDS with two components: a WGAN generator that synthesises minority-class attack traffic to deal with class imbalance, and SHAP attributions wired into a closed feedback loop so the detector adapts when attack distributions drift. It's being evaluated on the N-BaIoT dataset against standard baselines. The repository stays private until the thesis is done, but I'm happy to talk about the approach.

## Education

**Bina Nusantara University**

- Master Degree (Computer Science), 2025 to present
- Bachelor Degree (Cybersecurity), 2022 to 2025, GPA 3.49

## Contact

The fastest way to reach me is [LinkedIn](https://www.linkedin.com/in/rafael-satriaprima-yudianto-423068317).
