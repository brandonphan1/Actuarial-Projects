# Auto Insurance Claims Risk Analysis & Loss Modeling

## Overview

This project analyzes auto insurance claims data to model claim severity and identify key drivers of insurance risk. Using regression and machine learning techniques, the analysis focuses on explaining variation in loss costs and improving model interpretability for actuarial applications.

The project emphasizes core property & casualty actuarial concepts, including loss modeling, risk segmentation, and feature analysis, while addressing practical modeling challenges such as multicollinearity and proxy variable bias.

---

## Objectives

* Model insurance claim severity using statistical and machine learning methods
* Identify key drivers of loss costs and quantify their impact
* Evaluate model performance and explanatory power
* Improve model interpretability by addressing multicollinearity and proxy variables
* Translate analytical findings into actuarial risk insights

---

## Methodology

### Data Preparation

* Cleaned and structured raw insurance claims dataset
* Encoded categorical variables for modeling
* Evaluated data quality and variable distributions

---

### Loss Modeling

* Implemented regression and machine learning models to predict claim severity
* Evaluated model performance using R² and residual analysis
* Achieved up to 81% explained variance in loss costs

---

### Feature Analysis

* Conducted feature importance analysis to identify primary risk drivers
* Identified geographic risk (location) as the dominant factor influencing claim severity
* Assessed relationships between policyholder attributes and loss outcomes

---

### Model Diagnostics & Interpretability

* Diagnosed multicollinearity among predictor variables
* Identified proxy variable effects (e.g., premium-related variables)
* Re-estimated models after removing leakage variables to validate model structure and robustness

---

## Key Results

* Model explained up to 81% of variation in insurance claim severity
* Geographic location emerged as the most significant driver of loss costs
* Income and vehicle-related factors contributed secondary effects
* Removal of proxy variables improved interpretability and reduced model bias
* Results highlight the importance of careful feature selection in actuarial modeling

---

## Repository Structure

* `data/` — insurance claims dataset
* `outputs/` — visualizations and model results
* `notebooks/` — modeling and analysis code

---

## Tools & Skills

* Python (pandas, scikit-learn)
* Excel (data exploration and validation)
* Regression analysis and machine learning
* Feature importance and model diagnostics
* Insurance analytics and risk modeling
