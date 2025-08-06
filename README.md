# Healthcare Premium Prediction

A machine learning project that predicts healthcare insurance premiums based on various demographic and health factors. The project uses age-based model segmentation and includes a Streamlit web application for interactive predictions.

## 📋 Project Overview

This project predicts healthcare insurance premiums using machine learning algorithms. The model is segmented based on age groups (≤25 years and >25 years) to improve prediction accuracy. The solution includes comprehensive data analysis, feature engineering, model training, and a user-friendly web interface.


## 🔬 Methodology

### Age-Based Model Segmentation
The project uses two separate models based on age groups:
- **Young Group (≤25 years)**: Uses `model_young.joblib` and `scaler_young.joblib`
- **Rest Group (>25 years)**: Uses `model_rest.joblib` and `scaler_rest.joblib`

### Feature Engineering
1. **Normalized Risk Score**: Calculated based on medical history
   - Diabetes: 6 points
   - Heart disease: 8 points
   - High blood pressure: 6 points
   - Thyroid: 5 points
   - No disease: 0 points
   - Maximum possible score: 14 (normalized to 0-1 scale)

2. **Categorical Encoding**: One-hot encoding for categorical variables
3. **Feature Scaling**: MinMax scaling for numerical features

### Machine Learning Pipeline
1. **Data Preprocessing**: Cleaning and feature engineering
2. **Exploratory Data Analysis**: Understanding data patterns and distributions
3. **Feature Selection**: Identifying important features
4. **Model Training**: Age-segmented model training
5. **Model Evaluation**: Performance assessment using various metrics
6. **Model Deployment**: Streamlit web application

## 🚀 Getting Started

### Prerequisites
```bash
pip install streamlit pandas numpy scikit-learn joblib xgboost matplotlib seaborn
```

### Running the Application
1. Open the app directory:
   ```bash
   cd app
   ```

2. Run the Streamlit application:
   ```bash
   streamlit run main.py
   ```

3. Open your browser and go to `http://localhost:8501`

   
