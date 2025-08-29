# 🏭 Predictive Maintenance & Process Anomaly Detection – F&B Manufacturing  

This repository contains my project developed during the **Honeywell Campus Connect Hackathon 2025**.  
The goal was to design an **ML-based predictive maintenance system** that detects **process anomalies** in Food & Beverage (F&B) manufacturing (focus: baked goods), using **multivariable time-series data** from raw materials and equipment parameters.  

---

## 🚀 Problem Statement  
The challenge was to **predict and explain product quality deviations** while manufacturing is in progress.  
Anomaly = deviation of final product quality from expected standards.  

Constraints included:  
- Collecting **multivariable process data** (raw material deviations, mixer speed, oven temperature, process time, etc.)  
- Establishing **relationships** between process parameters and product quality  
- Ensuring the model provides **actionable insights** for operators  

---

## 🔧 Tech Stack  
- **Languages & Libraries**: Python, Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn  
- **Explainability**: SHAP  
- **Visualization/Dashboard (optional)**: Streamlit / Matplotlib dashboards  
- **Dataset**: Publicly available predictive maintenance datasets (UCI AI4I 2020, extended with synthetic anomaly labeling)  

---

## 📊 Workflow  

1. **Data Preprocessing & Cleaning**  
   - Outlier removal, handling missing values, standardization  
   - Feature engineering from raw process variables  

2. **Exploratory Data Analysis (EDA)**  
   - Distribution analysis  
   - Correlation heatmaps  
   - Multivariable trend plots  

3. **Modeling**  
   - Baseline: **Logistic Regression**  
   - Advanced: **Random Forest**  
   - Optimized: **XGBoost**  
   - Final: **XGBoost with Class Balancing** (handled rare anomalies)  

4. **Evaluation Metrics**  
   - Accuracy, Precision, Recall, F1-Score, ROC-AUC  
   - Focus on **Recall** to ensure anomalies are caught early  

5. **Explainability**  
   - SHAP values for feature importance  
   - Identified key drivers of product quality deviations  

6. **Visualization & Anomaly Scoring**  
   - Anomaly scores plotted over batches  
   - Highlighted regions of predicted quality risks  

---

## 📌 Results  
- Logistic Regression F1: **0.20**  
- Random Forest F1: **0.73**  
- XGBoost F1: **0.76**  
- Class-Balanced XGBoost F1: **0.79+** (with higher Recall)  

⚡ **Outcome**: A robust anomaly detection system that not only predicts deviations but also explains **why** they occur, making it useful for real-world F&B operators.  

---

## 🎯 Key Learnings  
- Handling **class imbalance** in industrial datasets  
- Importance of **explainability (SHAP)** for operator trust  
- **Time management** in delivering end-to-end ML within 2 days  
- Translating data science into **practical, actionable insights**  


## 🙏 Acknowledgements  
Thanks to **Honeywell Campus Connect Program** for the problem statement & hackathon opportunity.  
