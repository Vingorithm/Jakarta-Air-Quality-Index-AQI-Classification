# Jakarta Air Quality Index (AQI) Classification

## 🌆 Overview
This project classifies Jakarta’s Air Quality Index (AQI) using machine learning based on pollutant concentration data from 2010 to 2023. It aims to predict daily air quality categories—**BAIK**, **SEDANG**, and **TIDAK SEHAT**—from key pollutants (PM10, PM2.5, SO2, CO, O3, NO2).

## 🎯 Purpose
- Support public awareness of air quality
- Assist policymakers in implementing environmental strategies
- Provide decision support for outdoor activity planning

## 📂 Dataset
- Source: Pemprov DKI Jakarta
- Data: Aggregated AQI values by station and date (2010–2023)
- Features: `pm10`, `pm25`, `so2`, `co`, `o3`, `no2`, `max`, `critical`, `category`

## 🧠 Models Used
- **SVM** (Support Vector Machine)
- **LightGBM** (Light Gradient Boosting Machine)
- **Random Forest**

## 🔧 Preprocessing Steps
- Missing value handling with imputation
- Outlier detection using IQR method
- One-hot and label encoding for categorical data
- Feature scaling and train-test split

## 📈 Model Evaluation

| Model         | Accuracy | F1-Score | Training Time |
|---------------|----------|----------|----------------|
| SVM           | 95.96%   | 95.55%   | 5.4 s          |
| LightGBM      | 99.96%   | 99.91%   | 15.8 s         |
| Random Forest | 99.97%   | 99.95%   | 12.3 s         |

**Best Model:** Random Forest (balance between speed and accuracy)

## 📊 Visualizations
- Heatmaps for feature correlation
- AQI distribution over time
- Pollutant trends using Altair and Plotly

## 📘 Methodology
Based on **CRISP-DM**:
1. Business Understanding
2. Data Understanding
3. Data Preparation
4. Modeling
5. Evaluation
6. Deployment (Conceptual)

## 🔗 Use Cases
- Public AQI apps
- Government decision dashboards
- Research in environmental informatics
