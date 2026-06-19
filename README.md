# AI-Based Predictive Modeling of Individual Carbon Footprints Using Behavioral and Energy Consumption Data

## Overview
This project develops an AI-driven predictive framework to estimate individual carbon footprints using behavioral and energy consumption data. The system leverages machine learning algorithms and explainable AI techniques to provide accurate carbon emission predictions and identify the key lifestyle factors contributing to emissions.

## Objectives
- Predict individual carbon emissions using machine learning.
- Compare the performance of Random Forest, XGBoost, and MLP models.
- Identify the most influential factors affecting carbon footprints.
- Improve model transparency using SHAP explainability.

## Features
- Data preprocessing and feature engineering
- Outlier detection and removal using IQR
- Random Forest Regressor
- XGBoost Regressor
- Multi-Layer Perceptron (MLP)
- Model evaluation using R², RMSE, and MAE
- SHAP-based feature importance analysis
- Data visualization and insights generation

## Dataset
The dataset contains behavioral and energy consumption attributes including:

- Transportation habits
- Vehicle type
- Monthly travel distance
- Air travel frequency
- Diet type
- Waste generation
- Energy consumption patterns
- Heating energy source
- Social and lifestyle behaviors

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- SHAP
- Matplotlib
- Seaborn
- Jupyter Notebook

## Machine Learning Models
| Model | Purpose |
|---------|---------|
| Random Forest | Ensemble learning for regression |
| XGBoost | Gradient boosting prediction |
| MLP Regressor | Deep learning-based prediction |

## Results
| Model | R² Score |
|---------|---------|
| Random Forest | 0.977 |
| XGBoost | 0.975 |
| MLP Regressor | 0.977 |

The results demonstrate strong predictive performance, with transportation behavior, vehicle usage, air travel frequency, and energy consumption identified as major contributors to carbon emissions.

## Explainable AI
SHAP (Shapley Additive Explanations) was used to:
- Interpret model predictions
- Rank feature importance
- Visualize feature contributions
- Support transparent decision-making

## Project Structure
```text
├── data/
├── notebooks/
├── models/
├── outputs/
├── images/
├── README.md
└── requirements.txt
