# Week 3: Statistical Analysis and Predictive Modeling using R

## Project overview
This project uses the public Titanic passenger dataset to examine factors associated with survival and build a logistic-regression classification model.

## Dataset
- Source: https://raw.githubusercontent.com/mwaskom/seaborn-data/master/titanic.csv
- Outcome: `survived` (0 = No, 1 = Yes)
- Predictors: passenger class, sex, age, family aboard, fare, and port of embarkation.
- `alive` is excluded because it duplicates the outcome; high-missingness `deck` and redundant `embark_town` are also excluded.

## Methods
1. Data cleaning and median/mode imputation.
2. Chi-square test for association between sex and survival.
3. Welch two-sample t-test comparing age by survival group.
4. Shapiro-Wilk age-distribution check and Spearman correlations.
5. Stratified 80/20 train-test split and 5-fold cross-validation.
6. Logistic regression with accuracy, precision, recall, F1, confusion matrix, and ROC-AUC.
7. VIF screening and ROC/calibration visualizations.

## Run
Open `week3_titanic_model.R` in RStudio and run the full script. Required packages are installed by the script if missing. Outputs are saved in `week3_outputs/`.

## Important
Run the script yourself in RStudio and include genuine screenshots of the console, model output, confusion matrix, ROC curve, and diagnostic files in your submitted report. Do not describe preview or expected results as executed results.
