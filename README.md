# Healthcare Cost Prediction Model

## Project Overview

This data science project aims to predict customer healthcare costs for a leading Health Insurance company. By leveraging machine learning techniques, we develop a model that estimates individual medical costs billed by health insurance, helping to tailor services and assist customers in planning their healthcare expenses more effectively.

## Dataset

The primary dataset, `insurance.csv`, contains the following features:

- `age`: Age of the primary beneficiary (int)
- `sex`: Gender of the insurance contractor (male/female)
- `bmi`: Body mass index (float)
- `children`: Number of dependents covered by the insurance plan (int)
- `smoker`: Smoking status of the beneficiary (yes/no)
- `region`: Beneficiary's residential area in the US (4 regions)
- `charges`: Individual medical costs billed by health insurance (float, target variable)

A separate `validation_dataset.csv` is provided for model validation, containing similar features without the `charges` column.

## Methodology

1. **Data Preprocessing**:
   - Handle missing values and outliers
   - Encode categorical variables
   - Normalize numerical features

2. **Exploratory Data Analysis**:
   - Visualize relationships between features and healthcare costs
   - Identify key correlations and patterns

3. **Feature Engineering**:
   - Create interaction terms (e.g., age * bmi)
   - Develop categorical feature combinations

4. **Model Development**:
   - Split data into training and testing sets
   - Train multiple regression models (e.g., Linear Regression, Random Forest, Gradient Boosting)
   - Perform hyperparameter tuning

5. **Model Evaluation**:
   - Use metrics such as MAE, MSE, and R-squared
   - Conduct cross-validation for robustness

6. **Validation**:
   - Apply the best-performing model to `validation_dataset.csv`
   - Analyze prediction accuracy on new data

## Tools Used

- Python
- Pandas for data manipulation
- Scikit-learn for model development
- Matplotlib/Seaborn for data visualization
- Jupyter Notebooks for analysis and documentation