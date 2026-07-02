# CIND 820 Capstone Project

## Project Overview

This project investigates socioeconomic vulnerability across Toronto neighbourhoods using demographic, housing, education, labour market, and low-income indicators derived from the Toronto Neighbourhood Profiles dataset.

The objective is to identify the socioeconomic characteristics associated with vulnerability, classify neighbourhoods with similar profiles, and support evidence-based planning and resource allocation.

## Current Project Status

- ✅ 2016 Toronto Neighbourhood Profile dataset fully prepared and analyzed.
- ✅ Completed EDA, PCA, clustering, and feature engineering for the 2016 dataset.
- ✅ 2006 dataset assessed and cleaned for feature compatibility.
- ??? Several important socioeconomic indicators (labour and housing) are unavailable at the neighbourhood level in the 2006 dataset, limiting its suitability for predictive modelling.
-  2011 dataset is currently being prepared for feature engineering and predictive modelling.
- Next step: build predictive machine learning models using comparable neighbourhood-level
---

## Research Questions

### Research Question 1

Which socioeconomic indicators are most strongly associated with neighbourhood-level vulnerability and low-income prevalence in Toronto?

### Research Question 2

Can Toronto neighbourhoods be grouped into meaningful vulnerability profiles using dimensionality reduction and clustering techniques?

### Research Question 3

How may neighbourhood vulnerability patterns evolve over time based on future socioeconomic trends?

---

## Completed Analysis

### Notebook 1: Exploratory Data Analysis and Indicator Selection

* Data cleaning and preparation
* Indicator selection
* Missing value assessment
* Descriptive statistics
* Distribution analysis
* Initial correlation analysis
* Creation of machine-learning-ready dataset

### Notebook 2: Feature Relationship Analysis and Dimensionality Assessment

* Correlation matrix analysis
* Employment and unemployment indicator validation
* Multicollinearity assessment using Variance Inflation Factor (VIF)
* Feature relationship exploration
* Dimensionality assessment for PCA preparation

### Notebook 3: Dimensionality Reduction and Vulnerability Classification

* Data standardization
* Principal Component Analysis (PCA)
* Explained variance assessment
* Principal component interpretation
* K-Means clustering
* Vulnerability classification
* Cluster profiling and neighbourhood segmentation

---

## Key Findings

### PCA Results

The first three principal components explain approximately 88.6% of the total variance:

* PC1: Socioeconomic vulnerability dimension
* PC2: Education and labour market participation dimension
* PC3: Housing affordability and low-income dimension

### Clustering Results

Four neighbourhood clusters were identified:

* Cluster 0: Moderate vulnerability neighbourhoods
* Cluster 1: High vulnerability neighbourhoods
* Cluster 2: Lower vulnerability neighbourhoods
* Cluster 3: High-income and highly educated neighbourhoods

---

## Repository Structure

data/

* 01_EDA_and_Indicator_Selection.ipynb
* 02_Feature_Relationship_Analysis_Dimensionality.ipynb
* 03_Dimensionality_reduction_and_Vulnerability_Classification.ipynb
* neighbourhood_profiles_ml_ready.csv
* toronto_neighbourhood_analysis_v2.csv
* toronto_neighbourhood_clusters.csv

reports/

* 01_EDA_and_Indicator_Selection.html
* 02_Feature_Relationship_Analysis_Dimensionality.html
* 03_Dimensionality_reduction_and_Vulnerability_Classification.html

Notebook 1:
EDA, cleaning, indicator selection

Notebook 2:
Correlation analysis, multicollinearity assessment (VIF),
PCA dimensionality reduction

Notebook 3:
K-Means clustering and neighbourhood vulnerability profiling

---

## Current Status

Completed:

* Exploratory Data Analysis
* Indicator Selection
* Feature Relationship Analysis
* PCA
* K-Means Clustering
* Vulnerability Classification

Planned:

Integrate 2006 Toronto Neighbourhood Profiles
Longitudinal analysis
Predictive modelling
Vulnerability forecasting
Interactive visualizations

---
## Analyst Role and Decision Context

This project simulates the work of a municipal socioeconomic data analyst supporting:

* Toronto city planners
* Housing policy analysts
* Community development agencies
* Nonprofit organizations

The results support decisions related to:

* Affordable housing prioritization
* Community investment planning
* Employment support allocation
* Early intervention strategies
* Neighbourhood vulnerability monitoring

---
(Version_1)

# CIND 820 Capstone Project

## Project Summary
## Predictive Socioeconomic Modeling: Forecasting Neighbourhood-Level Low-Income Prevalence in Toronto

### Project Overview

This capstone project investigates socioeconomic vulnerability across Toronto neighbourhoods using open data from the City of Toronto Neighbourhood Profiles dataset. The objective is to identify the socioeconomic factors associated with low-income prevalence, classify neighbourhoods based on vulnerability characteristics, and develop a foundation for future predictive modelling.

The project supports evidence-based decision making for:

* Toronto City Planners
* Housing Policy Analysts
* Real Estate/ Business investors
* Community Development Agencies
* Non-Profit Organizations

---

## Research Questions

### RQ1: Socioeconomic Drivers of Vulnerability

Which socioeconomic variables are most strongly associated with neighbourhood-level low-income prevalence in Toronto?

### RQ2: Neighbourhood Vulnerability Classification

Which Toronto neighbourhoods demonstrate the highest socioeconomic vulnerability based on income, education, employment, housing, and demographic indicators?

### RQ3: Future Vulnerability Trends

How may low-income prevalence and housing burden indicators change across Toronto neighbourhoods over time?

Future project phases will incorporate historical neighbourhood profile datasets (2006 and 2011) to support longitudinal analysis and predictive modelling.

---

## Dataset

### Primary Dataset

**Toronto Neighbourhood Profiles (2016)**

Source:
https://open.toronto.ca/

The dataset contains socioeconomic, demographic, housing, employment, education, and income indicators for Toronto neighbourhoods.

### Key Indicators Used

* Low Income Measure After Tax (LIM-AT)
* Immigrant Population
* Visible Minority Population
* Renters
* No Diploma
* Bachelor's Degree
* Core Housing Need
* Unaffordable Housing
* Labour Force Participation Rate
* Employment Rate
* Unemployment Rate
* Lone Parent Families

---

## Methodology

### Notebook 1 – Exploratory Data Analysis and Indicator Selection

Objectives:

* Data cleaning and preparation
* Variable selection
* Missing value assessment
* Correlation analysis
* Dataset restructuring
* Automated data profiling

Outputs:

* Cleaned modelling dataset
* EDA report
* Indicator selection justification

---

### Notebook 2 – Feature Relationship Analysis and Dimensionality Reduction

Objectives:

* Feature standardization
* Principal Component Analysis (PCA)
* Scree Plot analysis
* Explained variance analysis
* Component interpretation

Results:

* First 3 principal components retained
* Approximately 89% of variance explained
* Reduced dimensionality while preserving socioeconomic information

---

### Notebook 3 – Vulnerability Classification and Clustering

Objectives:

* PCA-based neighbourhood scoring
* K-Means clustering
* Elbow Method optimization
* Cluster interpretation

Results:

* Four neighbourhood vulnerability clusters identified
* Distinct socioeconomic profiles observed across clusters
* Cluster summaries generated for policy interpretation

---

## Repository Structure

```text
CIND820-Capstone-Project/

├── data/
│   ├── 01_EDA_and_Indicator_Selection.ipynb
│   ├── 02_Feature_Relationship_Analysis_Dimensionality.ipynb
│   ├── 03_Dimensionality_reduction_and_Vulnerability_Classification.ipynb
│   ├── neighbourhood_profiles_ml_ready.csv
│   ├── toronto_neighbourhood_analysis_v2.csv
│   └── toronto_neighbourhood_clusters.csv

├── reports/
│   ├── 01_EDA_and_Indicator_Selection.html
│   ├── 02_Feature_Relationship_Analysis_Dimensionality.html
│   └── 03_Dimensionality_reduction_and_Vulnerability_Classification.html

├── visualizations/

├── proposal/

├── docs/
│   ├── Interim_Report_Submitted.pdf
│   └── Interim_Report_Revised_After_Professor_Feedback.pdf

└── README.md
```

---

## Software and Libraries

Python Version:

* Python 3.11

Key Libraries:

* pandas
* numpy
* matplotlib
* seaborn
* scikit-learn
* ydata-profiling

---

## Reproducibility

Recommended execution order:

1. Notebook 1 – Data Cleaning and EDA
2. Notebook 2 – PCA and Feature Analysis
3. Notebook 3 – Vulnerability Classification and Clustering

Generated reports are available in the reports/ directory.

---

## Data Privacy and Ethics

This project uses publicly available aggregate neighbourhood-level data.

* No personally identifiable information (PII) is included.
* Results are reported at the neighbourhood level.
* Analysis follows ethical principles outlined in the Tri-Council Policy Statement (TCPS 2).

---

## Future Work

Future phases will expand the analysis through:

* Integration of 2006 and 2011 Toronto Neighbourhood Profile datasets.
* Longitudinal analysis of socioeconomic vulnerability.
* Predictive modelling of low-income prevalence.
* Integration of housing affordability and labour market datasets.
* Development of vulnerability forecasting models.

---

## GenAI Declaration

Generative AI tools were used to assist with code troubleshooting, documentation drafting, report organization, and explanation of statistical methods. All analytical decisions, data preparation, modelling procedures, interpretation of results, and final report content were reviewed, verified, and approved by the project author. 