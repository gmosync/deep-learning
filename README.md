# Deep Learning Experiments

This repository contains code, notebooks, and experiments from my Master's in Artificial Intelligence deep learning coursework. It includes a clean Python project structure, reproducible virtual environment setup, and modular source code for experimentation and testing.


## Project Structure

```bash
deep-learning/
├── .venv/ # local virtual environment (ignored by Git)
├── notebooks/ # Jupyter notebooks for experiments
├── src/ # Python modules and reusable code
├── data/ # local data files (ignored)
├── artifacts/ # model outputs, plots, logs
├── tests/ # optional test files
├── requirements.in # editable list of top-level dependencies
├── requirements.txt # fully pinned lock file (auto-generated)
└── .gitignore # files excluded from Git versioning
```

## Reproducing the environment

> **Recommended:** use a project-local virtual environment so this repo’s
> dependencies stay isolated from any other Python projects on your machine.

### Using `venv` + `pip`

```bash
# 1  Clone the repo
git clone git@github.com:gmosync/deep-learning.git
cd deep-learning

# 2  Create & activate a virtual environment (Python ≥ 3.10)
python3 -m venv .venv
# macOS / Linux
source .venv/bin/activate
# Windows (PowerShell)
# .venv\Scripts\Activate.ps1

# 3  Install the exact pinned dependencies
pip install -r requirements.txt

# 4  Launch Jupyter (if you want notebooks)
jupyter notebook
