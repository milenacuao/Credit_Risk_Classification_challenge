# Credit_Risk_Classification_challenge
![image](https://github.com/milenacuao/Credit_Risk_Classification_challenge/assets/151895571/88cd8c1f-abe6-46e6-b999-a032dc85a0d6)

In this Challenge, you’ll use various techniques to train and evaluate a model based on loan risk. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

OVERVIEW OF THE ANALYSIS

The primary objective of this analysis is to train and evaluate machine learning models for predicting loan risk. By utilizing a dataset comprising historical lending activities from a peer-to-peer lending service, the analysis seeks to develop a model capable of assessing borrower creditworthiness and accurately classifying credit risk.

The key financial metric in the dataset is the loan status, which serves as the target variable for prediction. The features utilized to predict the loan status include:

Loan Size: The principal amount of money borrowed. Interest Rate: The percentage of interest charged on the loan amount. Borrower Income: The annual income of the borrower. Debt-to-Income Ratio: The ratio of the borrower's total monthly debt payments to their monthly gross income. Number of Accounts: The total number of credit accounts held by the borrower. Derogatory Marks: Records of any negative credit events, such as defaults or late payments. Total Debt: The aggregate amount of debt owed by the borrower. These features are critical in building a robust predictive model, as they collectively provide a comprehensive view of the borrower's financial health and repayment capacity.

The machine learning process undertaken in this analysis comprises several key stages, designed to develop, train, and evaluate the predictive model effectively

Creation of Label Sets and Feature DataFrame: Extract the target variable (loan status) and relevant features (such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt) from the provided dataset. Construct a DataFrame for the features and a corresponding label set for the target variable.

Data Splitting:Divide the dataset into training and testing subsets using the train_test_split method. This ensures that the model can be trained on one portion of the data and evaluated on a separate, unseen portion to assess its generalizability.

Model Development:Develop a logistic regression model as the initial approach. Model Training:it the logistic regression model to the training data. Prediction Generation:se the fitted model to make predictions on the testing dataset. This involves applying the model to the testing feature data to predict the loan status labels Model Evaluation: Evaluate the performance of the model using several metrics: Accuracy Score,Confusion Matrix,Classification Report.

The primary objective of these methodological steps was to evaluate and compare the performance of the logistic regression models under different data conditions. Specifically, one model was trained on the original dataset, This aimed to assess the effectiveness of enhancing the model's predictive capabilities for loan risk classification. This systematic approach ensures a thorough and rigorous development and evaluation of the machine learning model, aiming to achieve high accuracy and reliability in predicting loan risk based on historical lending data.

RESULTS

<img width="579" alt="image" src="https://github.com/milenacuao/Credit_Risk_Classification_challenge/assets/151895571/c61fea4d-ea5f-4600-adfe-9436e50ecf88">

The performance of the Logistic Regression model trained on the original dataset demonstrates commendable predictive capabilities for both healthy and high-risk loans. This is evidenced by the high overall accuracy score of 99.18% and a balanced accuracy score of 95.20%.

Healthy Loans, the precision score for healthy loans is 100%, indicating that every prediction made for healthy loans was correct. This high precision is a direct consequence of the predominance of healthy loan instances in the dataset. in the other hand High-Risk Loans, the precision score for high-risk loans is 85%. This suggests that while the model is generally accurate, there is still a significant proportion of false positives in the high-risk loan predictions. This discrepancy underscores the impact of class imbalance on the model's ability to predict the minority class accurately.

The recall score for healthy loans is 99%, meaning that nearly all actual healthy loans were correctly identified by the model. This high recall reflects the model's effectiveness in capturing the majority class.High-Risk Loans,is 91%, indicating that the model correctly identified 91% of the actual high-risk loans. This relatively high recall demonstrates the model's competency in recognizing high-risk loans despite the class imbalance.

These insights are crucial for understanding the limitations and potential areas for improvement in the model.

SUMMARY

Based on the comprehensive analysis, it is recommended to employ this logistic regression model for predicting the creditworthiness of borrowers. The model demonstrates a high predictive accuracy, exceeding 95% in determining the repayment outcome of loans. This exceptional accuracy can be strategically integrated into a business risk profile to optimize financial operations.
