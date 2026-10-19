🩺 DIABETES RISK PREDICTION USING MACHINE LEARNING (BINARY CLASSIFICATION)

Hello! This project focuses on analyzing clinical variables associated with diabetes and building a predictive model capable of forecasting its presence based on patients' medical information.

🎯 PROJECT OVERVIEW AND HYPOTHESIS

The core objective of this study was to examine key clinical risk factors and assist healthcare analytics by automating early detection. 

During the Exploratory Data Analysis (EDA), variables such as Glucose, BMI, and Age showed a clear positive correlation with the presence of diabetes. The correlation matrix confirmed that Glucose is the variable most strongly associated with the target outcome, fully supporting the initial hypothesis of the project.

🛠️ DATA PREPROCESSING AND CLEANING

A critical step in this project was handling clinical inconsistencies:

Missing Value Imputation: Biological variables containing values equal to zero (which is clinically impossible, such as a blood pressure or BMI of 0) were identified as missing data.

Strategy: These values were treated and successfully imputed using the median of each respective variable to preserve data integrity before feeding the model.

📊 TECH STACK AND METHODOLOGY

Language: Python

Libraries: Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn

Model Implemented: Logistic Regression

📈 PERFORMANCE AND RESULTS

The Logistic Regression model was evaluated using a test set of 154 patients, yielding an overall Accuracy of 71% (correctly classifying approximately 7 out of 10 observations). 

Classification Metrics Breakdown:

Class 0 (Non-Diabetes): Strong predictive power with 75% Precision and 82% Recall (82 out of 100 healthy patients correctly identified).

Class 1 (Diabetes): Achieved 60% Precision and 50% Recall. The model successfully captures patterns related to the disease, though its capacity to detect positive instances remains moderate, identifying half of the positive cases in the test set.

Confusion Matrix:
[[82 18]
 [27 27]]

82 True Negatives: Healthy patients correctly identified.

27 True Positives: High-risk patients correctly flagged.

27 False Negatives: Patients with diabetes who were missed by the model.

🚀 FUTURE WORK AND OPTIMIZATION

As part of future iterations, more complex algorithms (such as Random Forest, XGBoost, or Support Vector Machines) will be evaluated alongside hyperparameter tuning. The main goal of future updates will be to improve predictive performance, specifically boosting the Recall (sensitivity) for the positive class to minimize critical false negatives in diagnostic screening.

📂 REPOSITORY STRUCTURE

pima_diabetes_prediction.ipynb: Jupyter Notebook containing the end-to-end pipeline (EDA, preprocessing, modeling, and evaluation).


