# Alzheimer's Disease Detection

This repository contains Jupyter notebooks exploring machine-learning approaches to classify the `Diagnosis` field in the included Alzheimer's disease dataset. The notebooks cover logistic regression, support vector machines, feature selection, hyperparameter tuning, and voting ensembles.

> **Important:** This is an educational project, not a medical device. Its models and results are not intended for diagnosis, treatment decisions, or other clinical use.

## Project contents

| File | Description |
| --- | --- |
| `alzheimers_disease_data.csv` | Dataset used by the notebooks (2,149 records, 35 columns). |
| `Logistic_regression.ipynb` | Logistic regression workflow and classification evaluation. |
| `SVM.ipynb` | Support vector machine workflow, including a SelectKBest feature-selection experiment. |
| `Hypertuning with KBest and RFE.ipynb` | Feature selection with SelectKBest and RFE, model tuning, and voting classifiers. |
| `Hyperparameter tuning and hard voting ,soft voting .ipynb` | Hyperparameter tuning and hard- and soft-voting ensemble experiments. |

## Dataset

The target column is `Diagnosis` (values `0` and `1`). The dataset also includes demographic, lifestyle, medical-history, cognitive-assessment, and symptom fields, along with `PatientID` and `DoctorInCharge`.

Before using the data for modeling, review each notebook's preprocessing and feature-selection steps. In particular, consider whether identifiers or fields that could reveal the target should be excluded from model inputs.

## Getting started

1. Clone or download this repository.
2. Install Python 3 and Jupyter Notebook or JupyterLab.
3. Install the libraries used by the notebooks:

   ```bash
   python -m pip install jupyter pandas numpy matplotlib seaborn scikit-learn
   ```

4. Start Jupyter from the repository directory:

   ```bash
   jupyter notebook
   ```

5. Open a notebook and run its cells. Keep `alzheimers_disease_data.csv` in the repository directory; the notebooks load it by filename.

The notebooks may use different preprocessing, train/test splits, and evaluation steps. Compare results only after checking those choices and how each notebook handles the target and input features.
