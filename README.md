1. Project Title
Employee Retention & Attrition Prediction at Salifort Motors Using Tree-Based Machine Learning Models (Decision Tree & Random Forest)
2. Project Overview
This project addresses employee turnover at Salifort Motors by developing machine learning models to predict whether an employee will leave the company (left) and identify the primary drivers behind attrition. Following exploratory data analysis and feature engineering (including an overworked indicator), both Decision Tree and Random Forest classifiers were built and evaluated. Random Forest outperformed the single Decision Tree model, revealing that workload (number_project, overworked), performance evaluations (last_evaluation), and length of service (tenure) are the strongest predictors of employee departure.
3. Business Understanding
 * Business Problem: Salifort Motors experiences high employee turnover and needs to answer a critical organizational question: "What is likely to make an employee leave the company?"
 * Business Impact: Accurately predicting employee attrition enables the Human Resources (HR) department to identify at-risk employees early, uncover systemic workplace issues, and implement targeted retention policies to reduce hiring and onboarding costs.
 * Analytical Approach: Because the target variable (left) is binary/categorical, supervised classification models (Logistic Regression and tree-based ensemble methods) were selected to balance predictive performance with clear feature interpretability.
4. Data Understanding
 * Dataset & Variables: The HR dataset captures employee work metrics, satisfaction, evaluation scores, tenure, salary tiers (salary_low, salary_medium, salary_high), work accidents (work_accident), and department assignments (sales, technical, support, accounting, marketing) .
 * Feature Engineering & Key Drivers: Created an engineered binary feature (overworked) to capture employees working excessive monthly hours (200+ hours/month). Exploratory analysis and feature importance plots confirmed that attrition is heavily driven by workload burnout and tenure milestones rather than department or salary alone.
5. Modeling and Evaluation
 * Models Built: Constructed and compared Decision Tree and Random Forest classifiers to predict employee attrition (left).
 * Model Comparison & Champion Selection: The Random Forest model slightly outperformed the Decision Tree model across evaluation metrics.
 * Feature Importance Findings:
   * Decision Tree Top Predictors: number_project (~0.38), last_evaluation (~0.35), tenure (~0.17), and overworked (~0.09).
   * Random Forest Top Predictors: last_evaluation (~0.35), number_project (~0.32), tenure (~0.20), and overworked (~0.09), followed by secondary factors like work_accident and salary_low.
6. Conclusion
 * Key Takeaway: Employee attrition at Salifort Motors is primarily driven by overwork and burnout—specifically employees handling too many projects, working 200+ hours per month, or reaching the four-year tenure mark without advancement.
 * Actionable HR Recommendations:
   * Cap Project Workloads: Set a strict upper limit on the number of concurrent projects assigned to an employee.
   * Address Four-Year Tenure Attrition: Promote employees who have been with the company for at least four years, or conduct targeted surveys to understand dissatisfaction at the four-year mark.
   * Reform Overtime & Compensation Policies: Either reward employees proportionately for working longer hours or eliminate expectations of unpaid overtime, ensuring overtime pay and time-off policies are clearly communicated.
   * Decouple Evaluations from Overwork: Stop reserving high evaluation scores exclusively for employees working 200+ hours per month; implement a fair, proportionate reward scale for effort and output.
   * Improve Work Culture: Hold company-wide and team-level discussions to address burnout and establish healthier workload norms.
