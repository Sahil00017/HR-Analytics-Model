# 📊 HR Analytics Project

## 🏆 Overview
Employee retention and workforce management are critical challenges for organizations. This project explores **HR Analytics**, analyzing employee data to uncover patterns that influence attrition, job satisfaction, and workforce demographics.  

The dataset (`general_data.csv`) consists of various employee attributes such as **age, job role, education, attrition status, monthly income, job satisfaction,** and more. This analysis aims to provide valuable insights for HR professionals to enhance employee retention strategies.  

## 🎯 Objectives
- 🔍 **Understand Workforce Demographics:** Analyze employee distribution across different roles, departments, and education levels.
- 📊 **Data Visualization & Statistical Insights:** Use visualizations and statistical measures to highlight significant workforce trends.
- 🤖 **Build a Predictive Model:** Develop a machine learning model to predict employee attrition.


## 🚀 Features & Analysis
The notebook follows a structured approach with the following key components:

### 1️⃣ **Data Loading & Cleaning**
   - 📂 Load dataset (`general_data.csv`) using **Pandas**.
   - 🧹 Check for missing values and handle them appropriately.
   - 🔄 Explore data types and ensure consistency for analysis.

### 2️⃣ **Exploratory Data Analysis (EDA)**
   - 📜 **Summary Statistics:** Compute basic statistics like mean, median, and standard deviation.
   - 📈 **Distribution Analysis:** Visualize employee demographics (age, experience, salary).
   - 🔗 **Correlation Analysis:** Examine relationships between different features.
   - 🚪 **Attrition Breakdown:** Understand attrition rates across various attributes.

### 3️⃣ **Visualization & Insights**
To better understand employee trends, multiple visualizations were created:

#### 📊 **Categorical Features Analysis**
- **Bar Charts for Categorical Variables:**  
  - Each categorical variable (e.g., **Job Role, Education, Attrition**) was analyzed using **bar plots**.  
  - The value counts of each category were displayed using **black-colored bar charts** for a clear contrast.  
  - **Example:** Employee distribution across different **departments** and **education levels**.

#### 📈 **Numerical Features Analysis**
- **Histogram & Boxplot for Continuous Variables:**  
  - Each numerical feature (e.g., **Age, Monthly Income, Years at Company**) was analyzed with **histograms and boxplots**.
  - **Histograms** show the overall distribution of values.
  - **Boxplots** help in identifying outliers and median trends.
  - These visualizations provide insights into salary ranges, tenure, and workforce demographics.

The combination of **bar charts, histograms, and boxplots** ensures a detailed and visually clear representation of HR data.

### 4️⃣ **Machine Learning Model**
   - 🤖 **Training a Classification Model:** Predict employee attrition.
   - 🏋️ **Model Training:** Implement machine learning techniques for prediction.
   - 📊 **Evaluation Metrics:** Assess model performance using accuracy, precision, recall, and F1-score.

## ⚙️ Installation & Requirements
To run this project locally, ensure you have the following dependencies installed:

### 📦 **Dependencies**
This project requires **Python 3.x** and the following libraries:
```bash
pip install pandas numpy matplotlib seaborn scipy scikit-learn
```

## 🛠 Running the Notebook
1. 🚀 Clone the repository:
```bash
  git clone https://github.com/Sahil00017/HR-Analytics-Regression
  cd HR-Analytics-Regression
```
2. 📂 Open Jupyter Notebook:
```bash
  jupyter notebook
```
3. ▶️ Run HR_Analytics.ipynb sequentially.

## 📑 Dataset Information  
The dataset contains anonymized employee records with the following key features:  

| 🏷️ **Feature**          | 📋 **Description**                                      |
|-------------------------|--------------------------------------------------------|
| 🆔 **Employee ID**      | Unique identifier for employees                        |
| 🎂 **Age**              | Employee's age                                         |
| 👨‍💼 **Job Role**       | Designation within the company                        |
| 🏢 **Department**       | Department where the employee works                    |
| 🎓 **Education**        | Education level (e.g., Bachelor's, Master's, PhD)     |
| 💰 **Monthly Income**   | Salary details                                        |
| 📆 **Total Working Years** | Overall experience in years                        |
| ⏳ **Years at Company**  | Number of years in the current company                |
| 😊 **Job Satisfaction** | Employee job satisfaction rating (1-4)                |
| ❌ **Attrition**        | Whether the employee left the company (`Yes`/`No`)    |

## 📈 Model Performance

### 🏋️ Training Performance:
- **Training Accuracy:** `0.6116`
- **Precision:** `0.6195`
- **Recall:** `0.5824`
- **Confusion Matrix(Training Data):**
  ```
  [[341 191], [223 311]]
  ```
- **📊 Classification Report (Training Data):**

| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| **0** | 0.60      | 0.64   | 0.62     | 532     |
| **1** | 0.62      | 0.58   | 0.60     | 534     |
| **Accuracy** |   |   | **0.61** | **1066** |
| **Macro Avg** | 0.61 | 0.61 | 0.61 | 1066 |
| **Weighted Avg** | 0.61 | 0.61 | 0.61 | 1066 |


### 🧪 **Testing Performance:**
- **Testing Accuracy:** `0.5815`
- **Precision:** `0.5875`
- **Recall:** `0.5311`
-  **Confusion Matrix(Testing Data):**
  ```
   [[113 66],[83 94]]
  ```
-  **Classification Report(Testing Data):**

| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| 0     | 0.58      | 0.63   | 0.60     | 179     |
| 1     | 0.59      | 0.53   | 0.56     | 177     |
| **Accuracy** |       |        | **0.58** | **356** |
| **Macro avg** | 0.58  | 0.58   | 0.58     | 356     |
| **Weighted avg** | 0.58  | 0.58   | 0.58     | 356     |


### 📌 **Observations**
- The **training accuracy (61%)** is slightly higher than **testing accuracy (58%)**, suggesting moderate generalization.
- The **precision and recall values** indicate that the model is **reasonably good but can be improved** with feature engineering or hyperparameter tuning.
- **False positives and false negatives** in the confusion matrix highlight areas where the model misclassifies employees.

## 📜 License
This project is open-source and available under the **MIT License**.
