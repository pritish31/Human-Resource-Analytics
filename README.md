Here’s a well-structured `README.md` file for your HR Data Analytics project:

---

# **HR Data Analytics: Employee Attrition Prediction**

![HR Analytics](https://img.shields.io/badge/HR-Analytics-brightgreen) ![License](https://img.shields.io/badge/license-MIT-blue)

## **Project Overview**

Employee attrition poses significant challenges to organizations, including high costs of rehiring and training, loss of institutional knowledge, and reduced productivity. This project leverages data analytics and machine learning to explore the key factors contributing to employee attrition and provides actionable insights for improving retention strategies.

### **Key Objectives**
1. Identify factors contributing most to employee attrition.
2. Develop predictive models to classify employees at risk of leaving.
3. Provide actionable recommendations to improve employee retention.

---

## **Dataset**

The dataset contains **1470 employee records** with the following features:
- **Categorical**: Department, Job Role, Marital Status, Business Travel, etc.
- **Numerical**: Monthly Income, Total Working Years, Age, Distance from Home, etc.
- **Target Variable**: `Attrition` (Yes/No)

Source: [IBM HR Analytics Employee Attrition & Performance Dataset]
---

## **Exploratory Data Analysis**
The analysis includes:
1. **Univariate Analysis**: Distribution of key variables using histograms and boxplots.
2. **Bivariate Analysis**: Relationships between categorical and continuous variables, e.g., `Attrition` vs `MonthlyIncome`.
3. **Correlation Analysis**: Heatmap to identify feature dependencies.
4. **Feature Engineering**: Encoding categorical variables and creating dummy variables for machine learning.

---

## **Data Preprocessing**
- Removed irrelevant columns: `EmployeeCount`, `Over18`, and `StandardHours`.
- Addressed imbalanced dataset using stratified train-test split.
- Scaled numerical features using `StandardScaler`.
- Created dummy variables for categorical features.

---

## **Machine Learning Models**

| **Model**                 | **ROC-AUC Score** |
|---------------------------|--------------------|
| Logistic Regression       | 0.546             |
| Random Forest             | 0.543             |
| XGBoost                   | 0.622             |
| Support Vector Machine    | 0.500             |
| LightGBM                  | 0.609             |
| CatBoost                  | 0.586             |
| AdaBoost                  | 0.599             |

### **Best Performing Model**
- **XGBoost Classifier** achieved the highest performance with an ROC-AUC score of **0.622**. This model effectively identified employees at risk of leaving the organization.

---

## **Key Findings**

1. **Top Predictors of Attrition**:
   - **OverTime**: Employees working overtime are more likely to leave.
   - **MonthlyIncome**: Employees with lower income levels are at higher risk.
   - **Job Role**: Laboratory Technicians and Sales Representatives are more likely to leave.
   - **Marital Status**: Single employees show higher attrition rates.

2. **Insights from EDA**:
   - Employees with low job satisfaction, low environment satisfaction, and minimal years at the company are more likely to leave.
   - Research and Development employees are less likely to leave compared to other departments.

---

## **Recommendations**

1. Reduce overtime workloads to improve employee satisfaction.
2. Focus retention efforts on single employees in high-risk roles like Sales and HR.
3. Offer competitive salaries to employees at lower income levels.
4. Monitor and support employees with low years at the company.

---

## **Tools and Technologies**

- **Programming Language**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost, LightGBM, CatBoost
- **Visualization**: hvPlot, Matplotlib
- **IDE**: Jupyter Notebook

---

## **Project Structure**

```plaintext
├── data/
│   ├── HR-Employee-Attrition.csv
├── notebooks/
│   ├── hr_data_analysis.ipynb
├── results/
│   ├── model_comparison.csv
├── README.md
└── LICENSE
```

---

## **Contact**

If you have any questions, feel free to reach out
