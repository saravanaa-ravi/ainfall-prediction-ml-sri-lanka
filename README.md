# 🌧️ Rainfall Prediction Using Machine Learning (Sri Lanka)

## 📌 Project Overview
Rainfall prediction is crucial for agriculture, water resource management, and disaster preparedness.  
This project focuses on predicting **whether it will rain the next day** using historical weather data from Sri Lanka and multiple machine learning models.

The project emphasizes:
- Robust **data preprocessing**
- **Exploratory Data Analysis (EDA)**
- Feature engineering for **time-series & seasonality**
- Training and evaluating multiple ML algorithms

---

## 📊 Dataset Information
- **Source:** Sri Lanka Weather Dataset (Kaggle)
- **Type:** Time-series weather data
- **Key Features:**
  - `time` – Date & time of observation
  - `rain_sum` – Daily rainfall (mm)
  - `precipitation_sum` – Daily precipitation (mm)
  - `temperature_2m_mean` – Mean temperature (°C)
  - `windspeed_10m_max` – Maximum wind speed (km/h)
  - `city` – Weather station location

---

## 🛠️ Data Preprocessing & Feature Engineering
### ✔ Data Cleaning
- Standardized column names
- Converted time to datetime format
- Removed duplicate records
- Ensured correct numeric data types

### ✔ Missing Value Handling & Outliers
- Time-based interpolation
- Forward & backward filling
- Outlier removal using **IQR method**

### ✔ Feature Engineering
- Lag features (`rain_lag1`, `rain_lag7`)
- Rolling averages (`rain_roll7`, `rain_roll30`)
- Cyclical encoding for seasonality (`month_sin`, `month_cos`)

### ✔ Encoding & Scaling
- One-hot encoding for categorical variables
- Min-Max scaling for numeric features

### ✔ Feature Selection
- Correlation-based feature removal
- Dimensionality reduction using **PCA**

---

## 🤖 Machine Learning Models Implemented

| Algorithm | Accuracy |
|---------|----------|
| MLP | 89.72% |
| **Support Vector Machine (SVM)** | **99.73%** |
| Random Forest | 89.78% |
| Logistic Regression | 88.91% |
| KNN | 89.01% |
| Decision Tree | 89.36% |

### 🏆 Best Performing Model
**Support Vector Machine (SVM)** achieved the highest accuracy of **99.73%**, demonstrating excellent generalization and stability.

---

## 👨‍💻 My Contribution
**Saravanan R (IT24102073)**  
- Designed and implemented the **Support Vector Machine (SVM)** model  
- Performed hyperparameter tuning using **GridSearchCV**
- Achieved **99.73% accuracy**, the best among all models

---

## ⚖️ Ethical Considerations
- Dataset anonymization
- Balanced class distribution
- Multiple evaluation metrics to reduce bias
- Transparent documentation of methods

---

## 🚀 Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

---

## 📌 Conclusion
The project demonstrates how effective preprocessing, feature engineering, and model selection significantly improve rainfall prediction accuracy.  
Among all tested models, **SVM proved to be the most reliable** for this dataset.

---

## 📚 References
REFERENCES

1. Dataset (Kaggle):
[1] Kaggle Weather Dataset, Kaggle, 2024. [Online]. Available: https://www.kaggle.com/
[Accessed: 20-Oct-2025].

2. Documentation (Scikit-learn):
[2] Scikit-learn Documentation, Version 1.5, scikit-learn.org, 2024. [Online]. Available:
https://scikit-learn.org/
[Accessed: 20 -Oct-2025].
