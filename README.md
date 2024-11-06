# ADD-Health-Depression-ML-Model
Machine learning model analyzing the 8-year depression trends in the Add Health study. This project cleans, processes, and models demographic, biometric, and mental health data to predict changes in depression levels using feature engineering, PCA and stochastic decent early stopping regression for optimized performance.

# ADD Health Depression ML Model (8-Years)
This repository contains a machine learning model analyzing data from the Add Health Study, focusing on predicting depression trends over an 8-year span from Wave 4 to Wave 5 using a variety of demographic, biometric, and mental health indicators.

# Dataset
Data was sourced from the ICPSR Add Health Public-Use Dataset. This study follows participants through different waves, collecting detailed information on various aspects. I used Wave IV and Wave V data. Specifically from DS0022, DS0028, DS0029, DS0030, DS0032
See ModelCode document for specific variables used.

# Main Sections
1.	Data Loading and Cleaning
Reads multiple .tsv files and cleans the dataset to handle missing values, reverse codes specific variables, and merges the data into a unified DataFrame.
2.	Feature Engineering
Transforms and creates relevant features based on Wave IV and Wave V mental health scores.
Encodes categorical variables and handles missing data.
3.	Model Preparation
Splits the dataset into training, validation, and test sets.
Applies preprocessing steps such as one-hot encoding, power transformation, and feature scaling.
4.	Dimensionality Reduction with PCA
Reduces the feature set to retain 95% of variance for efficient model training.
5.	Modeling with Manual Search and Early Stopping
Implements an SGDRegressor to predict depression levels in Wave V with early stopping for optimal training.
6.	Model Evaluation
Assesses the model's performance using RMSE and R2 score on the test set.
# Files
Project_Final_Troy.ipynb: Jupyter notebook containing all code for data processing, model training, and evaluation.
merged_df.tsv: Cleaned and preprocessed dataset for analysis.
parametersearch2.csv: Stores results of parameter search during model optimization.
# Dependencies
To run this project, install the necessary Python packages
# Key Packages
pandas and numpy for data manipulation
scikit-learn for machine learning models and preprocessing
matplotlib for data visualization
# Results
See ML_Final_Project_Report_Troy document for discussion of results
# License
This project is licensed under the MIT License. See the LICENSE file for more details.

