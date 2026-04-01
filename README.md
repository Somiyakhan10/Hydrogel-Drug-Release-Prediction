# 💊 Hydrogel Drug Release & Efficacy Prediction System

![Python Version](https://img.shields.io/badge/Python-3.8%2B-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Random%20Forest-green)
![Streamlit](https://img.shields.io/badge/Streamlit-1.28.0-red)
![License](https://img.shields.io/badge/License-MIT-yellow)

## 🧪 Project Overview

**Hydrogel Drug Release Prediction System** is a machine learning-powered web application that predicts drug release profiles and therapeutic efficacy of hydrogels based on formulation parameters. This tool helps researchers and pharmaceutical scientists optimize polymer formulations for controlled drug delivery systems.

### 🎯 Key Features

- ✅ **Dual Prediction Models**: 
  - Predicts 48-hour cumulative drug release (mg/ml)
  - Predicts therapeutic efficacy score (0-1 normalized)
- ✅ **5 Key Input Parameters**:
  - Polymer Type (PEG, Gelatin, Chitosan)
  - Polymer Concentration (0.5-10.0%)
  - Crosslink Density (0.1-1.0)
  - Temperature (20-40°C)
  - pH (5.5-7.4)
- ✅ **High Accuracy Models**: R² > 0.98 for drug release, R² > 0.88 for efficacy
- ✅ **Interactive Dashboard**: User-friendly interface with real-time predictions
- ✅ **Model Comparison**: Gradient Boosting vs Random Forest performance analysis
- ✅ **Feature Importance**: Understand which parameters most affect outcomes

---

## 📸 Dashboard Screenshots

### Main Dashboard Interface
<img width="947" height="413" alt="image" src="https://github.com/user-attachments/assets/bab50c73-1667-45fe-bb1f-e0c9129aa3ea" />

*The interactive dashboard showing all input parameters and prediction results*

### Drug Release Prediction
<img width="944" height="439" alt="image" src="https://github.com/user-attachments/assets/707329cb-33ec-466f-b6ec-fe9ad922204c" />


*Real-time prediction of drug release concentration with confidence intervals*

### Model Performance Metrics
<img width="946" height="429" alt="image" src="https://github.com/user-attachments/assets/1520bbb5-39b2-4c2d-a5dc-062612aa1474" />


*Performance comparison between Drug Release and Efficacy models*

---

## 🧠 How It Works

### Machine Learning Pipeline

The system uses **Random Forest Regressors** trained on synthetic data derived from real-world hydrogel formulation principles:

```python
# Model Architecture
- Algorithm: Random Forest Regressor
- Estimators: 200 trees
- Max Depth: 10 (Drug Release) / 8 (Efficacy)
- Features: 5 input parameters
- Training Data: 500 synthetic samples
