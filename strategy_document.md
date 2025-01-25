# Salifort Motors Employee Retention Project: Strategy Document

## Overview
Salifort Motors is experiencing challenges with employee retention and aims to address this by leveraging data-driven insights. This project will analyze historical employee data to identify key factors influencing turnover, predict which employees are most at risk of leaving, and propose actionable strategies to improve retention rates and overall workplace satisfaction.

---

## Objectives
1. **Understand the Problem Context**:
   - Define the business need and explore employee data to identify turnover drivers.
   - Establish alignment between project goals and HR strategies.
2. **Perform Exploratory Data Analysis (EDA)**:
   - Investigate variables such as evaluation scores, tenure, workload, and salary levels.
   - Detect and handle missing or anomalous data.
   - Use visualizations to highlight key trends and relationships.
3. **Build and Validate Predictive Models**:
   - Use machine learning techniques, including logistic regression and random forest, to model employee attrition.
   - Evaluate model performance and refine based on validation metrics.
4. **Derive Insights and Propose Actions**:
   - Provide HR with clear, data-backed recommendations to improve employee retention policies.

---

## Project Phases and Detailed Tasks

### **1. Plan**
- **Understand the Problem**:
  - Key Question: *What factors most significantly influence employees to leave Salifort Motors?*
  - Audience: HR leadership, company executives, and department managers.
  - Anticipated Impact:
    - Reduce turnover rates.
    - Improve employee satisfaction and engagement.
    - Enhance workforce planning and policy development.
- **Identify Resources**:
  - Historical employee dataset, including variables such as:
    - `last_evaluation`, `tenure`, `number_project`, `salary_low`, `overworked`, and `work_accident`.
  - Tools: Python, visualization libraries (Matplotlib, Seaborn), machine learning frameworks (Scikit-learn).
- **Deliverables**:
  - Cleaned and structured dataset.
  - Insights from EDA and visualizations.
  - Predictive models and their evaluation.
  - Final report with recommendations for stakeholders.

---

### **2. Analyze**
- **Perform EDA**:
  - Examine the dataset for missing values, anomalies, and variable distributions.
  - Key Columns of Interest:
    - `last_evaluation`: Performance scores.
    - `number_project`: Workload indicators.
    - `tenure`: Employee duration at the company.
    - `salary_low`: Compensation levels.
    - `overworked`: Workload status.
  - Key Questions:
    - Which variables correlate most strongly with employee turnover (`left`)?
    - Are there any patterns based on tenure or evaluation scores?
  - Visualizations:
    - Bar plots to examine categorical variables.
    - Correlation heatmaps to identify variable relationships.
    - Box plots to explore the impact of numerical variables on `left`.
- **Address Data Issues**:
  - Handle missing or inconsistent data.
  - Ensure standardization across all formats and units.
  - Consider potential sampling biases.
- **Ethical Considerations**:
  - Avoid reinforcing biases in predictions (e.g., salary or demographic factors).
  - Maintain confidentiality of sensitive employee data.

---

### **3. Construct**
- **Model Building**:
  - Chosen Models:
    - Logistic Regression:
      - Simplicity and interpretability for binary classification.
    - Random Forest:
      - Robustness in handling complex, non-linear relationships.
  - Key Metrics:
    - Accuracy, precision, recall, F1 score, and AUC.
    - Feature importance rankings to identify key predictors.
- **Model Assumptions**:
  - Logistic Regression:
    - Check for multicollinearity among predictors.
  - Random Forest:
    - Ensure sufficient data depth and balanced representation of classes.
- **Validation**:
  - Split data into training and testing sets (e.g., 70/30 split).
  - Use cross-validation to ensure generalizability.

---

### **4. Execute**
- **Insights from Models**:
  - Most impactful variables:
    - `last_evaluation`, `tenure`, `number_project`, `overworked`, `salary_low`, and `work_accident`.
  - Random forest slightly outperformed logistic regression in predictive accuracy.
- **Recommendations**:
  - *Workload Management*: Cap the number of projects assigned to employees to prevent burnout.
  - *Tenure Support*: Investigate and address dissatisfaction among employees with four years of tenure.
  - *Reward Systems*: Align performance evaluation and rewards to realistic and achievable workloads.
  - *Work Culture Improvements*: Enhance communication on overtime pay policies, expectations around workload, and time-off policies.
  - *Performance Incentives*: Create proportionate rewards for employees contributing extra effort.
- **Delivery to Stakeholders**:
  - Present findings using visualizations tailored to HR and executive audiences.
  - Include actionable steps with clear links to model insights.

---

## Success Metrics
- Reduced annual employee turnover rates.
- Improved employee engagement and satisfaction scores.
- Streamlined HR interventions aligned with data-driven predictions.
- Higher overall organizational productivity and morale.
