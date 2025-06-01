# Redi_Machine_Learning_Project

### Notebook Workflow Summary
The script begins by setting up the Python environment and importing necessary libraries. It then loads the training, test, and sample submission datasets. Exploratory data analysis is performed to understand the data's characteristics. Data preprocessing steps, including imputation, scaling, and encoding, are applied using sklearn pipelines. The PyCaret library is then used to efficiently train, compare, and select the best-performing classification model. The chosen model is evaluated using various metrics and visualisations. Finally, the model makes predictions on the official test set, the model is saved, and a submission file is generated in the required format.

## Diabetes Prediction Model

This machine learning project focuses on developing a model to predict the likelihood of a patient having a specific type of diabetes based on various health-related features. The model is trained on a dataset of women's health metrics.

### Rationale for the Project

This project was developed to create a predictive model for the "SheCures" challenge/contest to identify diabetes types from health data. It is a practical application of machine learning techniques for a healthcare-related problem.

### Requirements of the Diabetes Prediction Model

The primary goal is to build a script that processes health data, trains a machine learning model, and predicts diabetes types. The input data is provided in CSV files.

### Specific requirements of the model development process:

#### Load and Inspect Data:

* Read training data (Train.csv), test data (Test.csv), and a sample submission format (SampleSubmission.csv).
  
* Understand data structure, types, missing values, and basic statistics.
  
* Visualise feature correlations.

#### Preprocess Data:

* Identify numerical and categorical features.
* Create and apply preprocessing pipelines:
  * Impute missing numerical values (e.g., using KNNImputer).
  * Scale numerical features (e.g., using MinMaxScaler).
  * Encode categorical features (e.g., using OneHotEncoder).
* Split data into training and testing sets before certain preprocessing steps to prevent data leakage.

### Train and Select Model:
* Utilise PyCaret to set up the ML environment and compare various classification models.
* Choose and train a specific model based on performance metrics (e.g., Random Forest based on F1-score).
  
### Evaluate Model Performance:
* Assess the chosen model using metrics like accuracy, precision, recall, and F1-score (via classification_report).
* Visualise performance using a confusion matrix and feature importance plots.

### Generate Predictions:
* Use the trained model to predict diabetes types on the unseen test data.
  
### Save Model and Submission:
* Save the finalised trained model for deployment.
* Create a submission CSV file in the specified format containing predictions for the test data.
