# Brain Age Prediction of Healthy Adults Using Multivariate Regression Analysis

## Project Overview

This project focuses on predicting the brain age of healthy adults using multivariate regression analysis. Brain age prediction is a crucial task in identifying deviations from typical aging processes, which may indicate early signs of neurodegenerative diseases such as Alzheimer's. The study leverages MRI imaging data and explores various feature engineering techniques to enhance the predictive performance of machine learning models.

## Table of Contents

- [Brain Age Prediction of Healthy Adults Using Multivariate Regression Analysis](#brain-age-prediction-of-healthy-adults-using-multivariate-regression-analysis)
  - [Project Overview](#project-overview)
  - [Table of Contents](#table-of-contents)
  - [Data and Feature Engineering](#data-and-feature-engineering)
    - [Feature Engineering Techniques](#feature-engineering-techniques)
  - [Model Construction](#model-construction)
  - [Results and Analysis](#results-and-analysis)
  - [Conclusions and Future Work](#conclusions-and-future-work)


## Data and Feature Engineering

The dataset used in this study comprises MRI data from 1,600 healthy adult volunteers. Key features include:

- **Demographic Information**: Gender, age.
- **MRI-derived Metrics**: Volume, surface area, thickness, curvature, etc.

### Feature Engineering Techniques

- **Binning**: Conversion of continuous features to categorical features through binning.
- **Grouped Aggregate Features**: Age groups were created, and statistical measures like mean, median, and standard deviation were calculated within these groups.
- **Ratio and Aggregate Features**: New features were generated, such as total brain volume and gray-to-white matter ratio.
- **Feature Selection**: Recursive Feature Elimination with Cross-Validation (RFECV) was used for automatic feature selection.

## Model Construction

Several machine learning models were employed to predict brain age:

- **Linear Regression**: Used as a baseline model for performance comparison.
- **Gradient Boosting Decision Trees (GBDT)**: XGBoost and LightGBM models were implemented to capture complex, nonlinear relationships in the data.
- **Hyperparameter Tuning**: Bayesian optimization was utilized to fine-tune model hyperparameters, enhancing model robustness and preventing overfitting.

## Results and Analysis

- **Best Performing Model**: LightGBM with grouped aggregate features showed the best performance in predicting brain age.
- **Evaluation Metrics**: The models were evaluated using Mean Absolute Error (MAE), Pearson Correlation Coefficient (PCC), and R² score.

## Conclusions and Future Work

- **Conclusions**: The project highlights the importance of sophisticated feature engineering in improving the accuracy of brain age prediction models. LightGBM was identified as the most effective model in this study.
- **Future Work**: Further research could focus on refining these models, exploring additional data sources, and applying the models in clinical settings for early diagnosis of neurodegenerative diseases.

