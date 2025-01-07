## Module 12 Report

### Overview of the Analysis

The purpose of this analysis was to evaluate the performance of machine learning models in predicting loan risk. Specifically, we analyzed a dataset containing financial information about loans to determine whether a loan was likely to be healthy (low risk) or high-risk.

The dataset included the following key features:
	•	Loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt.
The target variable, loan_status, was binary:
	•	0 representing a healthy loan and 1 representing a high-risk loan.

The machine learning process involved the following stages:
	1.	Data Preprocessing: We separated the dataset into features (X) and target labels (y), followed by a train-test split to create training and testing datasets.
	2.	Model Selection: Logistic Regression was chosen as the primary algorithm because of its effectiveness in binary classification problems and interpretability.
	3.	Model Training: The logistic regression model was trained using the training dataset.
	4.	Model Evaluation: The model was evaluated on the test dataset using metrics such as accuracy, precision, recall, and balanced accuracy. A confusion matrix and classification report provided additional insights.

## Results

## Logistic Regression Model:

	•	Accuracy: 99%
	•	Precision:
	•	Healthy loans (0): 1.00
	•	High-risk loans (1): 0.84
	•	Recall:
	•	Healthy loans (0): 0.99
	•	High-risk loans (1): 0.94
	•	Balanced Accuracy: 0.952

The confusion matrix revealed:

	•	Healthy loans (0): 18,655 true positives and 110 false negatives.
	•	High-risk loans (1): 583 true positives and 36 false negatives.

## Summary

The logistic regression model demonstrated exceptional performance, achieving high accuracy, precision, and recall. It excelled at predicting healthy loans (0) with near-perfect metrics and performed strongly for high-risk loans (1), albeit with slightly lower precision.

## Recommendation:

This model is recommended for use due to its robust performance on both healthy and high-risk loans. It maintains a balance between identifying high-risk loans accurately and minimizing false positives for healthy loans.

Considerations:

	•	The choice of whether to prioritize precision or recall for high-risk loans depends on business priorities. If minimizing false positives for high-risk loans is critical (e.g., avoiding unnecessary interventions), further improvement in precision for class 1 may be necessary.
	•	If identifying as many high-risk loans as possible is more important, the model’s high recall for 1 is already well-suited for the task.
