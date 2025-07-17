# 🏭 Industry Steel Temperature Prediction

## 📋 Project Description
This is a graduation project focused on developing a machine learning model to predict the temperature of steel at various processing stages, helping reduce energy consumption in production.  
> **Client:** Metallurgical plant LLC *"So We Harden Steel"*.

**Objective:** Predict the final steel temperature based on technological parameters and alloy composition.

---

## 📂 Data

The project uses multiple datasets collected from steel processing equipment. Each dataset contains thousands of records related to different stages and parameters of the process:

- **Electrode data:** measurements of arc electrode usage 
- **Bulk materials (by observation):** quantities of bulk materials added 
- **Bulk materials (by time):** time‑series of bulk material additions 
- **Gas data:** gas flow rates and usage 
- **Temperature measurements:** observed temperatures during processing 
- **Wire materials (by observation):** wire material usage 
- **Wire materials (by time):** time‑series of wire material feed 

All datasets are merged and preprocessed to build a model predicting the final steel temperature.


---

## 🧪 Approach
✅ Exploratory Data Analysis (EDA):

Initial data inspection and feature understanding

✅ Data preprocessing:

Computed total power feature

Merged all datasets on a common key

Replaced missing (NaN) values with zeros

Removed irrelevant features and outliers

Performed correlation analysis

✅ Model training:

Linear Regression

DecisionTreeRegressor

RandomForestRegressor

CatBoostRegressor

LGBMRegressor

✅ Model testing and evaluation

✅ Feature importance analysis

✅ Hyperparameter tuning via `GridSearchCV`.

---

## 📈 Results
🏆 Best performing model: **CatBoost**  
Cross‑validated MAE: ~5.9
MAE on test set: 6.41

📊 Key factors influencing temperature:

Initial steel temperature
Processing time


📝 Conclusions
To reduce energy consumption during steel processing at ООО «So We Harden Steel», we built a machine learning model to predict the final temperature.

After analyzing and preprocessing the data, we trained and compared several models. The best performing one was CatBoostRegressor, which achieved an MAE of 6.41 on the test set.

We recommend deploying CatBoostRegressor for production use. Additionally, feature importance analysis showed that focusing on initial temperature and processing time provides the biggest impact on the final temperature and should be the focus for further process optimization.
---

## 🚀 How to Run
1️⃣ Clone the repository:
git clone https://github.com/ellyalalala/IndustrySteelTemperature.git
cd IndustrySteelTemperature

2️⃣ Install dependencies:
pip install -r requirements.txt

3️⃣ Run the notebook:
jupyter notebook IndustrySteelTemperature.ipynb


---

Tech Stack:

Python 3.x

Pandas, NumPy, Matplotlib, Seaborn

Scikit-learn

CatBoost
