# PACE STRATEGY DOCUMENT
## PROJECT: EMPLOYEE TURNOVER PREDICTION - SAILFORT MOTORS

# PLAN

---

### 1. Business Context
Sailfort Motors is experiencing high employee turnover, which is causing financial burdens in terms of recruitment, training, and development expenses. Apart from the financial burden, high turnover is also causing disruptions in the organization's productivity and teamwork.

Management requires a predictive insight into the factors that contribute to employee turnover and whether the risk of employee turnover can be forecasted early enough to take corrective measures. 

### 2. Strategic Objective
To develop a predictive classification model that:
- Forecasts employees at risk of turnover
- Estimates the most important factors contributing to turnover
- Enables proactive employee retention initiatives

The bigger picture: Transition from reactive recruitment to proactive workforce planning.

### 3. Key Business Questions
1. What are the most important factors in the workplace that contribute to employee turnover? 
2. Is workload (projects, hours) a determinant of employee turnover? 
3. To what extent does employee satisfaction matter? 
4. Are specific departments or job categories at higher risk?
5. Can the risk of employee turnover be forecasted with reasonable accuracy? 

### 4. Data Scope & Working Assumptions
The data set contains employee-level variables such as job, department, workload variables, performance measures, satisfaction levels, tenure, salary level, and employee turnover (target variable).

Hypotheses to be tested:
1. Overworked employees are at a higher risk of leaving the organization
2. Low satisfaction is a strong predictor of employee turnover
3. Compensation level affects employee retention
4. Employee turnover risk may be concentrated in certain departments

These hypotheses will be tested using exploratory analysis and modeling

### 5. Resources and Tools
- Python (Pandas, NumPy)
- Scikit-learn (Logistic Regression, Decision Tree, Random Forest)
- XGBoost
- Data visualization libraries (Matplotlib / Seaborn)

### 6. Risk and Ethical Issues
- The model **should not** be employed to punish employees who are predicted to be "high risk".
- Sensitive variables should be treated with caution to prevent bias.
- Finding should inform retention-oriented strategies, not automated personal decision.

---

# ANALYZE

---

### 1. Data Understanding and Exploration
The initial analysis involved checking the quality of the data and looking for patterns in the turnover data.
Steps involved:
- Checked for missing or inconsistent data
- Checked the class balance of the turnover feature
- Checked the distributions of workload, satisfaction, tenure, and compensation
- Checked correlations between features and attrition.

Descriptive statistics were employed to check for unusual averages or values. Data visualization tools (histograms, box plots, bar charts) were used to ch eck for patterns in the data across departments and roles.

### 2. The main aims of EDA
1. To confirm of reject the initial hypotheses
2. To check for potential multicollinearity
3. To determine which variables are good predictors
4. To check if class imbalance was a problem that needed to be addressed

The ethical check at this stage ensured that no sensitive attribute was being used inappropriately to make decisions.

---

# CONSTRUCT

---

### Model Development
Features identified through EDA were employed to develop classification models.

Approach:
- Split data into training and testing sets (80/20 split, stratified if necessary)
- Encode features for categorical variables
- Develop baseline model: Logistic Regression
- Develop machine learning models: Decision Tree, Random Forest (and XGBoost, if used)

Model Evaluation criteria:
- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC

Particular emphasis was given to the recall value for employees who left, since not being able to detect at-risk employees would decrease business value.

---

# EXECUTE

---

### Insights and Business Recommendations
The evaluation of the model revealed the most important predictors of employee turnover, including workload intensity, satisfaction levels, and tenure patterns.

**Key Findings:**
- Identified high-risk employee groups
- Estimated the relative weights of key drivers
- Evaluated the model's reliability and limitations

Recommendations:
- Track employees with high workload intensity and low satisfaction
- Re-evaluate project assignment processes
- Enhance engagement initiatives in high-risk departments
- Apply predictive knowledge to retention efforts, not punishment

Limitations & Future Directions:
- Model accuracy relies on survey data quality
- Additional information (engagement trends, manager feedback, exit interviews) could enhance predictions
- Periodic retraining would be necessary for long-term use
