# Dimensionality Reduction

In this repo we will have a look at dimensionality reduction techniques using Jupyter Notebooks and popular Python libraries such as NumPy, Pandas, Matplotlib, Seaborn, and Scikit-learn. This project is designed to help data scientists and machine learning practitioners understand and implement various dimensionality reduction algorithms.

## Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [How It Works](#how-it-works)
4. [Technology Stack](#technology-stack)
5. [Requirements](#requirements)
6. [Installation](#installation)
7. [Configuration](#configuration)
8. [Quick Start](#quick-start)
9. [Usage](#usage)
10. [Project Structure](#project-structure)
11. [Development](#development)
12. [Limitations](#limitations)
13. [License](#license)

## Introduction

Dimensionality reduction is a crucial step in data preprocessing, helping to simplify complex datasets while retaining essential information. This project provides hands-on experience with three popular dimensionality reduction techniques: Principal Component Analysis (PCA), t-Distributed Stochastic Neighbor Embedding (t-SNE), and PCA within a pipeline for Support Vector Machines (SVM).

## Features

### 1. Principal Component Analysis (PCA)
- **What it does:** Reduces the number of random variables under consideration, by obtaining a set of principal variables.
- **Why it exists:** PCA is widely used in data visualization and feature extraction.
- **Why it is useful:** It helps in reducing dimensionality while retaining most of the variance.

### 2. t-Distributed Stochastic Neighbor Embedding (t-SNE)
- **What it does:** A non-linear dimensionality reduction technique that is particularly well suited for high-dimensional data.
- **Why it exists:** t-SNE is used for visualizing high-dimensional data by giving each data point a location in a two or three-dimensional space, where similar points are close to each other and dissimilar points are farther apart.
- **Why it is useful:** It is excellent for exploring the structure of complex datasets.

### 3. PCA in Pipeline with SVM
- **What it does:** Combines PCA with an SVM classifier to improve performance on high-dimensional data.
- **Why it exists:** This approach helps in reducing overfitting and improving generalization.
- **Why it is useful:** It provides a practical solution for applying dimensionality reduction in real-world machine learning tasks.

## How It Works

The project consists of three Jupyter Notebooks:

1. **Principal Component Analysis (PCA):** Introduces the concept of PCA using a sample dataset and demonstrates how to perform PCA.
2. **t-SNE:** Explains t-SNE and provides an example implementation.
3. **PCA in Pipeline with SVM:** Combines PCA with an SVM classifier for better performance.

## Technology Stack

| Technology | Purpose |
|------------|---------|
| Jupyter Notebook | Interactive environment for data analysis and visualization. |
| NumPy | Fundamental package for scientific computing with Python. |
| Pandas | Data structures and operations for manipulating numerical tables and time series. |
| Matplotlib & Seaborn | Libraries for creating static, animated, and interactive visualizations in Python. |
| Scikit-learn | Simple and efficient tools for data mining and data analysis. |

## Requirements

- Python 3.11.3
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Installation

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

No specific configuration is required.

## Quick Start

1. Clone the repository:
   ```bash
   git clone https://github.com/PartORG/ds-dimensionality-reduction.git
   cd ds-dimensionality-reduction
   ```
2. Set up your environment (see [Installation](#installation)).
3. Open Jupyter Notebook and run the notebooks in the following order:
   - 1_Principal_Component_Analysis.ipynb
   - 2_t_SNE.ipynb
   - 3_PCA_in_Pipeline.ipynb

## Usage

Run the Jupyter Notebooks to explore dimensionality reduction techniques.

```bash
jupyter notebook
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

The project uses a Makefile for setting up the development environment. Contributions are welcome, but please ensure that all changes are tested and documented.

## Limitations

- This project is designed for educational purposes and may not be suitable for production environments.
- The sample dataset used in the notebooks is limited and should be replaced with larger datasets for real-world applications.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.