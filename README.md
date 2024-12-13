Fetal Health Classification Using Machine Learning

Overview
This project focuses on using machine learning to predict fetal well-being, aligning with the UN Sustainable Development Goal (SDG) 3 to reduce child mortality and improve maternal health. The model leverages cardiotocography (CTG) data and advanced machine learning algorithms to classify fetal health into three categories: Normal, Suspect, and Pathological.

By applying the XGBoost algorithm with BorutaSHAP feature selection, the model achieves high accuracy while improving precision and recall for minority classes, making it a robust tool for fetal health assessment.

Key Features
Dataset: Cardiotocography dataset from UCI Machine Learning Repository with 2126 records and 22 attributes.

Machine Learning Models:
Logistic Regression
Random Forest
Gaussian Naive Bayes
Support Vector Classifier (SVC)
XGBoost Classifier (selected as the best model)

Feature Selection: BorutaSHAP algorithm for improved accuracy and interpretability, especially for minority class classification.

Performance:
XGBoost Classifier with BorutaSHAP achieves 94% accuracy.
Balanced F1-scores for all classes, with significant improvements in minority class precision and recall.

Methodology
Exploratory Data Analysis:
Analyzed fetal health features such as fetal heart rate, uterine contractions, and variability metrics.
Identified key correlated features using a correlation heatmap.

Model Development:
Evaluated multiple classification models using cross-validation.
Selected XGBoost for its superior accuracy and generalization.

Feature Selection:
Applied BorutaSHAP to identify critical features like accelerations, prolonged decelerations, and variability metrics.

Evaluation:
Used metrics such as precision, recall, and F1-score to assess model performance.
Improved minority class classification with Boruta-enhanced features.

Results
Accuracy:
XGBoost without BorutaSHAP: 93%
XGBoost with BorutaSHAP: 94%
Performance for Minority Classes:
Class 1: Precision (89%), Recall (72%), F1-score (79%)
Class 2: Precision (86%), Recall (92%), F1-score (89%)
Feature Importance: Key features include accelerations, uterine contractions, and variability metrics, identified using BorutaSHAP.
