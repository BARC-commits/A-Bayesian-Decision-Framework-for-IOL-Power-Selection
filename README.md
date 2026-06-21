# Bayesian IOL Power Selection: Monte Carlo Simulation

[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)

## Overview

This repository contains the complete Python code for the Monte Carlo simulation described in the manuscript:

> **"A Bayesian Decision Framework for IOL Power Selection: Balancing Formula Consensus with Asymmetric Clinical Risk"**

The simulation tests whether a Bayesian decision-theoretic framework can resolve clinically meaningful disagreements among modern IOL power formulas more effectively than pure maximum likelihood estimation (MLE), random selection, or the conventional "always-myopic" heuristic.

## Key Findings

- **Bayesian decision framework achieves the highest expected utility** (-0.282) vs. MLE (-0.302), Random (-0.717), and Always-Myopic (-0.646)
- **Reduces hyperopic outcomes from 50.0% to 42.5%** (15% relative reduction) while maintaining near-identical accuracy (MAE: 0.204 D vs. 0.201 D for MLE)
- **Avoids excessive myopic bias** (57.5% myopic vs. 98.4% for Always-Myopic)

## Formulas Included

The simulation models six contemporary formulas available on the ESCRS online calculator:

| Formula | SD (D) |
|---------|--------|
| Cooke K6 | 0.44 |
| EVO | 0.47 |
| Hill-RBF 3.0 | 0.48 |
| Hoffer QST | 0.50 |
| Kane | 0.48 |
| Pearl-DGS | 0.46 |

*SDs derived from the ESCRS calculator validation study (JCRS 2024).*

## Requirements

- Python 3.9+
- NumPy
- Pandas
- SciPy
- Matplotlib
- Seaborn

## Installation

```bash
git clone https://github.com/yourusername/bayesian-iol-simulation.git
cd bayesian-iol-simulation
pip install -r requirements.txt
```



## Usage

# Run the Simulation
```bash
python bayesian_iol_simulation.py
```
# Run in Jupyter Notebook
```bash
jupyter notebook bayesian_iol_simulation.ipynb
```

# Run in Kaggle

Copy the contents of bayesian_iol_simulation.py into a Kaggle notebook cell and run all cells.

## Output

The simulation generates:

1. Four summary tables showing MAE, refractive surprise rate, hyperopia vs. myopia rates, and expected utility for all strategies
2. Two publication-quality figures showing error distributions and performance comparison
3. A clinical case example from the ESCRS calculator
4. Statistical significance tests (paired t-tests, chi-square tests)


## Repository Structure
```bash
bayesian-iol-simulation/
├── bayesian_iol_simulation.py   # Main simulation script
├── bayesian_iol_simulation.ipynb # Jupyter notebook version
├── requirements.txt             # Python dependencies
├── README.md                    # This file
└── LICENSE                      # MIT License
```
## Citation

If you use this code in your research, please cite the associated manuscript:

Tan Aik Kah. "A Bayesian Decision Framework for IOL Power Selection: Balancing Formula Consensus with Asymmetric Clinical Risk."

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

ESCRS Calculator Validation Study Group for providing formula performance data


## Contact

For questions or comments, please open an issue or contact the corresponding author.

## Keywords:
Bayesian inference,
decision theory,
IOL power selection,
cataract surgery,
Monte Carlo simulation,
refractive outcomes,
ESCRS calculator


---

## Optional: requirements.txt

```txt
numpy>=1.21.0
pandas>=1.3.0
scipy>=1.7.0
matplotlib>=3.4.0
seaborn>=0.11.0
```

## MIT License

Copyright (c) 2026 [Tan Aik Kah]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.


