# Predictive Socioeconomic Modeling: Forecasting Neighborhood-Level Low-Income Prevalence Across Toronto Using Statistical Analysis and Machine Learning

https://github.com/ksalyamova/CIND820-Capstone-Project

## Overview

This capstone project develops a predictive analytics framework to investigate neighbourhood-level socioeconomic vulnerability across Toronto using statistical analysis and machine learning techniques.

Using publicly available data from the City of Toronto Open Data Portal, the project examines the relationships between demographic, labour market, educational, housing, and income indicators to identify the factors associated with neighbourhood-level low-income prevalence.

The project follows a complete data science workflow including:

- Data Preparation
- Exploratory Data Analysis (EDA)
- Correlation Analysis
- Multicollinearity Assessment (VIF)
- Feature Selection
- Principal Component Analysis (PCA)
- K-Means Clustering
- One-Way ANOVA
- Multiple Linear Regression
- Random Forest Regression
- Cross Validation
- Temporal Model Validation

The final outcome is a reproducible machine learning framework capable of supporting evidence-based municipal planning and socioeconomic decision-making.

---

# Business Problem

Municipal planners, housing policy analysts, and community organizations require reliable analytical methods to identify neighbourhoods experiencing elevated socioeconomic vulnerability.

Although Toronto's Neighbourhood Profiles contain extensive socioeconomic information, the datasets are descriptive and do not directly support predictive decision-making.

This project transforms publicly available socioeconomic data into predictive models capable of:

- identifying neighbourhoods at greater socioeconomic risk;
- quantifying the factors associated with low-income prevalence;
- classifying neighbourhoods into meaningful vulnerability profiles; and
- evaluating whether historical socioeconomic indicators remain reliable predictors of future neighbourhood conditions.

---

# Project Objectives

The objectives of this project are to:

- Prepare machine-learning-ready datasets
- Identify socioeconomic indicators associated with neighbourhood low-income prevalence
- Reduce dimensionality using Principal Component Analysis (PCA)
- Identify neighbourhood vulnerability profiles using K-Means clustering
- Develop predictive regression models
- Compare model performance using multiple evaluation metrics
- Evaluate temporal model generalizability using historical data
- Support evidence-based municipal planning

---

# Research Questions

### Research Question 1

Which socioeconomic indicators are most strongly associated with neighbourhood-level low-income prevalence across Toronto?

---

### Research Question 2

Can Toronto neighbourhoods be grouped into statistically distinct socioeconomic vulnerability profiles?

---

### Research Question 3

Which predictive modelling approach provides the most accurate, efficient, and stable estimation of neighbourhood-level low-income prevalence?

---

# Stakeholders

This project was developed from the perspective of a Municipal Socioeconomic Data Analyst.

Primary stakeholders include:

- Toronto City Planners
- Housing Policy Analysts
- Community Development Agencies
- Non-Profit Organizations
- Municipal Decision Makers

The results support:

- Affordable housing prioritization
- Resource allocation
- Community investment planning
- Employment support initiatives
- Long-term socioeconomic monitoring

---

# Dataset

**Source**

City of Toronto Open Data Portal

Datasets Used

- Toronto Neighbourhood Profiles (2016)
- Toronto Neighbourhood Profiles (2011)

The 2016 dataset was used for:

- EDA
- Statistical Analysis
- PCA
- Clustering
- Predictive Modelling

The 2011 dataset was prepared for temporal validation to evaluate whether historical socioeconomic indicators successfully predict neighbourhood conditions in 2016.

---

# Target Variable

**Dependent Variable**

Low_Income_AfterTax_Pct (LIM-AT)

The percentage of individuals living below the Low Income Measure After Tax (LIM-AT), representing neighbourhood socioeconomic vulnerability.

---

# Analytical Workflow

## Notebook 1

### Exploratory Data Analysis and Feature Selection

Topics

- Data Cleaning
- Missing Value Assessment
- Descriptive Statistics
- Distribution Analysis
- Feature Selection

---

## Notebook 2

### Feature Relationship Analysis

Topics

- Pearson Correlation
- Spearman Correlation
- VIF
- Feature Selection Comparison

---

## Notebook 3

### PCA and Neighborhood Vulnerability Assessment

Topics

- Standardization
- Principal Component Analysis
- Explained Variance
- Elbow Method
- K-Means Clustering
- Cluster Profiling
- One-Way ANOVA

---

## Notebook 4

### Predictive Modelling

Models

- Multiple Linear Regression
- Random Forest Regression

Evaluation Metrics

- R²
- Adjusted R²
- MAE
- RMSE
- MAPE
- WAPE
- Training Time
- Prediction Time
- Five-Fold Cross Validation

---

## Notebook 5

### Historical Dataset Preparation

Preparation of a machine-learning-ready 2011 dataset for temporal validation.

---

## Notebook 6

### Temporal Comparative Analysis

Comparison of common socioeconomic indicators between the 2011 and 2016 datasets.

---

## Notebook 7

### Temporal Model Validation

A Linear Regression model trained on the 2011 dataset was evaluated using the independent 2016 dataset to assess model generalizability over time.

---

# Machine Learning Methods

## Statistical Analysis

- Descriptive Statistics
- Pearson Correlation
- Spearman Correlation
- Variance Inflation Factor (VIF)
- One-Way ANOVA

## Unsupervised Learning

- Principal Component Analysis (PCA)
- K-Means Clustering

## Supervised Learning

- Multiple Linear Regression
- Random Forest Regression

## Model Validation

- Train/Test Split
- Five-Fold Cross Validation
- Temporal Model Validation

---

# Key Findings

The project demonstrates that neighbourhood socioeconomic vulnerability can be effectively investigated using statistical analysis and machine learning.

Major findings include:

- Employment, education, housing affordability, and demographic characteristics were strongly associated with neighbourhood low-income prevalence.

- Principal Component Analysis successfully reduced multicollinearity while preserving the majority of socioeconomic information.

- K-Means clustering identified four statistically distinct neighbourhood vulnerability profiles.

- Multiple Linear Regression provided an effective balance of predictive accuracy, interpretability, computational efficiency, and model stability.

- Temporal validation demonstrated that historical socioeconomic indicators remained useful predictors of future neighbourhood-level low-income prevalence.

---

# Repository Structure

```
CIND820-Capstone-Project/

│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   ├── 01_EDA_and_Feature_Selection.ipynb
│   ├── 02_Feature_Relationship_Analysis.ipynb
│   ├── 03_PCA_and_Neighborhood_Vulnerability_Assessment.ipynb
│   ├── 04_Predictive_Modelling_Neighborhood_Vulnerability.ipynb
│   ├── 05_2011_Machine_Learning_Dataset_Preparation.ipynb
│   ├── 06_Temporal_Validation_and_Comparative_Analysis.ipynb
│   └── 07_Temporal_Model_Validation.ipynb
│
├── reports/
│
├── images/
│
├── requirements.txt
│
└── README.md
```

---

# Software

- Python
- Jupyter Notebook
- Visual Studio Code
- Git
- GitHub

---

# Python Libraries

- pandas
- numpy
- matplotlib
- scipy
- scikit-learn
- statsmodels
- yellowbrick
- openpyxl

---

# Installation

Clone the repository

```bash
git clone https://github.com/yourusername/CIND820-Capstone-Project.git
```

Navigate into the project

```bash
cd CIND820-Capstone-Project
```

Install dependencies

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook

```bash
jupyter notebook
```

---

# Results

The developed framework provides a reproducible approach for:

- identifying neighbourhoods experiencing elevated socioeconomic vulnerability;
- supporting evidence-based housing and community planning;
- evaluating predictive model performance;
- assessing model stability over time; and
- informing long-term municipal planning decisions.

---

# Limitations

The original project proposed using the 2016 and 2021 Toronto Neighbourhood Profiles for temporal analysis.

Due to differences in variable definitions and dataset structure, the 2021 dataset was not directly comparable with the 2016 dataset. Consequently, the study used the 2011 and 2016 datasets to ensure methodological consistency and reliable temporal validation.

---

# Future Work

Future research may extend this framework by:

- incorporating future Toronto Neighbourhood Profile releases;
- integrating additional datasets such as health, crime, transportation, and housing market data;
- evaluating Gradient Boosting, XGBoost, and Neural Networks;
- developing interactive dashboards for decision makers; and
- applying the framework to other Canadian municipalities.

---

# Author

**Kamola Salyamova**

CIND820 Capstone Project

Toronto Metropolitan University

The Chang School of Continuing Education

Supervisor: Dr. Tamer Abdou

July 2026

---

# Acknowledgements

This project was completed as part of the CIND820 Capstone Project at Toronto Metropolitan University using publicly available data from the City of Toronto Open Data Portal.