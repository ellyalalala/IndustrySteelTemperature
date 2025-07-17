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
2️⃣ Install dependencies:
pip install -r requirements.txt
3️⃣ Run the notebook:
jupyter notebook IndustrySteelTemperature.ipynb


---

Tech Stack
Python 3.x

Pandas, NumPy, Matplotlib, Seaborn

Scikit-learn

CatBoost
