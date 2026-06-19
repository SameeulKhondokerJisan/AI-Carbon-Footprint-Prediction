# AI-Based Predictive Modeling of Individual Carbon Footprints Using Behavioral and Energy Consumption Data

## 🌍 Project Overview

Climate change has become one of the most pressing global challenges, and reducing carbon emissions is essential for sustainable development. Traditional carbon footprint calculators often rely on static emission factors and generalized assumptions, resulting in less accurate estimates.

This project presents an AI-powered predictive framework that estimates individual carbon footprints using behavioral and energy consumption data. By leveraging advanced machine learning algorithms and Explainable AI (XAI), the system provides accurate emission predictions while identifying the key lifestyle factors contributing to carbon emissions.

The framework combines behavioral indicators such as transportation habits, dietary choices, waste generation patterns, and energy consumption metrics to create a personalized and data-driven carbon footprint estimation model.

---

## 🎯 Objectives

The primary objectives of this project are:

- Develop an AI-based model for predicting individual carbon footprints.
- Analyze the impact of behavioral and energy consumption factors on carbon emissions.
- Compare multiple machine learning algorithms for predictive performance.
- Improve model transparency through Explainable AI techniques.
- Provide actionable insights that can support sustainable decision-making.

---

## 🔍 Problem Statement

Traditional carbon footprint estimation methods:

- Depend on fixed emission factors.
- Require extensive manual input.
- Lack personalization.
- Fail to capture dynamic lifestyle variations.
- Offer limited explainability.

To overcome these limitations, this project utilizes machine learning models capable of learning complex relationships between behavioral patterns and carbon emissions while providing transparent explanations for predictions.

---

## 📊 Dataset Description

The dataset contains various lifestyle, behavioral, transportation, and energy-related features that influence carbon emissions.

### Key Features

#### Personal Information
- Body Type
- Sex

#### Lifestyle & Consumption
- Diet Type
- Social Activity Frequency
- Monthly Grocery Bill
- Number of New Clothes Purchased Monthly

#### Transportation
- Vehicle Type
- Vehicle Monthly Distance (KM)
- Air Travel Frequency
- Transport Mode

#### Energy Consumption
- Heating Energy Source
- Energy Efficiency Indicators

#### Waste Management
- Waste Bag Size
- Waste Bag Weekly Count
- Recycling Habits

### Target Variable

- **CarbonEmission** (Predicted Carbon Footprint)

---

## ⚙️ Data Preprocessing

Several preprocessing steps were performed before model training:

### Data Cleaning
- Handling missing values
- Correcting inconsistent entries

### Missing Value Treatment
- Median Imputation (Numerical Features)
- Mode Imputation (Categorical Features)

### Outlier Removal
- Interquartile Range (IQR) Method

### Feature Encoding
- One-Hot Encoding for categorical variables

### Feature Scaling
- StandardScaler normalization

### Dataset Splitting
- 80% Training Data
- 20% Testing Data

---

## 🤖 Machine Learning Models

Three machine learning models were implemented and compared.

### 1. Random Forest Regressor

Configuration:

- Number of Trees: 400
- Max Features: sqrt
- Minimum Samples Leaf: 2
- Parallel Training Enabled

Advantages:

- Handles non-linear relationships
- Robust against overfitting
- Good feature importance analysis

---

### 2. XGBoost Regressor

Configuration:

- Estimators: 1200
- Maximum Depth: 6
- Learning Rate Optimized
- Subsample: 0.9
- Column Sample Rate: 0.9

Advantages:

- High predictive accuracy
- Handles complex feature interactions
- Excellent generalization capability

---

### 3. Multi-Layer Perceptron (MLP)

Architecture:

- Hidden Layer 1: 256 Neurons
- Hidden Layer 2: 128 Neurons
- Hidden Layer 3: 64 Neurons

Other Settings:

- ReLU Activation
- Adam Optimizer
- Early Stopping
- StandardScaler Pipeline

Advantages:

- Captures complex patterns
- Suitable for non-linear relationships
- Deep learning-based prediction

---

## 📈 Model Evaluation Metrics

The models were evaluated using:

### R² Score
Measures prediction accuracy.

### RMSE
Root Mean Squared Error.

### MAE
Mean Absolute Error.

### Cross Validation
5-Fold Cross Validation was used to improve model reliability and reduce overfitting.

---

## 🏆 Results

### Model Performance Comparison

| Model | R² Score |
|---------|---------|
| Random Forest | 0.977 |
| XGBoost | 0.975 |
| MLP Regressor | 0.977 |

### Key Findings

- XGBoost achieved outstanding predictive performance.
- Random Forest demonstrated strong interpretability and robustness.
- MLP effectively captured complex patterns but required more computational resources.
- Transportation behavior emerged as the strongest contributor to carbon emissions.

---

## 📊 Important Insights

### Transportation Impact

Key contributors:

- Vehicle Type
- Monthly Travel Distance
- Air Travel Frequency

Individuals who:

- Travel more frequently
- Use petrol-powered vehicles
- Fly often

produce significantly higher carbon emissions.

---

### Dietary Habits

Diet type influences carbon footprints.

Findings showed:

- Vegetarian diets generally produce lower emissions.
- Certain non-vegetarian dietary patterns contribute higher emissions.

---

### Energy Consumption

Heating energy source significantly affects emissions.

Observed Sources:

- Electricity
- Natural Gas
- Wood

Wood-based heating generated comparatively higher emissions.

---

### Waste Generation

Higher waste production is associated with:

- Increased carbon footprints
- Higher resource consumption
- Lower sustainability practices

---

## 🔬 Explainable AI (XAI)

To improve transparency, SHAP (Shapley Additive Explanations) was integrated.

### SHAP Benefits

- Explains model decisions
- Ranks feature importance
- Improves trust in AI predictions
- Supports policy-making and sustainability planning

### SHAP Visualizations

- Beeswarm Plot
- Waterfall Plot
- Global Feature Importance
- Local Prediction Explanations

---

## 📌 Most Influential Features

According to SHAP analysis, the most impactful factors include:

1. Vehicle Monthly Distance
2. Air Travel Frequency
3. Vehicle Type
4. Heating Energy Source
5. Waste Bag Weekly Count
6. Diet Type
7. Social Activity Frequency
8. Monthly Grocery Bill

---

## 🛠 Technologies Used

### Programming Language
- Python

### Libraries
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- XGBoost
- SHAP

### Development Environment
- Jupyter Notebook

---

## 📂 Project Structure

```text
AI-Carbon-Footprint-Prediction/
│
├── data/
│   ├── raw_dataset.csv
│   └── processed_dataset.csv
│
├── notebooks/
│   └── carbon_footprint_prediction.ipynb
│
├── models/
│   ├── random_forest.pkl
│   ├── xgboost.pkl
│   └── mlp.pkl
│
├── outputs/
│   ├── evaluation_results.csv
│   └── prediction_results.csv
│
├── images/
│   ├── correlation_heatmap.png
│   ├── shap_beeswarm.png
│   ├── shap_waterfall.png
│   └── visualizations/
│
├── README.md
├── requirements.txt
└── LICENSE
```

---

## 🚀 Future Work

Future enhancements may include:

- Real-world user datasets
- IoT sensor integration
- Satellite environmental data
- Real-time carbon monitoring
- Mobile application deployment
- Personalized sustainability recommendations
- Carbon reduction advisory system
- LIME-based explainability integration

---

## 🌱 Potential Applications

This framework can be used by:

### Individuals
- Monitor personal carbon emissions
- Make environmentally conscious decisions

### Organizations
- Sustainability assessment
- Carbon management initiatives

### Governments
- Environmental policy planning
- Climate action programs

### Researchers
- Environmental analytics
- Explainable AI studies
- Sustainability modeling

---

## 👨‍💻 Team Members

| Name | ID |
|--------|--------|
| Md. Siyam Hossain | 0242310005341223 |
| Nadim Mahmud | 0242310005341247 |
| Jannatul Jeor Bushra | 0242310005341291 |
| Sameeul Khondokar Jisan | 0242310005341365 |

---

## 📚 References

- Lundberg, S. M., & Lee, S. I. (2017). A Unified Approach to Interpreting Model Predictions.
- Sethi, S., & Jain, M. (2019). Application of Random Forest Regression for Predicting Carbon Emissions.
- Chandel, S., Shukla, A., & Khatri, S. (2020). Predicting Carbon Footprints Using Machine Learning Algorithms.
- Sharma, A., & Singh, R. (2021). Integrating IoT-Based Sensors for Dynamic Carbon Footprint Prediction.
- Zhang, J., et al. (2018). Machine Learning-Based Approach for Predicting Individual Carbon Footprints.

---

## 📄 License

This project was developed for academic and research purposes under Daffodil International University.

---

### ⭐ If you find this project useful, consider giving it a star!
