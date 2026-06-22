# Bayesian Decision Framework for IOL Power Selection

## Overview
This repository contains the complete Python code for a Monte Carlo simulation implementing a **Bayesian decision-theoretic framework** to resolve intraocular lens (IOL) power disagreements among six modern formulas: Cooke K6, EVO, Hill-RBF 3.0, Hoffer QST, Kane, and Pearl-DGS.  
The framework simulates 100,000 virtual eyes and compares Bayesian decision-making against alternative strategies such as MLE, median consensus, weighted consensus, Barrett-only, random selection, and always-myopic heuristics.

---

## Features
- **Monte Carlo Simulation**: 100,000 iterations for robust statistical inference.  
- **Bayesian Decision Framework**: Penalizes hyperopia more heavily than myopia to reflect clinical risk asymmetry.  
- **Comparative Strategies**: Benchmarks Bayesian decisions against multiple heuristics.  
- **Sensitivity Analyses**:
  - Hyperopia penalty variations (1.5×, 2×, 3×).  
  - Trigger thresholds (0.50 D, 0.75 D, 1.00 D).  
  - Correlated errors (ρ = 0.4).  
- **Clinical Case Example**: Demonstrates real-world application with ESCRS calculator outputs.  
- **Publication-Quality Figures**: Styled with Seaborn and Matplotlib.

---

## Requirements
- Python 3.8+  
- Libraries:
  - numpy  
  - pandas  
  - matplotlib  
  - seaborn  
  - scipy  

Install dependencies with:
```bash
pip install numpy pandas matplotlib seaborn scipy
```
---

## Usage
1. Clone the repository:
```bash
git clone https://github.com/your-repo/IOL-Bayesian-Framework.git
cd IOL-Bayesian-Framework
```

2. Run the notebook or script:
```bash
python bayesian_iol_simulation.py
```

3. Review outputs:

i. Tables of mean absolute error (MAE), refractive surprise rates, hyperopia/myopia distribution, and expected utility.

ii. Sensitivity analysis results.

iii. Clinical case example walkthrough.

---

## Results Summary
1. Bayesian framework consistently achieves the highest expected utility.

2. Reduces hyperopic outcomes compared to pure MLE and random selection.

3. Avoids excessive myopic bias seen in “always-myopic” heuristics.

4. Robust across penalty variations, trigger thresholds, and correlated error scenarios.

---

## Clinical Implications
This computational proof-of-concept demonstrates the potential of Bayesian methods to improve clinical decision-making in refractive cataract surgery.
Prospective clinical validation is required before adoption in practice.

---

## Citation
If you use this code or framework in your research, please cite the associated manuscript or repository:

Tan Aik Kah. "Monte Carlo Simulation: Bayesian Decision Framework for IOL Power Selection." GitHub Repository, 2026.




