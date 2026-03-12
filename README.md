# 🧠 Diabetes Risk Prediction using Machine Learning (BRFSS 2015)

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.18976614.svg)](https://doi.org/10.5281/zenodo.18976614)
[![ORCID](https://img.shields.io/badge/ORCID-0009--0005--7126--223X-green)](https://orcid.org/0009-0005-7126-223X)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

---

## 📌 Overview

This repository contains the complete code and research resources for the study:

**"Statistical Analysis and Machine Learning Prediction of Diabetes Risk Using BRFSS Data"**

The aim of this project is to develop a **machine learning based predictive system** that can estimate diabetes risk using demographic, behavioral, and clinical health factors from the **BRFSS 2015 dataset** published by the CDC.

This research combines three major components:

- Statistical hypothesis testing  
- Supervised machine learning models  
- Explainable Artificial Intelligence (XAI)

This framework allows the system not only to **predict diabetes risk** but also to **explain the key health factors influencing predictions**.

---

## 🎯 Key Highlights

| Metric | Value |
|------|------|
| Dataset | BRFSS 2015 |
| Records | 253,680 individuals |
| Features | 21 variables |
| Best Model | XGBoost |
| Accuracy | 82.16% |
| ROC-AUC | 0.8234 |
| Explainability | SHAP |
| Class Imbalance Handling | SMOTE + Random Undersampling |

---

## 📂 Repository Structure

```
Diabetes_Prediction_BRFSS
│
├── README.md
├── requirements.txt
├── diabetes_prediction.ipynb
│
├── scripts
│   ├── analysis.py
│   ├── models.py
│   └── shap_analysis.py
│
├── data
│   └── brfss_2015_diabetes.csv
│
├── results
│   ├── roc_curves.png
│   ├── confusion_matrix.png
│   └── shap_summary_plot.png
│
└── paper
    └── diabetes_prediction_paper.pdf
```

---

## 🚀 Installation

### 1️⃣ Clone the repository

```bash
git clone https://github.com/waqi786/Diabetes_Prediction_BRFSS.git
cd Diabetes_Prediction_BRFSS
```

### 2️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

---

## 📊 Dataset

The dataset used in this research comes from the **Behavioral Risk Factor Surveillance System (BRFSS)** conducted by the **Centers for Disease Control and Prevention (CDC)**.

Dataset characteristics:

- 253,680 individuals  
- 21 health related variables  
- Demographic information  
- Lifestyle behavior indicators  
- Clinical health conditions  

Download the dataset from:

https://www.cdc.gov/brfss/annual_data/annual_2015.html

After downloading, place the dataset file inside the **data/** folder.

---

## 🧪 Methodology

### 1️⃣ Statistical Analysis

Statistical hypothesis testing was used to identify significant differences between diabetic and non-diabetic populations.

Methods used:

- Shapiro-Wilk test for normality  
- Mann-Whitney U test  
- Independent t-test  
- Chi-square test for categorical variables  

Significance level:

```
p < 0.001
```

---

### 2️⃣ Data Preprocessing

Several preprocessing steps were applied before model training:

- Missing value handling  
- Feature encoding  
- Feature normalization  
- Train-test split (80/20)  
- Class imbalance handling using **SMOTE + Random Undersampling**

---

### 3️⃣ Machine Learning Models

The following supervised learning models were trained:

- Logistic Regression  
- Random Forest  
- XGBoost  

Hyperparameter tuning was performed using **Grid Search with cross-validation**.

---

### 4️⃣ Model Evaluation Metrics

The models were evaluated using the following metrics:

- Accuracy  
- Precision  
- Recall  
- F1-Score  
- ROC-AUC  
- Specificity  
- Matthews Correlation Coefficient (MCC)

---

### 5️⃣ Explainable Artificial Intelligence

Model interpretability was achieved using **SHAP (SHapley Additive exPlanations)**.

SHAP analysis was used to:

- Identify global feature importance  
- Explain individual predictions  
- Detect major diabetes risk factors

---

## 📊 Results

### Model Performance Comparison

| Model | Accuracy | ROC-AUC | Precision | Recall | F1 Score |
|------|------|------|------|------|------|
| XGBoost | **82.16%** | **0.8234** | 0.4443 | 0.5266 | 0.4820 |
| Random Forest | 80.60% | 0.8191 | 0.4281 | 0.5028 | 0.4624 |
| Logistic Regression | 72.98% | 0.8160 | 0.3489 | 0.5047 | 0.4127 |

---

## 📈 Important Risk Factors

According to SHAP analysis, the most influential predictors of diabetes were:

1. High Blood Pressure  
2. Self-reported General Health  
3. High Cholesterol  
4. Body Mass Index (BMI)  
5. Age Category  

---

## 📝 Citation

If you use this work in your research, please cite:

```bibtex
@article{ali2026diabetes,
  title={Statistical Analysis and Machine Learning Prediction of Diabetes Risk Using BRFSS Data},
  author={Ali, Waqar},
  journal={Zenodo},
  year={2026},
  doi={10.5281/zenodo.18976614}
}
```

---

## 📜 License

This project is licensed under the **Creative Commons Attribution 4.0 International License (CC BY 4.0)**.

You are free to:

- Share — copy and redistribute the material  
- Adapt — remix, transform, and build upon the material  

Under the following condition:

- Attribution must be given to the original author.

License link:

https://creativecommons.org/licenses/by/4.0/

---

## 📬 Contact

**Waqar Ali**  
Data Science Researcher  

Email: dsali20838@gmail.com  
GitHub: https://github.com/waqi786  

---

⭐ If you find this repository useful, please consider giving it a star.
