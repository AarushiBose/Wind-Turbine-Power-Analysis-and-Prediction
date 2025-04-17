# ⚡ WindSight: Wind Turbine Power Analysis and Forecasting System

(![image](https://github.com/user-attachments/assets/404344bd-3947-4be7-8630-bb3040a6b957)

## 🌬️ Project Overview  
**WindSight** is a comprehensive system designed to analyze wind turbine performance data and predict future power output using advanced machine learning models. By leveraging historical SCADA data, this project enables better planning, operational efficiency, and insights into wind energy production.

---

## 🧭 Methodology

The overall workflow of the project is illustrated below:

(![image](https://github.com/user-attachments/assets/adcc1eb6-dd8b-4088-819e-b96c7a1c2e33))

> The process begins with raw SCADA data, followed by preprocessing, feature engineering, data exploration (visualizations), and predictive modeling using various ML algorithms.

---

## 🚀 Features  

- **Data Analysis**: In-depth exploratory data analysis of turbine operations  
- **Power Prediction**: Predictive modeling using ML algorithms to forecast energy output  
- **Performance Metrics**: Compare turbine efficiency across varying environmental conditions  
- **Visualization**: Interactive and static visualizations to uncover trends and anomalies  

---

## 🛠️ Technologies Used  

- **Programming**: Python  
- **Libraries**:  
  - `Pandas`, `NumPy` – Data manipulation and preprocessing  
  - `Scikit-learn`, `XGBoost` – Machine learning models  
  - `Matplotlib`, `Seaborn`, `Plotly` – Visualizations  
  - `Jupyter Notebooks` – Development and analysis environment  

---

## 📊 Dataset  

The project utilizes **2018 SCADA data** from Turkish wind farms, featuring:

- ⏱️ 10-minute interval readings from multiple turbines  
- 🌪️ Wind speed at hub height (m/s)  
- ⚡ Power output (kW)  
- 🌡️ Environmental conditions (temperature, pressure)  
- ⚙️ Operational parameters (blade pitch, rotor speed)  
- 🟥 Turbine status flags  

---

## 📈 Model Performance Comparison  

| Model                 | R² Score | MAE (MW) | RMSE (MW) |
|----------------------|----------|----------|-----------|
| Random Forest        | 84.80%   | 37.15    | 58.71     |
| XGBoost              | 81.96%   | 41.94    | 63.95     |
| LSTM                 | -5.84%   | 137.75   | 165.04    |
| Hybrid (XGBoost+LSTM)| **93.05%** | **30.06** | **42.30**  |

> ✅ **Best Model:** `Hybrid (XGBoost + LSTM)` with **R² = 93.05%**


