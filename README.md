## Residential Property Valuation & Predictive Modeling

### **Project Overview**
This repository focuses on the application of supervised machine learning to predict residential real estate prices. Utilizing the Ames Housing dataset, this project moves beyond descriptive statistics to build a predictive framework that quantifies how specific property attributes—such as square footage, year built, and basement capacity—impact market valuation.

This analysis is designed for stakeholders in the mortgage, insurance, and real estate investment sectors who require data-driven appraisals over subjective estimates.

### **Core Analytical Objectives**
*   **Predictive Accuracy:** Develop a regression-based model to estimate sale prices with minimal error.
*   **Feature Attribution:** Identify which architectural and structural features contribute most significantly to a property's dollar value.
*   **Data Integrity:** Execute a clean data pipeline, including the handling of missing values and feature selection, to ensure model robustness.

### **Technical Stack**
*   **Modeling:** Scikit-Learn (Linear Regression, Train/Test Splitting)
*   **Data Processing:** Pandas, NumPy
*   **Visualization:** Seaborn, Matplotlib
*   **Dataset:** Ames Housing (Fetch via OpenML)

### **Methodology & Implementation**

**1. Data Preprocessing**
Filtering the 70+ available features into a subset of high-impact variables (e.g., Living Area, Year Built, Total Basement Square Footage) to prevent model overfitting and maintain interpretability.

**2. Exploratory Data Analysis (EDA)**
Implementing regression plots to visualize the linearity between square footage and price, ensuring the underlying assumptions of a linear model are met.

**3. Regression Modeling**
Training a Linear Regression model on 80% of the data and validating performance on the remaining 20%. The model evaluates the "marginal value" of individual features (e.g., "What is the average price increase for every additional square foot?").

**4. Performance Metrics**
The model is evaluated using:
*   **R-Squared (R²):** To determine the proportion of variance explained by the model.
*   **Mean Absolute Error (MAE):** To provide a tangible "dollar-amount" average error for predictions.

### **Key Insights**
*   **Primary Value Driver:** Above-grade living area consistently serves as the strongest predictor of value.
*   **Depreciation vs. Appreciation:** The `YearBuilt` coefficient successfully captures the premium placed on newer construction versus historical properties.

### **Installation & Usage**

1. **Clone the repository**
```bash
git clone https://github.com/thesjhu/housing-prediction-analysis
```

2. **Install requirements**
```bash
pip install pandas scikit-learn matplotlib seaborn
```

### **Author**
**Sijie Hu**  
MS in Information Systems, Data Analytics | Bar. **Execute Analysis**
