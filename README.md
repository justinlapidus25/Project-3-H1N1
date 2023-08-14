# Project-3-H1N1
Data Preparation
The code starts by reading data from CSV files and performing data preprocessing steps such as dropping null values and irrelevant columns. It then splits the data into feature matrix X and target vector y, followed by splitting into training and testing sets.

Pipelines
Two pipelines are defined, one for Logistic Regression with Bagging and another for Decision Tree Classifier with Bagging. Both pipelines include preprocessing steps such as one-hot encoding and scaling, as well as oversampling using SMOTE to address class imbalance.

Model Evaluation
The code uses GridSearchCV to perform hyperparameter tuning for both pipeline models. Confusion matrices, ROC curves, and AUC scores are generated for model evaluation.

Feature Importance
The feature importance of the models is also analyzed using Decision Tree and Random Forest classifiers. The important features that contribute to predicting H1N1 vaccine uptake are identified and visualized.

Conclusion
This repository demonstrates the process of predicting H1N1 vaccine uptake using different machine learning techniques. The models are evaluated and compared based on performance metrics, and important features are identified for making predictions.

Please note that this README provides a high-level overview of the project. For detailed code and implementation, refer to the Jupyter Notebook provided in the repository.
