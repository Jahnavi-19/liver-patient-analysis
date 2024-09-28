# Liver Patient Analysis
# Project Overview:
This project addresses the critical challenge of predicting liver disease in patients by applying machine learning algorithms to a dataset of patient records. The goal is to improve early diagnosis and reduce the burden on medical professionals, especially in regions with limited healthcare access. Using supervised learning techniques, this project aims to provide an accurate classification model that can predict whether a patient is at risk of liver disease based on specific health indicators.
# Objectives:
The primary goal of the project is to build a classification model that can predict liver disease in patients, using features such as bilirubin levels, enzyme counts, and protein levels from a dataset of 584 Indian patients. The project also focuses on:
* Reducing the time and costs associated with delayed diagnosis.
*  Exploring and selecting the most effective machine learning algorithms for this problem.
*  Using performance metrics such as F-beta score and Receiver Operating Characteristics (ROC) curve to assess model performance.
# Problem Statement:
Given a dataset of patient records, the task is to develop a supervised learning model that can classify a patient as either a liver disease patient or a non-liver disease patient. The dataset consists of 416 liver disease patient records and 167 non-liver disease patient records collected from the North East of Andhra Pradesh, India. The aim is to build a predictive model that reduces the back-and-forth diagnosis process between hospitals and laboratories.
# Methodology:
## Data Preparation & Feature Engineering:
The dataset contained numerical and categorical features like Age, Gender, Total Bilirubin, Albumin, and more.
Missing values were handled by cleaning the dataset, and one-hot encoding was used for categorical features like gender.
The dataset was split into training and test sets for model evaluation.
## Machine Learning Algorithms:
Evaluated several supervised learning algorithms, but Logistic Regression provided the best performance in terms of accuracy and F-beta score. The model was trained and fine-tuned using the Grid Search Cross Validation technique to optimize hyperparameters. Here’s a breakdown of the models considered:
* Logistic Regression: Chosen as the primary model due to its suitability for binary classification tasks.
* Other Techniques: Explored methods like Random Forest and SVM (Support Vector Machine), but Logistic Regression proved to be the most effective for this dataset.
## Model Performance Metrics:
* F-beta score: This was used to balance precision and recall for a more nuanced evaluation, especially important in medical diagnostics.
* ROC-AUC: To further assess the classifier’s performance in terms of True Positive Rate (TPR) versus False Positive Rate (FPR).
* Accuracy Achieved: 71.43%, but with plans to improve it by using larger and more diverse datasets.
# Exploratory Data Analysis (EDA):
Various visualization techniques were used to understand the relationships between the features and the target variable (liver disease). Some of the key analyses included:
* Scatter Plot: Between Total Bilirubin and Direct Bilirubin, showing a strong correlation in liver disease patients.
* Count Plot: Depicting the number of patients diagnosed with liver disease versus those who were not.
* Correlation Heatmap: Demonstrating relationships between features like Enzyme Levels and Bilirubin levels to identify key predictors of liver disease.
# Technical Tools and Technologies:
* Machine Learning: Logistic Regression
* Data Visualization: Matplotlib, Seaborn
* Flask, HTML/CSS: For model serialization and reuse
* Joblib: For saving and loading the scaler used for data transformation
