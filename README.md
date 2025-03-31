# ⚡ Energy Demand Prediction Using Machine Learning

A project focused on forecasting electricity demand using historical UK National Grid data (2009–2024), powered by a suite of regression and ensemble learning algorithms.

---

## 📌 Why This Project Matters

Accurate electricity demand forecasting is vital for grid operators, utility companies, and policymakers. It allows for:

- ⚖️ Efficient energy distribution
- 🏭 Optimized power generation scheduling
- 🧠 Demand-response automation
- 🌱 Renewable energy integration
- 💰 Cost-saving strategies

In the face of climate change and energy transition, being able to **predict usage patterns** ensures a **stable, sustainable, and economical** power system.

---

## 📂 Dataset Overview

- **Source**: Historic UK grid electricity demand dataset (2009–2024)
- **Granularity**: Half-hourly measurements
- **Fields Used**:
  - `settlement_date`: Date of measurement
  - `settlement_period`: Half-hour interval index
  - `demand`: Energy consumed in MW

### ➕ Feature Engineering

To boost model performance, we derived several temporal and behavioral features such as:
- Year, Month, Day, Day of Week, Quarter
- Hour, Half-Hour
- Peak/Off-Peak Labeling
- Weekend Indicator
- Seasonal Grouping

---

## 🧠 Machine Learning Models Used

To model the complex patterns in electricity demand, several regression algorithms were applied and compared:

### 1. **Linear Regression**  
Simple yet effective baseline to model linear relationships.

### 2. **Support Vector Regressor (SVR)**  
A robust model that can capture nonlinear relationships by using kernel tricks.

### 3. **Gradient Boosting Regressor**  
Ensemble technique that builds strong predictive models using many weak learners in sequence. It showed **excellent performance** in this project by minimizing error effectively.

---

## 📊 Evaluation Metrics

Models were evaluated using:

- **MAE (Mean Absolute Error)**
- **RMSE (Root Mean Squared Error)**
- **R² Score (Coefficient of Determination)**

These metrics ensure we capture both average and worst-case prediction errors.

---

## 📈 Results Visualization

![image](https://github.com/user-attachments/assets/01121d09-e8dd-4de0-944c-95146d403587)


## 💡 Insights from Data

- Electricity demand follows strong **daily and seasonal trends**.
- Peak usage occurs during working hours and cold months.
- Demand drops significantly on weekends and holidays.
- Weather, economy, and special events influence demand patterns (future integration possible).

---

## 🛠 How to Run This Project

### ✅ Requirements

- Python 3.7+
- Jupyter Notebook or VSCode
- Install dependencies:

```bash
pip install -r requirements.txt
