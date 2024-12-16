# Breast Cancer Prediction Model

## Overview

This dataset was compiled from a collaborative study conducted at a leading oncology center to analyze factors affecting breast cancer outcomes. It includes anonymized data of over 300 patients who underwent various surgical procedures to remove their tumors. The study aimed to identify whether the patient survived (Alive) or not (Dead) after surgery.

This repository focuses on a data science project for breast cancer prediction and analysis using statistical tests and machine learning techniques. The project processes and analyzes the dataset to extract meaningful insights and builds predictive models for better healthcare decision-making.

---

## Project Objectives

The primary goal of this project is to:
1. Perform a detailed exploratory data analysis (EDA) on the breast cancer dataset.
2. Apply statistical tests to identify significant features influencing patient survival.
3. Develop a machine learning model for predicting patient outcomes.

---

## Column Descriptions

The dataset consists of 15 features, including demographics, protein levels, tumor information, and treatment details. The target variable is `Patient_Status`.

### Features:
- **Age**: Age of the patient.
- **Gender**: Male/Female indicator.
- **Protein1**: Protein marker 1 levels.
- **Protein2**: Protein marker 2 levels.
- **Protein3**: Protein marker 3 levels.
- **Protein4**: Protein marker 4 levels.
- **Tumour_Stage**: Stage of the tumor.
- **Histology**: Type of tumor histology.
- **ER status**: Estrogen receptor status.
- **PR status**: Progesterone receptor status.
- **HER2 status**: HER2 protein status.
- **Surgery_type**: Type of surgery performed.
- **Date_of_Surgery**: Date of the surgery.
- **Date_of_Last_Visit**: Date of the patient's last follow-up visit.
- **Patient_Status**: Target variable indicating whether the patient is `Alive` or `Dead`.

---

## Key Features

### Data Analysis
- Hypothesis testing (2-sample t-tests) was conducted to assess feature independence and select significant variables.
- Feature correlation analysis identified redundant or non-contributing features.

### Feature Selection
- Retained key features based on statistical significance:
  - `Age`, `Tumour_Stage`, `Surgery_type`, `Protein1`, `Protein2`
- Dropped non-significant features such as:
  - `ER status`, `PR status`, `HER2 status`

### Statistical Testing
- Conducted t-tests between numerical features and `Patient_Status` to evaluate feature dependency.

### Machine Learning Preparation
- Cleaned and preprocessed the dataset for model training.
- Removed irrelevant or redundant features for better performance.

---

## Steps Involved

### Data Preprocessing
- Cleaning and handling missing values.
- Statistical analysis for feature selection.

### Exploratory Data Analysis (EDA)
- Visualization of the dataset's key features and relationships.

### Feature Engineering
- Selection of relevant variables based on domain knowledge and statistical testing.

### Machine Learning (Future Work)
- Preparing data for training classification models (to be implemented).

---

## Observations and Use Cases

### Predictive Insights
- **Survival Prediction**: Features such as tumor stage, protein levels, and histology are analyzed to predict patient survival (`Patient_Status`).

### Variables
#### Dependent Variable (Target for Prediction)
- **Patient_Status**: Survival prediction (`Alive`/`Dead`).

#### Independent Variables (Predictors)
- `Age`, `Gender`, `Protein1`, `Protein2`, `Tumour_Stage`, `Histology`, `Surgery_type`, follow-up data.

---

## Key Challenges

1. **Missing Values**:
   - Null values in `Patient_Status` and `Date_of_Last_Visit` may limit survival analysis.
   
2. **Categorical Data**:
   - Columns like `Histology` and `Surgery_type` may require encoding for machine learning models.

---

## Future Work

- Develop machine learning models to predict patient outcomes.
- Optimize model performance through hyperparameter tuning.
- Expand feature engineering with domain-specific insights.

---

## Conclusion

This dataset provides a comprehensive view of breast cancer treatment and outcomes, offering opportunities for both descriptive analysis and predictive modeling. Researchers can explore clinical factors influencing survival, predict outcomes, and develop personalized treatment strategies using this dataset.

---
## Kaggle Dataset Link

https://www.kaggle.com/datasets/amandam1/breastcancerdataset/data

