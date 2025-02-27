# Medical Charges Prediction Model  

## 📌 Project Overview  
This project aims to build a machine learning model that predicts **medical charges** for patients based on factors like **age, BMI, smoking status, and region**. 
By leveraging **clustering and regression techniques**, this model provides insights into how different factors influence medical costs.  

## 📂 Dataset  
The dataset used contains the following features:  
- **age** – Age of the primary beneficiary  
- **sex** – Gender of the beneficiary  
- **bmi** – Body mass index (BMI)  
- **children** – Number of dependents covered by insurance  
- **smoker** – Whether the individual is a smoker  
- **region** – Residential region (northeast, southeast, southwest, northwest)  
- **charges** – Medical charges billed by health insurance  

## 🛠️ Methods Used  
### 🔹 Data Preprocessing  
- Checked for **missing values** (none found)  
- **Exploratory Data Analysis (EDA)** for understanding feature distributions and correlations  
- **Categorical encoding** for non-numeric features  

### 🔹 Machine Learning Models  
- **Clustering Approaches**  
  - K-Means Clustering  
  - Hierarchical Clustering  
  - Manual grouping to identify high-cost patient segments  
- **Regression Models**  
  - **Ordinary Least Squares (OLS) Regression** – Predicts medical charges based on all features  
  - **Random Forest Model** – Used for comparison and fairness evaluation  

### 🔹 Model Evaluation  
- **R-Squared & Adjusted R-Squared** – Measures model accuracy  
- **Feature Importance Analysis (LIME)** – Identifies key factors influencing medical charges  
- **Fairness Metrics**  
  - Precision, Recall, and F1-score  
  - False Positive Rate (FPR) and False Negative Rate (FNR) across different demographic groups  
  - Evaluation of demographic parity and equalized odds  

## 🔍 Key Findings  
✅ **Smoking status** is the most significant factor affecting medical charges.  
✅ **BMI and Age** also have a notable impact, with higher BMI correlating to higher costs.  
✅ The model shows **high accuracy and fairness** across most groups, but certain demographic subgroups (e.g., young adults) exhibit lower recall.  
✅ The dataset is **clean but lacks real-world complexity** (e.g., medical history, insurance type).  

## 🚀 Future Improvements  
- **Expand feature set** – Include additional attributes such as pre-existing conditions and insurance type.  
- **Improve robustness** – Introduce synthetic noise and simulate real-world data issues.  
- **Enhance fairness analysis** – Use more fairness evaluation metrics.  
- **Experiment with more models** – Test deep learning techniques for better predictions.  
