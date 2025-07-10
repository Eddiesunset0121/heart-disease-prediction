# Project 3. Heart Disease  Prediction: A Logistic Regression Analysis

:large_blue_diamond: Project Objective 
 - This project analyzes the UCI Heart Disease dataset to identify the key factors that influence the presence of heart disease. The goal is to build an accurate and interpretable classification model that can predict a person's likelihood of having heart disease based on their clinical and demographic attributes.

:star2: Key Skills & Tools 
- Data Manipulation & Analysis: Pandas, NumPy

- Data Visualization: Matplotlib, Seaborn

- Machine Learning: Scikit-learn (Train-Test Split, Pipeline, ColumnTransformer, StandardScaler, OneHotEncoder, LogisticRegression)

- Model Evaluation: Scikit-learn Metrics (Confusion Matrix, ROC/AUC Curve, Classification Report)

- Core Competencies: Exploratory Data Analysis (EDA), Outlier Analysis, Predictive Modeling, Model Performance Evaluation.

:herb: Analysis & Key Findings 	
 - The analysis involved a comprehensive EDA to understand the relationships between variables, followed by the development and evaluation of a predictive logistic regression model.

:herb: Exploratory Data Analysis & Feature Insights: 
 - Outlier Investigation: Outlier analysis was performed using the IQR method and boxplots. The outliers identified in features like trestbps (resting blood pressure) and chol (cholesterol) were retained, as they were determined to represent legitimate, albeit extreme, clinical measurements crucial for an accurate model rather than data entry errors.

:herb: Key Categorical Predictors: A detailed analysis using count plots revealed several strong predictors for heart disease: 

- ST Slope (slope): Patients with a flat (1) or downsloping (2) ST segment during exercise have a significantly higher incidence of heart disease.

- Exercise-Induced Angina (exang): The presence of angina induced by exercise is a strong indicator of heart disease.

- Number of Blocked Vessels (ca): The probability of heart disease increases sharply as the number of major vessels blocked by fluoroscopy rises from 0 to 3.

- Thalassemia Type (thal): A "fixed defect" or "reversible defect" in blood flow is strongly associated with a positive diagnosis.

:herb: Predictive Model Development & Performance: 
 - Preprocessing Pipeline: A scikit-learn Pipeline was constructed to streamline the workflow. Numerical features were standardized using StandardScaler, and categorical features were transformed using OneHotEncoder to prepare the data for the model.

 - Logistic Regression Model: A logistic regression model was trained on the preprocessed data, achieving an overall accuracy of 84% on the unseen test set.

:herb: Model Evaluation: 	

- AUC Score: The model demonstrated excellent discriminative ability with an Area Under the ROC Curve (AUC) of 0.92.

- Classification Report: The model showed a strong and balanced performance for predicting the "Has Heart Disease" class, with a Precision of 0.84, a Recall of 0.84, and an F1-Score of 0.84.

- Confusion Matrix Insights: The model correctly identified 27 out of 32 patients with heart disease (True Positives) and 24 out of 29 patients without heart disease (True Negatives). The model made 5 False Negative predictions, which is the most critical metric to monitor and improve upon in a medical diagnostic context.

:bulb: Application & Conclusion 
- This logistic regression model serves as a reliable and interpretable tool for identifying individuals at high risk for heart disease.

- Clinical Decision Support: The model can be used in a clinical setting to assist healthcare professionals by providing a data-driven probability of disease, helping to prioritize patients for further, more invasive testing.

- Risk Factor Quantification: By highlighting the importance of factors like ST slope and exercise-induced angina, the model reinforces their diagnostic value and can be used to better educate patients on key health indicators and preventative measures.
