# 🏥 Diabetes Prediction & Readmission Analysis

## 📌 Project Overview
This project focuses on **predicting diabetes and analyzing hospital readmission patterns** using machine learning and statistical techniques. The dataset consists of **medical records of diabetic patients**, and we perform:
- **Data Imputation** using K-Nearest Neighbors (KNN)
- **Logistic Regression for Diabetes Prediction**
- **Hospital Readmission Analysis** based on HbA1c levels
- **Feature Importance Analysis**

## 📂 Dataset Information
- **Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/machine-learning-databases/00296/dataset_diabetes.zip)
- **Data Type**: Patient records with demographics, medical history, and lab results.
- **Key Features**:
  - `Glucose`, `BloodPressure`, `SkinThickness`, `Insulin`, `BMI`
  - `A1Cresult`: Indicates HbA1c levels
  - `Change`: Whether medication was changed
  - `Readmitted`: If the patient was readmitted
  - `diag_1`: Primary diagnosis code

## 🛠️ Data Preprocessing
✔️ **Missing Value Handling**: Replaced missing values using **KNN Imputation**
✔️ **Feature Scaling**: Standardized numerical features
✔️ **Encoded Outcome Variable** as -1 (No Diabetes) and 1 (Diabetes)
✔️ **Feature Engineering**: Grouped diagnosis codes into broader medical conditions

## 🤖 Machine Learning Models
### **1️⃣ Diabetes Prediction using Logistic Regression**
- **Preprocessing**: Standardized input features
- **Accuracy**: **76.19%**
- **Feature Importance**:
  - **Glucose** & **BMI** are the strongest predictors of diabetes
  - **Blood Pressure & Skin Thickness** have minimal impact

### **2️⃣ Hospital Readmission Analysis**
- **Analyzed HbA1c levels vs medication change & readmission**
- **Key Findings**:
  - Patients with **higher HbA1c (>8%)** are more likely to have their medication changed
  - **Measured HbA1c patients** are **more likely to be readmitted** than those without measurements
  - **Diabetes patients have higher readmission rates** than other conditions

## 📊 Visualization & Insights
- **ROC Curve** to evaluate classification performance
- **Heatmaps & Bar Charts** to show correlations
- **Stacked Bar Plots** for readmission rates across different conditions

## 📌 How to Run the Project
1. **Clone the repository**
   ```bash
   git clone https://github.com/Vasanthrk29/HealthCare.git
   cd HealthCare
   ```
2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```
3. **Run the Python script**
   ```bash
   python HealthCare.py
   ```

## 🚀 Future Enhancements
🔹 Use **Deep Learning (Neural Networks)** for better accuracy  
🔹 Explore **Survival Analysis** for hospital readmission prediction  
🔹 Deploy as a **Web App** for real-time patient risk assessment  

## 🏆 Contributors
👨‍💻 **Your Name** – [GitHub Profile](https://github.com/Vasanthrk29)

## 📜 License
This project is licensed under the **MIT License**. Feel free to use and modify!
