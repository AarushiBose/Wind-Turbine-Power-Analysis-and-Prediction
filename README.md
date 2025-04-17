# ⚡ WindSight: Wind Turbine Power Analysis and Forecasting System

![image](https://github.com/user-attachments/assets/53b06104-7da0-40d9-8bbc-6ecc1ca7c777)


## 🌬️ Project Overview 

**WindSight** is a comprehensive system built to support wind energy companies in fulfilling their contractual power generation obligations under Power Purchase Agreements (PPA).  

A wind energy company in Turkey, currently generating an average of **185.61 MW** daily, is bound by a PPA to deliver **167.05 MW** of power per day to the government. While this exceeds the required target, any generation falling below **150.35 MW** (a 10% deviation from the target) incurs penalties. Therefore, accurate forecasting and performance analysis are essential for **optimized resource allocation**, **penalty avoidance**, and **revenue maximization**.  

WindSight leverages **2018 SCADA data** — including wind speed, direction, and turbine power output at 10-minute intervals — to:
- Analyze operational patterns
- Predict future power generation using ML models
- Assist in policy-making and planning for stable power supply  

By applying advanced machine learning models like **Random Forest, XGBoost, LSTM**, and **Hybrid Ensemble models**, the project helps maintain generation within the stable operation zone and ensures **compliance with regulatory thresholds** while maximizing efficiency.

🔗 **Dataset**: [Wind Turbine SCADA Dataset (Kaggle)](https://www.kaggle.com/datasets/berkerisen/wind-turbine-scada-dataset)  

📈 **Key Metrics**:
- **Contractual Daily Target**: 167.05 MW  
- **Average Generation**: 185.61 MW  
- **Penalty Threshold**: Below 150.35 MW  
- **Permissible Deviation**: 5–10% below target  

🗂️ **Data Features**:
- `Date/Time`: Timestamp at 10-minute intervals  
- `LV ActivePower (kW)`: Real-time turbine power output  
- `Wind Speed (m/s)`: Measured at hub height  
- `Theoretical_Power_Curve (kW)`: Manufacturer-defined output  
- `Wind Direction (°)`: Turbine orientation based on wind  

WindSight not only empowers better **forecasting** but also enhances strategic decisions for **stable, penalty-free, and high-revenue operations** in the wind energy sector.


---

## 🧭 Methodology

The overall workflow of the project is illustrated below:

![image](https://github.com/user-attachments/assets/adcc1eb6-dd8b-4088-819e-b96c7a1c2e33)

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

## 📈 Model Performance Comparison  

| Model                 | R² Score | MAE (MW) | RMSE (MW) |
|----------------------|----------|----------|-----------|
| Random Forest        | 84.80%   | 37.15    | 58.71     |
| XGBoost              | 81.96%   | 41.94    | 63.95     |
| LSTM                 | -5.84%   | 137.75   | 165.04    |
| Hybrid (XGBoost+LSTM)| **93.05%** | **30.06** | **42.30**  |

> ✅ **Best Model:** `Hybrid (XGBoost + LSTM)` with **R² = 93.05%**


