🎓 Student Retention Prediction Using Machine Learning
📌 Project Overview

Student retention is a critical challenge faced by educational institutions worldwide. Identifying students at risk of dropping out at an early stage allows institutions to provide timely intervention, academic support, and financial assistance.

This project applies Machine Learning techniques to predict whether a student is likely to drop out using academic, demographic, and socio-economic features.

A Random Forest Classifier is used to build a predictive model capable of identifying at-risk students with high accuracy.

🎯 Project Objective

The primary objective of this project is:

To develop a classification model that predicts student dropout.

To analyze key factors influencing student retention.

To evaluate model performance using standard classification metrics.

To extract actionable insights for institutional decision-making.

📊 Dataset Description

The dataset used in this project contains:

4424 student records

35 features

Academic, demographic, and financial indicators

A target variable indicating student status

Target Variable
Value	Meaning
0	Not Dropout (Graduate / Enrolled)
1	Dropout
🔎 Features Included

The dataset includes:

Marital status

Application mode

Course information

Previous qualification

Nationality

Parents’ qualification & occupation

Tuition fee status

Age at enrollment

Academic performance (1st and 2nd semester)

Economic indicators (GDP, Inflation, Unemployment)

These features collectively help capture student background and performance patterns.

🛠 Technologies Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

🔬 Methodology

The project follows a structured Machine Learning pipeline:

1️⃣ Data Loading & Exploration

Loaded dataset using Pandas

Checked for missing values

Examined feature types

Analyzed class distribution

2️⃣ Exploratory Data Analysis (EDA)

Visualized class imbalance

Generated correlation heatmap

Compared academic performance between dropout and non-dropout students

Analyzed tuition fee payment status

Key Observations

Students with lower academic grades show higher dropout probability.

Failure to complete curricular units strongly correlates with dropout.

Tuition fee irregularities are linked to dropout risk.

3️⃣ Data Preprocessing

Converted target variable into binary format

Separated features (X) and target (y)

Performed train-test split (80% training, 20% testing)

4️⃣ Model Selection

Random Forest was chosen because:

Handles numerical features effectively

Reduces overfitting

Works well with structured/tabular data

Provides feature importance analysis

Requires minimal preprocessing

5️⃣ Model Training

The model was trained using:

200 decision trees

Default depth (None)

Random state for reproducibility

📈 Model Evaluation

Model performance was evaluated using multiple metrics.

🔹 Accuracy

86%

The model correctly classifies 86% of students.

🔹 Confusion Matrix
[[537   32]
 [ 91  225]]


True Negatives: 537

False Positives: 32

False Negatives: 91

True Positives: 225

🔹 Classification Report

For Dropout Class (1):

Precision: 0.88

Recall: 0.71

F1-score: 0.79

The model performs well in identifying at-risk students while maintaining strong overall performance.

🔹 ROC Curve & AUC Score

AUC Score: 0.90

An AUC score above 0.90 indicates excellent separability between dropout and non-dropout students.

🔹 Cross-Validation

5-fold cross-validation average score: ~87%

This demonstrates model stability and low overfitting risk.

🧠 Feature Importance

The most influential features include:

Curricular units 2nd semester (approved)

Curricular units 2nd semester (grade)

Curricular units 1st semester (approved)

Tuition fee status

Age at enrollment

This indicates academic performance and financial stability are the strongest predictors of dropout.

💡 Practical Applications

This model can help institutions:

Identify at-risk students early

Offer academic mentoring

Provide financial counseling

Develop retention strategies

Improve graduation rates

Early prediction allows proactive intervention rather than reactive action.

⚠ Limitations

Dataset may not generalize to all institutions

Limited feature engineering

Hyperparameter tuning not extensively performed

No external dataset validation

🚀 Future Improvements

Hyperparameter tuning using GridSearchCV

Model comparison with XGBoost or Gradient Boosting

Threshold tuning to improve dropout recall

Deployment as a web application

Real-time prediction dashboard

📂 Project Structure
Student_Retention_Project/
│
├── dataset.csv
├── Student_Retention_Notebook.ipynb
├── README.md
└── Report.pdf (optional)

🎓 Conclusion

This project demonstrates the application of Machine Learning in predicting student dropout using structured academic data.

The Random Forest model achieved:

86% Accuracy

0.90 AUC Score

Stable cross-validation performance

The findings confirm that academic performance and financial stability play a major role in student retention.

Machine learning models like this can significantly enhance institutional decision-making and improve student outcomes.
