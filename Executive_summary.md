# EXECUTIVE SUMMARY
## Employee Turnover Prediction - Sailfort Motors

Salifort Motors has been facing a higher-than-desired employee turnover rate, which is increasing the cost of hiring and affecting team stability. The objective of this project was to identify the reasons for the employee turnover and develop a predictive model to enable the HR department to proactively identify employees at risk.

After processing and analyzing data from nearly 12,000 employee records, some key patterns have emerged.

The most important reason for employee turnover is the level of employee satisfaction. Employees who left the company had lower satisfaction levels than those who remained.

Other important reasons are:

- **Tenure (3-5 years)** – Employees in the mid-career phase had higher turnover rates.

- **Higher monthly working hours** – Work intensity is apparently associated with employee turnover.

- **Number of projects** – Employees with heavier project loads had higher turnover rates.

- **Low salary levels** – Employees in the lowest salary group had the highest turnover rate (approximately 20%).

- **No promotion** – Employees who were promoted had significantly lower turnover rates.

To provide concrete results, three models were developed:

1. Logistic Regression (baseline model)
2. Random Forest
3. XGBoost

The XGBoost model gave the best results, achieving:
- **98% accuracy**
- **93% recall for employees who left**
- **0.98 ROC-AUC**

This means that the model is extremely effective at pinpointing the employees who are at risk of leaving – which is essential because failing to identify and retain at-risk employees is more expensive than having one additional retention conversation.

--- 

**Key Business Takeaways**
1. Satisfaction is more than a “soft metric” – it is the best available predictor of employee turnover.
2. Employees in the 3-5 year range may need targeted engagement or career development support.
3. Too much work is likely a burnout driver.
4. Promotion and compensation practices are a highly effective retention tool.
5. Department is not a significant determinant of employee turnover – individual-level variables are much more important.

---

**Recommendation**

This predictive model should be implemented as an early warning system for HR departments. Rather than waiting for employees to quit and then acting, the company can take proactive steps to support employees who are at risk based on predictive patterns.

This model should not be used as a punitive measure but rather as a guide for targeted retention conversations and improving workplace satisfaction.

---

If implemented correctly, this approach can lead to a reduction in turnover, lower recruitment costs, and a more stable and satisfied workforce.