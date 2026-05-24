# Insurance Risk Analytics

## Project Overview

This project focuses on analyzing insurance-related data to identify risk patterns, perform statistical hypothesis testing, and build predictive machine learning models.

The workflow includes:

- Exploratory Data Analysis (EDA)
- Statistical Hypothesis Testing
- Risk Pattern Identification
- Predictive Modeling
- Model Evaluation
- Data Version Control using DVC

---

# Project Structure

```bash
insurance-risk-analytics/

├── .github/
│   └── workflows/
│       └── ci.yml

├── data/                     # tracked by DVC
├── notebooks/
│   ├── 01_eda.ipynb
│   ├── 02_hypothesis_testing.ipynb
│   └── 03_modeling.ipynb

├── src/
│   ├── __init__.py
│   ├── data_loader.py
│   ├── eda_utils.py
│   ├── hypothesis_tests.py
│   └── modeling.py

├── reports/
│   └── final_report.md

├── tests/

├── requirements.txt
├── dvc.yaml
└── README.md
```

---

# Setup Instructions

## 1. Clone the Repository

```bash
git clone https://github.com/Redeat-Birhane/insurance-risk-analytics.git
cd insurance-risk-analytics
```

---

## 2. Create Virtual Environment

### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

### Mac/Linux

```bash
python3 -m venv venv
source venv/bin/activate
```

---

## 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 4. Initialize DVC

```bash
dvc init
```

## Reproducing Data Pipeline (DVC)

This project uses DVC (Data Version Control) to ensure reproducibility of the dataset pipeline. All datasets are versioned and can be restored at any time.

---

### 1. Install Dependencies

```bash
pip install -r requirements.txt

2. Initialize DVC and Restore Data

If cloning the repository for the first time:
dvc init
dvc pull
---

3. Run the Data Pipeline

To reproduce the data processing pipeline from raw data to cleaned data:
dvc repro

# Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- SciPy
- DVC
- Jupyter Notebook

---

# Workflow

1. Load and preprocess data
2. Perform exploratory data analysis
3. Conduct hypothesis testing
4. Train machine learning models
5. Evaluate model performance
6. Generate reports and insights

---
