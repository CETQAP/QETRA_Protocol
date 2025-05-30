# QETRA Protocol

**Quantum Eavesdropping Tamper Recognition Algorithm (QETRA)**  
**Developed by:** Dr. Zuhair Ahmed  
**Institute:** Centre of Excellence for Technology Quantum and AI (CETQAP), Canada  
**Date:** May 30, 2025  
**License:** [Specify License, e.g., MIT, Apache 2.0]

---

## Overview

The QETRA Protocol introduces a novel approach to detect eavesdropping in quantum key distribution (QKD) using classical Support Vector Machines (SVM). It is the first known implementation of a classical machine learning algorithm on real quantum hardware (IBM Quantum's Brisbane backend) for this purpose, bridging the domains of classical ML and quantum cryptography.

---

## Key Features

- Detects eavesdropping in QKD using classical SVM
- Achieved 94% recall and F1-score of 0.9495
- Tested on real quantum hardware (IBM Quantum Brisbane)
- Compares favorably with BB84, quantum ML, and QSVM approaches
- Offers a practical solution for enhancing QKD security on NISQ-era devices

---

## Results Summary

| Metric                  | Value     |
|-------------------------|-----------|
| Accuracy                | 95%       |
| Precision               | 95.92%    |
| Recall                  | 94%       |
| F1-Score                | 0.9495    |
| Tampered Detection Rate | 94%       |
| False Alarm Rate        | 4%        |
| Live Test Confidence    | 99.7%     |

---

## Experimental Setup

- Quantum Platform: IBM Quantum (Brisbane Backend)
- Classical ML Tool: Scikit-learn (v1.2.2)
- Quantum SDK: Qiskit (v0.43.0)
- ML Model: Support Vector Machine (SVM) with grid search optimization
- Data: Quantum circuit measurements labeled as secure or tampered
- Train-Test Split: 70:30 with 5-fold cross-validation

---

## Data Availability

All data used for training and evaluation is available in this repository, including:

- Raw measurement results in JSON format
- Frequency-distribution training sets
- SVM training notebook and configuration

## Getting Started

### Prerequisites

- Python 3.9+
- Qiskit 0.43.0
- Scikit-learn 1.2.2

### Installation

```bash
git clone https://github.com/CETQAP/QETRA_Protocol.git
cd QETRA_Protocol
pip install -r requirements.txt
```

### Run the Notebook

```bash
jupyter notebook QETRA_SVM.ipynb
```

---

## References

1. Bennett & Brassard (1984). Quantum cryptography: BB84.
2. Harrow, Hassidim & Lloyd (2009). Quantum algorithm for linear systems.
3. Shor (1994). Algorithms for quantum computation.
4. IBM Quantum. Brisbane Backend Documentation.

---

## License

This work is licensed under [YOUR LICENSE HERE].

---

## Acknowledgements

- IBM Quantum for access to hardware.
- Quantum community for insightful discussions.

---

## Disclaimer

IBM had no role in the study design, data analysis, or interpretation.
