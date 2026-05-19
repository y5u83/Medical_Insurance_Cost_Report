# 💰 Medical Insurance Cost Prediction Using Machine Learning

## 📌 Project Overview
This project presents a complete end-to-end data science workflow for predicting medical insurance charges using machine learning models. It was developed as part of the **CSC-44112 Advanced Applications of AI and ML** module.

The goal is to analyse how demographic and lifestyle factors influence insurance costs and to build models that accurately predict medical expenses.

---

## 🎯 Research Question
> Which demographic and lifestyle features most significantly affect medical insurance charges, and which machine learning model provides the most accurate predictions? 

---

## 📊 Dataset
- **Source:** Kaggle  
- **Link:** https://www.kaggle.com/datasets/mirichoi0218/insurance  
- **Records:** 1,338  
- **Features:**
  - Age
  - Sex
  - BMI (Body Mass Index)
  - Number of Children
  - Smoking Status
  - Region
  - Charges (Target Variable)

The dataset contains **no missing values**, making it ideal for machine learning modelling. [1](https://keeleacuk-my.sharepoint.com/personal/y5u83_students_keele_ac_uk/Documents/Microsoft%20Copilot%20Chat%20Files/25027657_part2.pdf)

---

## 🔍 Exploratory Data Analysis (EDA)
Key insights:
- Insurance costs are **highly skewed (right-skewed distribution)**
- **Smokers incur significantly higher charges**
- Strong correlations:
  - Smoking status → costs (~0.79)
  - Age → costs (~0.30)
- Interaction between **BMI and smoking** affects high costs [1](https://keeleacuk-my.sharepoint.com/personal/y5u83_students_keele_ac_uk/Documents/Microsoft%20Copilot%20Chat%20Files/25027657_part2.pdf)

---

## ⚙️ Models Implemented
The following regression models were used:

- ✅ Linear Regression (Baseline)
- ✅ Random Forest Regressor
- ✅ XGBoost Regressor (Best Model)

---

## 📈 Results

| Model | R² Score | RMSE ($) | MAE ($) |
|------|---------|----------|--------|
| Linear Regression | 0.744 | 5,826 | 4,012 |
| Random Forest | 0.861 | 4,289 | 2,431 |
| **XGBoost (Best)** | **0.874** | **4,102** | **2,198** |

✅ XGBoost achieved the highest performance, explaining ~87% of variance in insurance costs. [1](https://keeleacuk-my.sharepoint.com/personal/y5u83_students_keele_ac_uk/Documents/Microsoft%20Copilot%20Chat%20Files/25027657_part2.pdf)

---

## 🧠 Key Findings
- 🚬 **Smoking status is the most important predictor**
- 👤 Age and BMI strongly influence costs
- 🌳 Ensemble models outperform simple linear models
- 📉 Linear regression fails to capture non-linear relationships

---

## 🛠️ Technologies Used
- Python 3.12
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- XGBoost
- Google Colab

---

## 🚀 How to Run the Project
```bash
# Clone repository
git clone https://github.com/your-username/Medical_Insurance_Cost_Report.git

# Navigate to project directory
cd Medical_Insurance_Cost_Report

# Install dependencies
pip install -r requirements.txt

# Run notebook
