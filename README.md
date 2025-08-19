# 🩺 Predicting Diabetes with Machine Learning on CDC Health Indicators Dataset  

## 📌 Project Overview  
This project applies **machine learning classification models** to predict diabetes risk using the **CDC BRFSS 2015 Health Indicators dataset**.  
The goal is to build predictive models that can **classify individuals as healthy, pre-diabetic, or diabetic**, identify key health indicators, and provide insights for **public health strategies**.  

---

## 🎯 Objectives  
- **Classify Individuals** → Accurately classify people into healthy, pre-diabetic, or diabetic categories.  
- **Identify Key Predictors** → Discover the most important features influencing diabetes risk.  
- **Support Public Health** → Deliver actionable insights for early intervention and awareness campaigns.  

---

## 📊 Dataset: CDC BRFSS 2015  
- **Entries**: 253,680  
- **Features**: 21 health indicators (BMI, Age, General Health, Blood Pressure, etc.)  
- **Characteristics**:  
  - No missing values  
  - Mix of binary & continuous data  
  - **Imbalanced target classes** → Addressed using **SMOTE (Synthetic Minority Oversampling Technique)**  

---

## 🛠 Data Preprocessing Pipeline  
1. **Encoding & Scaling** → Handled categorical + numerical features  
2. **SMOTE** → Balanced minority diabetic/pre-diabetic classes  
3. **Train-Test Split** → 80% training / 20% testing  

---

## 🔑 Feature Selection  
- **Recursive Feature Elimination (RFE)** with Logistic Regression  
- **Tree-based Importance** from Random Forest & XGBoost  
- **SHAP Values** for explainability  

### Key Positive Correlations  
- Poor General Health (GenHlth)  
- Difficulty Walking (DiffWalk)  
- High Blood Pressure (HighBP)  
- Age  

### Key Negative Correlations  
- Higher Income & Education  
- Vegetable Consumption  

---

## 🤖 Machine Learning Models Used  
- **Logistic Regression** → Baseline model  
- **Decision Tree**  
- **Random Forest**  
- **XGBoost** → Best performing model  

---

## 📈 Results & Model Evaluation  
- **XGBoost** & **Random Forest** delivered the **highest accuracy & robustness**  
- **ROC-AUC Scores**:  
  - Logistic Regression → 0.94  
  - Decision Tree → 0.93  
  - Random Forest → 0.95  
  - XGBoost → 0.95  

📌 **Best Model: XGBoost** (highest AUC, excellent predictive power)  

---

## ✅ Key Findings  
1. Machine learning models can **reliably predict diabetes risk**.  
2. **Ensemble methods (RF, XGBoost)** outperform simpler models.  
3. Important features align with **medical literature** (Age, BMI, Blood Pressure, Lifestyle factors).  
4. **SMOTE** improves detection of underrepresented diabetic cases.  
5. Future potential for **clinical integration** and **deep learning exploration**.  

---

## 🔧 Tools & Technologies  
- **Python** (Pandas, NumPy, Matplotlib, Seaborn)  
- **Scikit-learn** (Logistic Regression, Decision Tree, Random Forest)  
- **XGBoost** (Gradient Boosting Classifier)  
- **SHAP** (Explainable AI)  
- **SMOTE** (Imbalanced-learn)  

---

## 📚 References  
- Pedregosa, F. et al. (2011). *Scikit-learn: Machine Learning in Python*. JMLR.  
- Chen, T., & Guestrin, C. (2016). *XGBoost: A Scalable Tree Boosting System*. KDD.  
- Hastie, T., Tibshirani, R., & Friedman, J. (2009). *The Elements of Statistical Learning*.  
- Géron, A. (2019). *Hands-On Machine Learning with Scikit-Learn, Keras & TensorFlow*.  


 
