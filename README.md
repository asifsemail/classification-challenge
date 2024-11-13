### Author

	•	Name: Asif Khan
	•	Date: November 2024
	•	Module: Module 13 Challenge - Spam Detector

# Spam Detector Project Overview

This project involves building a supervised machine learning model to help an Internet Service Provider (ISP) improve its email filtering system by accurately detecting spam emails. The dataset contains information about emails, with each email classified as either spam or not spam. The goal is to create two classification models (Logistic Regression and Random Forest) to determine which model better detects spam and is more suitable for the ISP’s filtering needs.

## Dataset

The dataset for this project is provided in CSV format and can be found at: shttps://static.bc-edx.com/ai/ail-v-1-0/m13/challenge/spam-data.csv The data includes various features describing emails, and a target variable, spam, which is:
	•	0 for legitimate emails (not spam)
	•	1 for spam emails

## Instructions and Steps

### Step 1: Data Preperation

	•	Read the Data: Load the dataset into a Pandas DataFrame.
	•	Prediction Statement: Before building the models, make an initial prediction as to which model (Logistic Regression or Random Forest) will perform better at classifying spam emails.
	•	Create Labels and Features:
	•	The target variable (y) is created from the spam column.
	•	The feature matrix (X) is created from the remaining columns.
	•	Check Data Balance: Use value_counts() to check the balance of the target variable (y).

### Step 2: Data Splitting

	•	Split the Data: Divide the dataset into training and testing sets using train_test_split.

### Step 3: Feature Scaling

	•	Standardize Features: Use StandardScaler to scale the features in X_train and X_test for better performance with Logistic Regression.

### Step 4: Model Building and Evaluation

	•	Logistic Regression Model:
	•	Train a Logistic Regression model using the scaled training data.
	•	Predict on the test data.
	•	Calculate the accuracy of the Logistic Regression model.
	•	Random Forest Model:
	•	Train a Random Forest model using the scaled training data.
	•	Predict on the test data.
	•	Calculate the accuracy of the Random Forest model.

### Step 5: Model Comparison

	•	Compare Model Performance: Determine which model performed better in detecting spam based on the accuracy scores of both models.
	•	Compare with Initial Prediction: Reflect on how the actual results compare with the initial prediction of which model would perform better.

## Requirements

The project requires the following libraries:
	•	pandas: For data manipulation and analysis.
	•	scikit-learn: For data preprocessing, model building, and evaluation.

## Usage

	1.	Clone this repository and navigate to the project directory.
	2.	Open the spam_detector.ipynb Jupyter Notebook.
	3.	Follow the cells in the notebook to:
	•	Load and preprocess the data.
	•	Split and scale the data.
	•	Train and evaluate the Logistic Regression and Random Forest models.
	•	Compare model accuracy and answer the evaluation questions.


## Key Insights and Questions Answered

	•	Logistic Regression is typically effective for linear data relationships, while Random Forest can handle complex, non-linear relationships.
	•	Scaling is essential for algorithms that rely on distance calculations (e.g., Logistic Regression).
	•	Random Forest is often robust and may perform better with larger datasets due to its ensemble nature.

