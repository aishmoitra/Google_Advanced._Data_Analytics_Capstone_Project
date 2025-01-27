# Salifort Motors Employee Retention Analysis

## Overview
Salifort Motors is facing challenges with employee retention. This project uses data analytics and machine learning techniques to identify the factors contributing to employee turnover and provide actionable recommendations for reducing attrition.

---

## Project Goals
1. Analyze historical employee data to understand the drivers of attrition.
2. Build predictive models to identify employees most at risk of leaving.
3. Deliver actionable recommendations to improve HR policies and workplace culture.

---

## Dataset

### Summary
- **Source**: `HR_dataset.csv`, Source: [Kaggle](https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics-and-job-prediction?resource=download)
- **Rows**: 14,999
- **Columns**: 10

### Key Variables:
- `satisfaction_level`: Employee satisfaction score.
- `last_evaluation`: Last performance evaluation score.
- `number_project`: Number of projects handled.
- `average_monthly_hours`: Average hours worked per month.
- `time_spend_company`: Tenure in years.
- `Work_accident`: Whether the employee had a workplace accident.
- `left`: Whether the employee left (1) or stayed (0).
- `promotion_last_5years`: Promotions in the last 5 years.
- `Department`: Employee's department.
- `salary`: Employee salary category (low, medium, high).

---

## Analysis Process

### 1. Exploratory Data Analysis (EDA)
- **Visualizations**:
  - Bar plots for categorical variables.
  - Correlation heatmaps for numerical variables.
  - Box plots to examine relationships with attrition.
- **Key Insights**:
  - High attrition among employees with low satisfaction and high workloads.
  - Tenure of four years shows a notable dissatisfaction trend.
  - Salary levels (`low`) significantly correlate with turnover.

### 2. Predictive Modeling
- Models Built:
  - Logistic Regression
  - Decision Tree Classifier
  - Random Forest Classifier
- **Best Model**: Random Forest, with higher accuracy and ability to rank feature importance.
- **Key Metrics**:
  - Accuracy, Precision, Recall, F1 Score, and AUC.

### 3. Recommendations
- Cap the number of simultaneous projects to prevent burnout.
- Investigate dissatisfaction among employees with four years of tenure.
- Revise overtime and workload policies to improve work-life balance.
- Communicate performance expectations and provide proportionate rewards.
- Regularly review and adjust salary structures to retain top talent.

---

## How to Use This Repository

### Files Included:
- **`salifort_motors_analysis.ipynb`**:
  - Full analysis notebook containing data preprocessing, EDA, and modeling.
- **`executive_summary.pdf`**:
  - High-level summary of findings and recommendations for stakeholders.

### Steps to Reproduce:
1. Clone the repository.
2. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```
3. Open the analysis notebook:
   ```bash
   jupyter notebook salifort_motors_analysis.ipynb
   ```
4. Follow the analysis workflow in the notebook.

---

## Technologies Used
- **Data Analysis**: Python (pandas, numpy, seaborn, matplotlib)
- **Machine Learning**: Scikit-learn, XGBoost
- **Visualization**: Matplotlib, Seaborn

---

## Results
- Random Forest achieved the highest performance, identifying key predictors like `last_evaluation`, `tenure`, `number_project`, and `salary_low`.
- Insights from EDA and modeling informed actionable HR strategies to reduce attrition.

---

## License
This project is licensed under the MIT License. The dataset used (`HR_dataset.csv`) is sourced from Kaggle and adheres to their terms of use.
