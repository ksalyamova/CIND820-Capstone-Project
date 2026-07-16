# Predictive Socioeconomic Modelling and Temporal Validation of Neighbourhood-Level Low-Income Prevalence in Toronto

## CIND820 Capstone Project
### Toronto Metropolitan University (TMU) – The Chang School of Continuing Education

**Author:** Kamola Salyamova

---

# Project Overview

Neighbourhood-level socioeconomic vulnerability is influenced by a complex combination of demographic, educational, employment, housing, and income-related factors. Understanding these relationships is essential for evidence-based municipal planning, resource allocation, and community development.

This capstone project investigates the socioeconomic factors associated with neighbourhood-level low-income prevalence across Toronto using the City of Toronto Neighbourhood Profiles (2011 and 2016) datasets and a combination of statistical analysis and machine learning techniques.

The project follows a complete analytical workflow beginning with data preparation and exploratory data analysis, followed by feature relationship analysis, dimensionality reduction, neighbourhood vulnerability assessment, predictive modelling, historical dataset preparation, temporal comparative analysis, and temporal model validation.

In addition to identifying the socioeconomic indicators associated with neighbourhood vulnerability, the project evaluates whether historical socioeconomic data can be used to accurately predict future neighbourhood-level low-income prevalence by training predictive models using the 2011 dataset and evaluating their performance on the independent 2016 dataset.

The analyses were completed as part of the Toronto Metropolitan University (TMU) Chang School **CIND820 Capstone Project**.

---

# Business Problem

Municipal planners, housing policy analysts, community development agencies, and non-profit organizations require reliable evidence-based methods to identify neighbourhoods experiencing elevated socioeconomic vulnerability.

Although neighbourhood profiles provide extensive socioeconomic information, they are primarily descriptive and do not quantify complex relationships among socioeconomic indicators or evaluate their predictive value.

This project develops a reproducible machine learning framework to support evidence-based decision-making by:

- identifying socioeconomic indicators associated with neighbourhood-level low-income prevalence;
- grouping neighbourhoods into statistically distinct socioeconomic vulnerability profiles;
- developing predictive models capable of estimating neighbourhood-level low-income prevalence; and
- evaluating whether predictive relationships remain reliable over time through temporal model validation.

---

# Project Objectives

The objectives of this project are to:

- prepare machine-learning-ready neighbourhood datasets from the Toronto Neighbourhood Profiles;

- identify and quantify the socioeconomic indicators most strongly associated with neighbourhood-level low-income prevalence;

- classify Toronto neighbourhoods into statistically distinct socioeconomic vulnerability profiles;

- develop predictive models capable of estimating neighbourhood-level low-income prevalence;

- compare predictive model performance using multiple evaluation metrics;

- evaluate whether historical socioeconomic indicators remain reliable predictors of future neighbourhood-level low-income prevalence; and

- provide evidence-based insights to support municipal planning, housing policy, and community investment decisions.

---

# Analyst Role

This project simulates the role of a **Municipal Socioeconomic Data Analyst** responsible for supporting evidence-based planning and policy development.

The intended stakeholders include:

- Toronto City Planners
- Housing Policy Analysts
- Community Development Agencies
- Non-Profit Organizations
- Municipal Decision Makers

The project supports decisions related to:

- affordable housing prioritization;
- neighbourhood investment planning;
- employment support allocation;
- identification of vulnerable neighbourhoods;
- long-term socioeconomic monitoring; and
- strategic resource allocation.

---

# Datasets

## Primary Data Source

**City of Toronto Open Data Portal**

## Datasets Used

- Toronto Neighbourhood Profiles (2016)
- Toronto Neighbourhood Profiles (2011)

### 2016 Dataset

The 2016 dataset serves as the primary analytical dataset and was used for:

- Exploratory Data Analysis (EDA)
- Feature Selection
- Statistical Analysis
- Dimensionality Reduction
- Clustering
- Predictive Modelling
- Geographic Neighbourhood Vulnerability Assessment

### 2011 Dataset

The 2011 dataset was prepared as a historical machine-learning-ready dataset and was used to evaluate the temporal generalizability of the predictive model.

Specifically, the 2011 dataset was used to:

- prepare a historical ML-ready dataset;
- identify variables common to both datasets;
- train the Linear Regression model; and
- evaluate predictive performance using the independent 2016 dataset.

---

# Dependent Variable

The dependent variable used throughout the project is:

**Low_Income_AfterTax_Pct (LIM-AT)**

Low_Income_AfterTax_Pct represents the percentage of individuals living below the Low-Income Measure After Tax (LIM-AT) and serves as the primary indicator of neighbourhood socioeconomic vulnerability throughout the project.

---

# Research Questions

## Research Question 1

**Which socioeconomic indicators are most strongly associated (quantified) with neighbourhood-level low-income prevalence in Toronto?**

This research question investigates the strength of the relationships between selected socioeconomic indicators and neighbourhood-level low-income prevalence.

**Addressed in:**

- Notebook 1 – EDA and Feature Selection
- Notebook 2 – Feature Relationship Analysis

---

## Research Question 2

**Can Toronto neighbourhoods be grouped into statistically distinct socioeconomic vulnerability profiles based on selected socioeconomic indicators?**

This research question investigates whether neighbourhoods exhibit distinct socioeconomic vulnerability patterns and whether meaningful groups can be identified.

**Addressed in:**

- Notebook 3 – PCA and Neighborhood Vulnerability Assessment

---

## Research Question 3

**Can neighbourhood-level low-income prevalence be accurately predicted using selected socioeconomic indicators?**

### (a) Predictive Model Development

**Which predictive model provides the most accurate estimates of neighbourhood-level low-income prevalence using the 2016 Toronto Neighbourhood Profiles dataset?**

**Addressed in:**

- Notebook 4 – Predictive Modelling of Neighborhood Vulnerability

---

### (b) Temporal Model Validation

**To what extent can a model trained using the 2011 Toronto Neighbourhood Profiles dataset accurately predict neighbourhood-level low-income prevalence in the independent 2016 dataset?**

This component evaluates whether historical socioeconomic indicators remain reliable predictors of future neighbourhood-level low-income prevalence.

**Addressed in:**

- Notebook 5 – 2011 Machine Learning Dataset Preparation for Temporal Comparative Analysis
- Notebook 6 – Temporal Validation and Comparative Analysis
- Notebook 7 – Temporal Model Validation

# Relationship Between Research Questions and Notebooks

| Research Question | Supporting Notebooks |
|-------------------|----------------------|
| **RQ1** – Which socioeconomic indicators are most strongly associated (quantified) with neighbourhood-level low-income prevalence in Toronto? | Notebook 1, Notebook 2 |
| **RQ2** – Can Toronto neighbourhoods be grouped into statistically distinct socioeconomic vulnerability profiles? | Notebook 3 |
| **RQ3(a)** – Which predictive model provides the most accurate estimates of neighbourhood-level low-income prevalence? | Notebook 4 |
| **RQ3(b)** – To what extent can a model trained on the 2011 dataset accurately predict neighbourhood-level low-income prevalence in the independent 2016 dataset? | Notebook 5, Notebook 6, Notebook 7 |


---
## Repository Structure 

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
│   ├── 05_2011_Machine_Learning_dataset_Preparation_for_Temporal_Comparative_Analysis.ipynb
│   ├── 06_Temporal_Validation_and_Comparative_Analysis.ipynb
│   └── 07_Temporal_Model_Validation.ipynb
│
├── reports/
├── images/
├── requirements.txt
└── README.md
```
# Key Findings

The project demonstrates that neighbourhood-level socioeconomic vulnerability can be effectively investigated using a combination of statistical analysis and machine learning techniques.

The major findings include:

- Housing affordability, employment, educational attainment, income, and demographic characteristics were identified as the socioeconomic indicators most strongly associated with neighbourhood-level low-income prevalence.

- Principal Component Analysis (PCA) successfully reduced redundancy among correlated socioeconomic indicators while preserving the majority of the original information.

- K-Means clustering identified statistically distinct neighbourhood socioeconomic vulnerability profiles, demonstrating that Toronto neighbourhoods exhibit meaningful socioeconomic groupings.

- Predictive modelling demonstrated that neighbourhood-level low-income prevalence can be accurately estimated using selected socioeconomic indicators. Among the evaluated models, Random Forest Regression achieved the strongest predictive performance on the 2016 dataset.

- Temporal model validation demonstrated that a Linear Regression model trained on the historical 2011 dataset successfully generalized to the independent 2016 dataset, achieving:

  - **R² = 0.666**
  - **MAE = 3.377**
  - **RMSE = 4.543**
  - **MAPE = 19.36%**
  - **WAPE = 17.30%**

  These results indicate that historical socioeconomic indicators remain valuable predictors of future neighbourhood-level low-income prevalence.

---

# Overall Conclusions

The project successfully addressed all three research questions through a structured analytical workflow.

The findings demonstrate that socioeconomic indicators can be used to quantify neighbourhood vulnerability, classify neighbourhoods into statistically distinct socioeconomic profiles, develop accurate predictive models, and evaluate whether these predictive relationships remain stable over time.

The temporal validation further demonstrated that a model trained using historical socioeconomic data maintained good predictive performance when applied to future neighbourhood data, supporting the use of predictive analytics as a tool for long-term socioeconomic planning.

Overall, the developed framework provides a reproducible approach for identifying neighbourhoods at greater socioeconomic risk and supports evidence-based planning for municipal governments, housing policy analysts, and community organizations.

---

# Limitations

The original project design proposed using the **2016** and **2021 Toronto Neighbourhood Profiles** to evaluate temporal changes in neighbourhood socioeconomic vulnerability.

During data preparation, however, the 2021 dataset was found to be insufficiently comparable with the 2016 dataset due to differences in variable availability, indicator definitions, and overall dataset structure. These inconsistencies limited the ability to construct directly comparable machine-learning-ready datasets using a common set of socioeconomic indicators.

To ensure methodological consistency and reliable temporal comparison, the study instead used the **2011** and **2016** Toronto Neighbourhood Profiles, which shared a more consistent structure and a common set of socioeconomic variables. This enabled the development of comparable machine-learning-ready datasets and supported a valid temporal model validation.

Additionally, this project focuses exclusively on neighbourhood-level socioeconomic indicators available through the Toronto Neighbourhood Profiles. Other potentially important determinants of neighbourhood vulnerability, such as health outcomes, crime statistics, transportation accessibility, or longitudinal economic shocks, were beyond the scope of this study.

---

# Future Work

Future research could extend this project by:

- incorporating future releases of the Toronto Neighbourhood Profiles as additional comparable datasets become available;

- integrating complementary datasets such as housing market trends, public health indicators, transportation accessibility, or crime statistics;

- investigating additional machine learning algorithms such as Gradient Boosting, XGBoost, or Neural Networks;

- developing interactive dashboards to support municipal decision-makers; and

- extending the framework to evaluate neighbourhood socioeconomic vulnerability in other Canadian municipalities.

---

# Software and Libraries

The project was developed using:

- Python
- Jupyter Notebook
- Visual Studio Code

Primary Python libraries include:

- Pandas
- NumPy
- Matplotlib
- SciPy
- Scikit-learn
- Statsmodels
- Yellowbrick
- OpenPyXL

---

# Installation

Clone the repository:

```bash
git clone https://github.com/<your-github-username>/CIND820-Capstone-Project.git
```

Install the required packages:

```bash
pip install -r requirements.txt
```

Open the notebooks using Jupyter Notebook or Visual Studio Code.

---

# Project Workflow Standard

Each notebook follows a consistent analytical structure:

**Objective → Code → Interpretation**

This standardized workflow promotes transparency, reproducibility, and consistency throughout the project.

---

# AI Productivity Declaration

Generative AI (ChatGPT) was used to assist with:

- code refinement;
- brainstorming the ideas;
- debugging;
- documentation;
- markdown preparation;
- project organization; and
- technical explanations.

All analytical decisions, data preparation, statistical analyses, model development, interpretation of results, and final project content were independently reviewed, validated, and approved by the project author.

---

# Acknowledgements

This project acknowledges the following organizations and resources:

- City of Toronto Open Data Portal
- Toronto Metropolitan University
- The Chang School of Continuing Education
- CIND820 Capstone Project
- Dr. Tamer Abdou for continuous support
---

# Author

**Kamola Salyamova**

Toronto Metropolitan University

The Chang School of Continuing Education

CIND820 – Capstone Project

2026