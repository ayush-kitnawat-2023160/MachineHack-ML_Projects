# 📶 Mobile Network Performance Prediction - MachineHack Challenge

Welcome to my solution for the **MachineHack** challenge:  
**"Predicting Measured Download Speed (Mbps)"** using machine learning techniques on mobile network performance data.

---

## 📌 Problem Statement

Build a machine learning model to predict **measured_download_Speed (Mbps)** based on various features including:
- Signal strength  
- Latency  
- Jitter  
- Device type  
- Battery level  
- And more...

---

## 🚀 Approach

The following steps were taken to solve the challenge:

### 🔧 Data Preprocessing
- Loaded `Train.csv` and `Test.csv`.
- Identified and handled missing values.
- Dropped unwanted or redundant columns.
- Applied **OneHotEncoding** for categorical features using `OneHotEncoder`.

## 🧪 Libraries Used

- `pandas`, `numpy`  
- `scikit-learn`  
- `xgboost`, `lightgbm`, `catboost`  
- `matplotlib` *(optional for visualization)*

### 📊 Model Building
Implemented and compared the following models:
- ✅ **RandomForestRegressor** (Best Performing)
- XGBoost Regressor
- LightGBM Regressor
- CatBoost Regressor

## 📊 Model Evaluation

Models were evaluated using:
- **MAE**: Mean Absolute Error  
- **MSE**: Mean Squared Error  
- **RMSE**: Root Mean Squared Error  
- **R² Score**: Coefficient of Determination  

| Model         | MAE     | MSE       | RMSE     | R² Score | Accuracy (%)   |
|---------------|---------|-----------|----------|----------|----------------|
| ✅ Random Forest | **7.5054** | **215.4509** | **14.6782** | **0.9967** | **99.67%**       |
| CatBoost      | 13.3196 | 366.9506  | 19.1560  | 0.9944   | 99.44%         |
| XGBoost       | 36.1206 | 2342.2510 | 48.3968  | 0.9645   | 96.45%         |
| LightGBM      | 37.3377 | 2457.2039 | 49.5702  | 0.9628   | 96.28%         |

➡️ **Random Forest** outperformed all other models in every metric.

## 📬 Author

**Ayush Kitnawat**



