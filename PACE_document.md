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