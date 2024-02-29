# credit-risk-classification
module 20 challenge 


Analysis Overview:
The analysis aims to employ various techniques for training and evaluating a model focused on loan risk using machine learning. Leveraging a dataset from a peer-to-peer lending services company, historical lending activity features like loan size, interest rate, borrower income, and others are utilized to build a model identifying creditworthiness. The goal is to predict loan status as either a Healthy Loan (0) or a High-Risk Loan (1), employing the Logistic Regression Algorithm due to its suitability for classification problems.

Machine Learning Process Stages:

Data Split:
The dataset is divided into training and testing sets to assess the model's performance.

Model Training:

Logistic Regression Model Initialization: Constructed using the original dataset with 75,036 low-risk and 2,500 high-risk data points.
Model Fitting: Utilized training data to fit the model, adjusting weights during training to minimize logistic loss.
Resampling with RandomOverSampler:
To address class imbalance, RandomOverSampler resampling is applied, ensuring equal representation of low and high-risk labels. After resampling, both classes consist of 56,277 data points each.

Logistic Regression Model with Resampled Data:
A logistic regression model is built using the resampled data to predict loan risk.

Model Evaluation:
Employed the validation set to evaluate model performance, using metrics like accuracy, precision, recall, and F1-score.

Results:

Machine Learning Model 1:

Healthy Loans (0): Precision and recall are both 1.00, indicating accurate predictions for this label.
High-Risk Loan (1): Precision is 0.87, and recall is 0.89, demonstrating high accuracy in predicting high-risk loans.
Overall accuracy: 0.99.
Machine Learning Model 2:

Precision: 87%, Recall: 89%, showcasing effective identification of high-risk loans with minimal false positives.
Overall accuracy: 0.99.
Summary:
Both models exhibit commendable accuracy, precision, and recall. However, the logistic regression model with resampling slightly outperforms, achieving an accuracy of 0.9945 compared to 0.9924 for the initial model. Considering the objective of accurately identifying healthy and high-risk loans, the logistic regression model with resampling is deemed the optimal choice.
