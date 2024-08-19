# Predictive Maintenance for Wind Turbine Generators

## Project Overview

Renewable energy sources are crucial for a sustainable future, and wind energy is a leading player in this domain. This project focuses on enhancing the operational efficiency of wind turbines through predictive maintenance. By predicting generator failures, we aim to enable timely maintenance actions that reduce costs and prevent unexpected breakdowns.

## Business Context

Predictive maintenance uses sensor data to monitor and predict the degradation of wind turbine components. Early detection of potential failures allows for cost-effective and timely maintenance, ensuring uninterrupted energy production.

## Objective

The primary objective of this project is to develop and optimize machine learning models that can accurately predict generator failures. These models will help in identifying when a generator is likely to fail, allowing for preventive maintenance actions that minimize operational costs.

## Data Description

- **Train.csv**: Training dataset with 20,000 observations and 40 features.
- **Test.csv**: Testing dataset with 5,000 observations and the same structure as the training data.
- **Target Variable**: Binary indicator of failure (1 = Failure, 0 = No Failure).

## Exploratory Data Analysis (EDA)

- The dataset was analyzed for distribution, skewness, outliers, and feature importance.
- Histograms and boxplots were generated for each feature to visualize data distribution.

## Data Pre-processing

- **Data Splitting**: The data was split into training, validation, and test sets.
- **Missing Value Imputation**: Median imputation was used for missing values.
- **Class Imbalance Handling**: SMOTE was used for oversampling, and Random UnderSampling was applied to handle class imbalance.

## Model Development

Multiple models were developed and compared, including:

- **Random Forest**
- **Gradient Boosting**
- **AdaBoost**
- **XGBoost**
- **Decision Tree**

### Model Evaluation and Selection

- The models were evaluated based on Recall, Precision, Accuracy, and F1 scores.
- Cross-validation was performed to ensure robustness.

### Best Model

- The "Tuned XGBoost Classifier" with oversampling was selected as the best model due to its strong recall, accuracy, and balanced performance across all metrics.

## Business Insights

- **Feature Importance**: V36 was identified as the most important feature, followed by V14, V26, V16, V18, V1, and V21.
- **Strategic Focus**: The organization is advised to focus on F1 score to balance the cost of repair and replacement in the long term.

## Conclusion

This project successfully identified the best machine learning model for predicting generator failures in wind turbines. The insights provided can help the organization optimize maintenance strategies and reduce operational costs.

## Future Work

- Further optimization of models using more advanced techniques.
- Exploration of additional features and external data sources to enhance model accuracy.
- Deployment of the model in a real-time monitoring system for continuous predictive maintenance.


---

This project serves as a comprehensive guide for implementing predictive maintenance in wind energy systems, ensuring operational efficiency and cost savings.

