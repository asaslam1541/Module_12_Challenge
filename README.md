# Credit Risk Analysis Report

**Overview:**

The purpose of this analysis is to assess the performance of two machine learning models in predicting credit risk using a dataset of historical lending activity from a peer-to-peer lending services company. The dataset is imbalanced, with a majority of healthy loans (label 0) and a minority of high-risk loans (label 1). We will compare the results of a logistic regression model trained on the original data and a logistic regression model trained on resampled data using RandomOverSampler.

**Results:**

*Logistic Regression Model with Original Data:*
- Balanced Accuracy Score: 0.9218
- Precision (High-Risk Loan - Label 1): 0.91
- Recall (High-Risk Loan - Label 1): 0.85

*Logistic Regression Model with Resampled Data:*
- Balanced Accuracy Score: 0.9128
- Precision (High-Risk Loan - Label 1): 0.91
- Recall (High-Risk Loan - Label 1): 0.83

**Summary:**

Both machine learning models performed well in predicting credit risk, but there are key differences between them.

*Logistic Regression Model with Original Data:*
- The model achieved a high balanced accuracy score of 0.9218, indicating strong overall performance.
- Precision for high-risk loans (label 1) is 0.91, meaning that when the model predicts a loan as high-risk, it is correct 91% of the time.
- Recall for high-risk loans (label 1) is 0.85, indicating that the model correctly identifies 85% of the actual high-risk loans.

*Logistic Regression Model with Resampled Data:*
- The model achieved a slightly lower balanced accuracy score of 0.9128 compared to the original data model.
- Precision for high-risk loans (label 1) remains at 0.91, indicating consistent accuracy in identifying high-risk loans.
- Recall for high-risk loans (label 1) decreased to 0.83, suggesting that the resampled data model misses more actual high-risk loans compared to the original data model.

In summary, both models are effective in predicting credit risk, but the logistic regression model trained on the original data slightly outperforms the model trained on resampled data. The original data model has a higher balanced accuracy score and better recall for high-risk loans. 

**Recommendation**:
- It is recommended to use the logistic regression model trained on the original data for credit risk prediction. It provides a slightly better overall performance, especially in correctly identifying high-risk loans. However, it is crucial to continue monitoring and improving the model's performance as the dataset evolves and more data becomes available.

**Justification**:
- The original data model achieves a higher balanced accuracy score and better recall for high-risk loans, making it more reliable for identifying potential credit risks. The minimal difference in precision between the two models does not justify the use of resampled data, as it sacrifices recall, which is critical in credit risk assessment. Moreover, using the original data aligns with the principle of not artificially altering the dataset unless there is a compelling reason to do so.
