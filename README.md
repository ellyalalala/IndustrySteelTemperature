# IndustrySteelTemperature


# 🏭 Industry Steel Temperature Prediction

## 📋 Project Description
This is a graduation project focused on developing a machine learning model to predict the temperature of steel at various processing stages, helping reduce energy consumption in production.  
> **Client:** Metallurgical plant LLC *"So We Harden Steel"*.
> In order to reduce production costs, the metallurgical plant LLC “So we harden steel” decided to reduce energy consumption at the stages of steel processing. You have to develop a model that predicts the temperature of steel.

**Objective:** Predict the final steel temperature based on technological parameters and alloy composition.

---

## 📂 Data
The dataset contains ~20,000 observations with the following features:
- Chemical composition
- Temperature at previous stages
- Processing time at each stage
- Oxygen supply rate

**Target variable:** **Final steel temperature (°C).**

---

## 🧪 Approach
✅ EDA:
- Removed outliers  
- Handled missing values  
- Explored feature correlations  

✅ Data preparation:
- Feature scaling
- Encoding categorical features (if applicable)

✅ Models:
- Linear Regression
- Random Forest
- Gradient Boosting (CatBoost)

✅ Hyperparameter tuning via `GridSearchCV`.

---

## 📈 Results
🏆 Best performing model: **CatBoost**  
📊 Metrics on test set:
- MAE: **5.44 °C**
- R²: **0.93**

The model demonstrates high prediction accuracy and is suitable for industrial deployment to optimize energy costs.

---

## 🚀 How to Run
1️⃣ Clone the repository:
```bash
git clone https://github.com/ellyalalala/IndustrySteelTemperature.git
cd IndustrySteelTemperature

Tech Stack
Python 3.x

Pandas, NumPy, Matplotlib, Seaborn

Scikit-learn

CatBoost
