# Dimensionality Reduction

In this repository, we explore various techniques for dimensionality reduction using Jupyter Notebooks.

## Requirements

To run this project, you will need:

- Python 3.11.3 (managed by pyenv)
- jupyterlab==3.6.3
- matplotlib==3.7.1
- seaborn==0.12.2
- numpy==1.24.3
- pandas==2.0.1
- scikit-learn==1.2.2

## Installation

### macOS

To set up your environment on macOS, run:

```bash
make setup
```

After running the `setup` command, activate the virtual environment with:

```bash
source .venv/bin/activate
```

### WindowsOS

For WindowsOS, you can set up your environment using PowerShell or Git-bash. Follow these steps for both:

**PowerShell:**

```powershell
pyenv local 3.11.3
python -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
```

**Git-bash:**

```bash
pyenv local 3.11.3
python -m venv .venv
source .venv/Scripts/activate
python -m pip install --upgrade pip
pip install -r requirements.txt
```

If you encounter an error when running `pip install --upgrade pip`, try using:

```bash
python.exe -m pip install --upgrade pip
```

## Usage

To run the project, follow these steps:

1. Activate your virtual environment (if not already activated).
2. Open any of the Jupyter Notebooks in this repository.

For example, to open `1_Principal_Component_Analysis.ipynb`, you can use:

```bash
jupyter lab 1_Principal_Component_Analysis.ipynb
```

This will launch JupyterLab and open the specified notebook for you to explore.