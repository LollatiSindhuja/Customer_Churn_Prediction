# Customer_Churn_Prediction
This project develops an end-to-end customer churn prediction system using supervised machine learning on the IBM Telco Customer Churn dataset. The system aims to accurately predict whether customers are likely to churn, enabling proactive retention strategies. 

Project Overview:
This project focuses on building a predictive model to identify customers likely to "churn" (cancel their service) in the telecom industry. By leveraging historical usage patterns and demographic data, the system enables companies to implement proactive retention strategies, which is significantly more cost-effective than acquiring new customers.

Dataset Profile:
The project utilizes the IBM Telco Customer Churn Dataset.
• Size: 7,043 customers with 21 features.
• Target Variable: Churn (Yes/No).
• Key Features: Tenure, Monthly Charges, Contract Type, Payment Method, and Internet Service type.
• Churn Rate: 26.5% of the total customer base.

Tech Stack:
• Programming Language: Python 3.9
• Environment: Jupyter Notebook (Anaconda Distribution)
• Libraries:
    ◦ Data Handling: Pandas, Numpy
    ◦ Visualisation: Matplotlib, Seaborn
    ◦ Machine Learning: Scikit-learn (Logistic Regression, Random Forest, SMOTE)

Methodology:
The project follows a comprehensive machine learning pipeline:
1. Data Cleaning: Handled 11 missing values in TotalCharges and converted data types.
2. Exploratory Data Analysis (EDA): Visualised patterns such as how month-to-month contracts correlate with a 42.7% churn rate.
3. Preprocessing: Applied Label Encoding for categorical variables and StandardScaler for numerical features.
4. Model Training: Evaluated Logistic Regression (baseline) and Random Forest (ensemble).
5. Evaluation: Metrics included Accuracy, Precision, Recall, and ROC-AUC.

Performance Results:
Metric            Logistic Regression          Random Forest
Accuracy          0.801 (80.1%)                        0.799 (79.9%)
Precision         0.647                        0.655
ROC-AUC           0.840                        0.837
Recall            0.548                        0.513
F1-Score          0.593                        0.576

Top Predictors:
Tenure, Monthly Charges, and Total Charges were identified as the most significant factors influencing churn.

Key Business Insights:
• Contract Risk: Customers on month-to-month contracts are 4x more likely to churn than those on 2-year contracts.
• Tenure: Customers with less than 12 months of service are at the highest risk.
• Financial Impact: Implementing this model to reduce churn by 15% could result in approximately $240,000 in annual savings.
