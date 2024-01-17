![Static Badge](https://img.shields.io/badge/2022-orange)
![Static Badge](https://img.shields.io/badge/development-yellow)
![Static Badge](https://img.shields.io/badge/RStudio-lightblue)


![Thumbnail](https://raw.githubusercontent.com/4nuG/predicting-house-prices/main/Predicting_House_Prices.png)

# Table of Contents

1. [Project Overview](#project-overview)
2. [Key Steps](#key-steps)
   - [Data Wrangling](#data-wrangling)
   - [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
   - [Predictive Model Building](#predictive-model-building)
   - [Model Validation](#model-validation)
   - [Conclusion](#conclusion)
3. [Full Project Write-Up](#full-project-write-up)

# Project Overview:
House price estimator for a house dataset using JMP. 

## Datasets
Datasets are called AmesHousing Data Training_Validation.jmp and AmesHousing Data Scoring.jmp and are in the repo. 

## Requirements
- JMP Pro 16

# Key Steps

## Data Wrangling:
- Outlier analysis was performed using continuous variables.
- Outliers at specific rows were identified and removed for analysis.
- Missing data analysis revealed no significant issues, and a principal component (PC) analysis was conducted.

## Exploratory Data Analysis (EDA):
- PC analysis identified key predictors, providing insights into the dataset structure.
- Exploration of PC1 and PC2 highlighted predictors related to living area and rooms above ground.

## Predictive Model Building:
- A standard least squares model was initially created.
- After addressing outliers, a refined model achieved an improved R-square value of 0.9509.
- Additional models, including stepwise and lasso, were employed and compared.

## Model Validation:
- Validation processes, such as Max Validation RSquare and model comparisons, were executed.
- Lasso model emerged as the best fit for scoring data, achieving a validation RSquare of 0.9087.

## Conclusion:
- The standard least squares model excelled for training data (RSquare: 0.9509).
- The stepwise Max RSquare model performed best for validation data (RSquare: 0.9238).
- When applied to scoring data, the lasso model exhibited superior performance (RSquare: 0.9087).
- Identified predictors from the lasso model were crucial for accurate predictions.

For a detailed exploration and findings, refer to the full project write-up in the repository.

