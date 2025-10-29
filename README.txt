Objective: Predict whether a client will default on their credit card payment next month.

# Credit Default Prediction

## Objective
The primary goal of this project is to build a robust predictive model to assess the credit risk of clients, specifically predicting whether a client will **default on their credit card payment next month** based on their historical payment and financial behavior.

## Dataset
The project utilized the **Default of Credit Card Clients** dataset from the UCI Machine Learning Repository. This dataset contains 30,000 customer records, including demographic data, credit limits, bill statements, and payment history over six months.

## Tools and Libraries
- **Python** (Pandas, NumPy) for data manipulation and cleaning.
- **Scikit-learn** for machine learning modeling (Logistic Regression, Random Forest).
- **Matplotlib/Seaborn** for Exploratory Data Analysis (EDA).
- **Tableau** (Assumed) for dashboard creation and visualization of key insights.

## Key Results and Performance

| Model | AUC Score | Notes |
| :--- | :--- | :--- |
| **Logistic Regression (Baseline)** | 0.7028 | Established the initial performance benchmark. |
| **Random Forest Classifier (Final)** | **0.7755** | Achieved a significant improvement over the baseline, demonstrating superior discriminatory power. |

### Core Insights
1.  **Class Imbalance:** The dataset exhibits a strong class imbalance, with only **22.12%** of clients defaulting.
2.  **Most Important Feature:** The single most predictive factor for default was **`late_payments`** (the count of months with payment delays), which was created during the Feature Engineering phase. This highlights the critical importance of recent payment behavior over static variables like credit limit or age.
3.  **Model Improvement:** The non-linear **Random Forest** model was essential for capturing complex interactions between variables, resulting in the higher AUC.

## Feature Engineering Highlights
Three powerful features were engineered to enhance model performance:
* **`late_payments`**: The count of positive payment statuses (`PAY_x > 0`).
* **`utilization`**: The ratio of the latest bill amount to the credit limit.
* **`avg_payment_ratio`**: The proportion of the bill paid off on average.

## Visualization
[Link to Tableau Dashboard Here] 
*Note: This link should point to your finalized Tableau Public dashboard showcasing Default Rate by Age Group and the Feature Importance chart.*

---

**¡Has completado el plan de 7 días!** Tienes un proyecto de Ciencia de Datos sólido, reproducible y profesionalmente documentado. ¡Felicidades por tu esfuerzo!