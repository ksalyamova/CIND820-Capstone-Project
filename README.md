# CIND 820 Capstone Project

## Project Overview

This project investigates socioeconomic vulnerability across Toronto neighbourhoods using demographic, housing, education, labour market, and low-income indicators derived from the Toronto Neighbourhood Profiles dataset.

The objective is to identify the socioeconomic characteristics associated with vulnerability, classify neighbourhoods with similar profiles, and support evidence-based planning and resource allocation.

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

## Current Status

Completed:

* Exploratory Data Analysis
* Indicator Selection
* Feature Relationship Analysis
* PCA
* K-Means Clustering
* Vulnerability Classification

Planned:

* Predictive modelling
* Forecasting analysis
* Final project report
* Interactive visualizations

* (old version)

# CIND 820 Capstone Project

## Project Summary

This project investigates socioeconomic vulnerability and neighborhood level low-income prevelance 

## Research Questions

### Research Question #1. 

Which socioeconomic variables are the strongest predictors of neighborhood-level low-income prevalence in Toronto?

What results will I get?

The analysis will identify which variables have the greatest influence on low-income prevalence, such as:

- Unemployment rate
- Median household income
- Education attainment
- Housing affordability indicators
- Labour force participation

Modeeling: will be using correlation analysis, Logistic Regression coefficients, and Random Forest feature importance scores, I will rank these variables according to their predictive power.

I will:
Conduct exploratory data analysis (EDA).
Examine correlations between predictors and low-income prevalence.
Build Logistic Regression and Random Forest models.
Compare feature importance across models.
Validate model performance using accuracy, precision, recall, and F1-score.

What will I do with these results?
I will identify the socioeconomic factors most strongly associated with poverty risk.

How could these results change current actions?
Instead of distributing (financial) resources based mainly on historical poverty rates, organizations can focus on the underlying drivers of vulnerability.


### Research Question #2

Which Toronto neighborhoods demonstrate the highest predicted socioeconomic vulnerability based on income, employment, education, and housing indicators?

The analysis will produce:

A vulnerability score for each neighborhood.
Risk classifications (Low, Medium, High).
Geographic maps showing vulnerable areas.
Neighborhood clusters with similar socioeconomic characteristics.

Modelling:
- Build classification models.
- Create vulnerability risk scores.
- Use clustering techniques (K-Means and/or Hierarchical Clustering).
- Visualize results through geographic maps and dashboards.
- Compare neighborhoods across multiple indicators.

What will I do with these results?
I will identify which neighborhoods are most vulnerable and require priority intervention.


How could these results change current actions?
Resources could be allocated more strategically.

### Research Question 3

How are low-income prevalence and housing burden indicators expected to change across Toronto neighborhoods over time?

What results will I get?

Forecasting models will estimate:
Future low-income prevalence.
Future housing burden trends.
Neighborhoods likely to improve.
Neighborhoods likely to experience increasing vulnerability.
How will I ensure I answer it fully?

Modelling:
- Analyze historical trends.
- Develop forecasting models.
- Compare projected outcomes across neighborhoods.
- Evaluate forecast accuracy.
- Visualize trends through forecasting dashboards.

What will I do with these results?

I will identify emerging socioeconomic risks before they become major problems.

How could these results change current actions?

Decision-makers can move from reactive planning to proactive planning.

## Analyst Role and Decision Context

This project simulates the role of a municipal socioeconomic data analyst supporting:
- Toronto city planners
- Housing policy analysts
- Community development agencies
- Nonprofit organizations

The analysis supports decisions related to:
- Affordable housing prioritization
- Employment support allocation
- Community investment planning
- Early intervention strategies for vulnerable neighborhoods

## ## Expected Project Impact (Conclusion)

Research Question 1 identifies the drivers of poverty risk.

Research Question 2 identifies which neighborhoods are most vulnerable today.

Research Question 3 forecasts which neighborhoods may become more vulnerable in the future.

Together, these findings support evidence-based planning, targeted resource allocation, and proactive policy intervention across Toronto communities.

