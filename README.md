# Dimensionality Reduction Techniques

In this repository, we explore various dimensionality reduction techniques using Jupyter Notebooks. These techniques are essential for handling high-dimensional data and improving model performance. This project is designed to help data scientists and machine learning practitioners understand and implement these methods effectively.

## Table of Contents
- [Features](#features)
- [How It Works](#how-it-works)
- [Technology Stack](#technology-stack)
- [Requirements](#requirements)
- [Installation](#installation)
- [Configuration](#configuration)
- [Quick Start](#quick-start)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Development](#development)
- [Limitations](#limitations)
- [License](#license)

## Features
### Principal Component Analysis (PCA)
- **What it does:** PCA is a statistical procedure that uses an orthogonal transformation to convert a set of observations of possibly correlated variables into a set of values of linearly uncorrelated variables called principal components.
- **Why it exists:** It helps in reducing the dimensionality of data while retaining most of its variance, making it easier to visualize and analyze.

### t-Distributed Stochastic Neighbor Embedding (t-SNE)
- **What it does:** t-SNE is a machine learning algorithm for visualizing high-dimensional data. It converts similarities between data points into joint probabilities and tries to minimize the Kullback-Leibler divergence between these distributions.
- **Why it exists:** It is particularly well-suited for the visualization of high-dimensional datasets, making complex patterns more apparent.

### PCA in Pipeline with SVM
- **What it does:** This notebook demonstrates how to integrate PCA into a machine learning pipeline using Support Vector Machines (SVM).
- **Why it exists:** It provides a practical example of how dimensionality reduction can be used to improve the performance of machine learning models.

## How It Works
The project consists of three Jupyter Notebooks, each focusing on a different dimensionality reduction technique. The notebooks are structured as follows:

1. **Principal Component Analysis (PCA):** Introduces PCA and demonstrates its application using a sample dataset.
2. **t-Distributed Stochastic Neighbor Embedding (t-SNE):** Explains t-SNE and provides an example of its use.
3. **PCA in Pipeline with SVM:** Integrates PCA into a machine learning pipeline to improve the performance of an SVM model.

## Technology Stack
| Technology | Purpose |
|------------|---------|
| Jupyter Notebook | Interactive environment for data analysis, visualization, and experimentation. |
| Matplotlib | A plotting library for creating static, interactive, and animated visualizations in Python. |
| Seaborn | A Python data visualization library based on matplotlib that provides a high-level interface for drawing attractive statistical graphics. |
| NumPy | A fundamental package for scientific computing with Python, providing support for large, multi-dimensional arrays and matrices, along with a collection of mathematical functions to operate on these arrays. |
| Pandas | An open-source data manipulation and analysis library built on top of NumPy. It provides data structures and operations for manipulating numerical tables and time series. |
| scikit-learn | A simple and efficient tool for data mining and data analysis, built on NumPy, SciPy, and matplotlib. It features various classification, regression, clustering, and dimensionality reduction algorithms.

## Requirements
The project requires Python 3.11.3 and the following packages:
- jupyterlab==3.6.3
- matplotlib==3.7.1
- seaborn==0.12.2
- numpy==1.24.3
- pandas==2.0.1
- scikit-learn==1.2.2

## Installation
To set up the environment, follow these steps:

### macOS
```bash
make setup
source .venv/bin/activate
```

### WindowsOS (PowerShell)
```powershell
pyenv local 3.11.3
python -m venv .venv
.venv\Scripts\Activate.ps1
pip install --upgrade pip
pip install -r requirements.txt
```

### WindowsOS (Git-bash)
```bash
pyenv local 3.11.3
python -m venv .venv
source .venv/Scripts/activate
python -m pip install --upgrade pip
pip install -r requirements.txt
```

## Configuration
No specific configuration is required for this project.

## Quick Start
To get started, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/PartORG/ds-dimensionality-reduction.git
   cd ds-dimensionality-reduction
   ```
2. Set up the environment:
   ```bash
   make setup
   source .venv/bin/activate
   ```
3. Open the Jupyter Notebooks in the following order:
   - 1_Principal_Component_Analysis.ipynb
   - 2_t_SNE.ipynb
   - 3_PCA_in_Pipeline.ipynb

## Usage
To run a specific notebook, activate the environment and use the following command:
```bash
jupyter lab 1_Principal_Component_Analysis.ipynb
```

## Project Structure
```
ds-dimensionality-reduction/
├── .github/workflows/
│   ├── REGX_test_import_libraries.sh
│   ├── discord-webhook-notify.yml
│   ├── replacement.yml
│   └── workflow-02.yml
├── .gitignore
├── 1_Principal_Component_Analysis.ipynb
├── 2_t_SNE.ipynb
├── 3_PCA_in_Pipeline.ipynb
├── Makefile
├── README.md
└── data/
    └── wine_data.csv
```

## Development
The project uses a Makefile for environment setup. The development workflow involves running the notebooks and making changes as needed.

## Limitations
- This project is designed for educational purposes and may not be suitable for production environments.
- The sample dataset used in the notebooks is limited and may not represent real-world data.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.