# Hydrogel Drug Release Prediction System

A machine learning-powered web application that predicts drug release profiles and therapeutic efficacy of hydrogels based on formulation parameters. This tool helps researchers and pharmaceutical scientists optimize polymer formulations for controlled drug delivery systems.

**Author: Somiya Khan**

---

## 📊 Drug Release & Efficacy Distributions

| Drug Release at 48h (mg/ml) | Efficacy Score |
|:---------------------------:|:--------------:|
<img width="1168" height="395" alt="image" src="https://github.com/user-attachments/assets/bb58993e-13af-4aec-9dea-2a1eacd91341" />


---

## 📋 Sample Predictions by Polymer Type

| Polymer Type | Drug Release (mg/ml) | Efficacy Score |
|--------------|---------------------|----------------|
| Chitosan | 24.5 | 0.95 |
| Gelatin | 21.5 | 0.85 |
| PEG | 11.5 | 0.65 |

---

## 📊 Drug Release & Efficacy Score by Polymer Type

<img width="1161" height="405" alt="image" src="https://github.com/user-attachments/assets/def7c721-e0ba-4d47-8adc-d34804837fed" />


*Comparison of drug release (mg/ml) and efficacy score across different polymer types (Chitosan, Gelatin, PEG)*

---

## 🎯 Key Features

| Feature | Description |
|---------|-------------|
| **Dual Prediction Models** | Predicts 48-hour cumulative drug release (mg/ml) and therapeutic efficacy score (0-1 normalized) |
| **5 Input Parameters** | Polymer Type, Polymer Concentration, Crosslink Density, Temperature, pH |
| **High Accuracy** | R² > 0.98 for drug release, R² > 0.88 for efficacy |
| **Interactive Dashboard** | User-friendly interface with real-time predictions |
| **Model Comparison** | Gradient Boosting vs Random Forest performance analysis |
| **Feature Importance** | Understand which parameters most affect outcomes |


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
