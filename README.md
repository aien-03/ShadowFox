## 📜 Internship Tasks Overview
For a detailed breakdown of all completed tasks, check [Tasks Overview](Tasks_Overview.md).





# Diabetes Prediction - Data Analysis and Machine Learning

## 📌 Project Overview
This project aims to analyze the **Diabetes dataset** and predict the likelihood of diabetes using **Machine Learning** techniques. We perform **Exploratory Data Analysis (EDA)**, visualize key patterns, and build a **Logistic Regression model** to classify diabetic vs. non-diabetic patients.

## 📊 Dataset Information
The dataset contains medical attributes related to diabetes risk, including:
- **Glucose Levels**
- **BMI (Body Mass Index)**
- **Blood Pressure**
- **Insulin Levels**
- **Age**
- **Pregnancies**
- **Skin Thickness**
- **Diabetes Pedigree Function** (Genetic Factor)

## 🎯 Research Questions
1. How do **Glucose levels and BMI** affect diabetes prediction?
2. Which factor has the **strongest correlation** with diabetes?

## 🔍 Exploratory Data Analysis (EDA)
We performed the following analyses:
- **Data Cleaning:** Handling missing values and duplicates.
- **Statistical Summary:** Checking means, medians, and distributions.
- **Correlation Analysis:** Identifying relationships between features.
- **Visualizations:** 
  - Histograms for distribution
  - Heatmaps for correlation
  - Boxplots for outliers

## 📈 Machine Learning Model - Logistic Regression
To predict diabetes, we built a **Logistic Regression Model** using **Scikit-Learn**.

### 🔹 Model Performance:
- **Accuracy:** 75%
- **Confusion Matrix:**


- **Classification Report:**
          precision    recall  f1-score   support
       0       0.81      0.80      0.81        99
       1       0.65      0.67      0.66        55
accuracy                           0.75       154

## 📌 Conclusion
- **Glucose levels** are a strong predictor of diabetes.
- **BMI and Age** also show a correlation with diabetes risk.
- The **Logistic Regression model** provides a 75% accuracy in predicting diabetes.

## 📂 Project Structure

## 🚀 How to Run the Project
1. Install dependencies:  
   ```bash
   pip install pandas numpy seaborn matplotlib scikit-learn
jupyter notebook
