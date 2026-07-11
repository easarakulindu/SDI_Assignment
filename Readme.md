# University Student Device Purchasing Analysis 💻

## Project Overview

This repository contains the data analysis pipeline for our research project investigating the primary factors that influence device purchasing decisions among university students.

Our core research question focuses on how factors like performance, brand name, and academic faculty impact the final financial commitment (`device_price`).

## Repository Structure

- `datasets/` - Contains the raw and processed Excel/CSV files.
- `01_data_cleaning.ipynb` - The pipeline for raw data ingestion, regex extraction, and imputation.
- `02_descriptive_analysis.ipynb` - Exploratory Data Analysis (EDA) containing univariate and bivariate visualizations.
- `03_inferential_modeling.ipynb` - [WIP] Multiple Linear Regression models to establish statistical significance.
- `requirements.txt` - Project dependencies.

---

## 🛠️ Local Setup Guide

We are using `uv` for fast Python environment management. Follow these steps to run the notebooks locally without breaking your system Python.

### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd <repository-folder-name>
```

## 2. Create and Activate the Virtual Environment

Generate the .venv folder:

```bash
python3 -m venv .venv
```

Activate the environment based on your operating system/shell:

Linux/macOS `(fish): source .venv/bin/activate.fish`

Linux/macOS ` (bash/zsh): source .venv/bin/activate`

Windows `(Command Prompt): .venv\Scripts\activate.bat`

Windows `(PowerShell): .venv\Scripts\Activate.ps1`

## 3. Install Dependencies

With the environment activated, install the required packages using pip:

```bash
pip install -r requirements.txt
```

## 4. Run the Notebooks in VS Code

Open the repository in VS Code.

Open any .ipynb file.

In the top right corner, click Select Kernel -> Python Environments and choose the one marked ('.venv': venv).

# ⚠️ Collaboration Rules (PLEASE READ BEFORE PULLING) ⚠️

Jupyter Notebooks (.ipynb files) are massive JSON files under the hood. If multiple people edit the same notebook locally and try to push to the main branch, it will cause catastrophic merge conflicts that are nearly impossible to resolve manually.

How to Propose Changes / Write the Report:
Option A (Git Branches): If you want to write code or markdown locally, create a new branch (git checkout -b your-name-edits) and push that branch. Do not push directly to main.

Option B (Google Colab): We will do our live collaborative editing (writing the final report and tweaking models) over a shared Google Colab session to completely avoid Git merge conflicts.
