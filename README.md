Credit Risk Analysis Report

Overview of Process:
1. Data collection via CSV file
2. Data pre-processing
3. Feature selection
4. Data splitting between training and testing
5. Model selection
6. Training
7. Evaluation of test data using accuracy, precision, recall and F1 score

Results:
The support level for the test data is unbalanced. There was total of 19,384 labels predicted during the test of which 18,765 were healthy loans and 619 were high-risk loans.
The accuracy score came in at 0.99. The accuracy score of 99% is good but the imbalanced support level detracts from the high accuracy.
The precision score of .84 for the high-risk loans tells us that 84% of the high-risk loans predicted were actually high-risk loans. Thus, 16% of the healthy loans were miss-classified as high-risk.
The recall score of .94 for high risk loans tells us that the model predicted 94% of the high risk loans accurately. Thus, 6% of labels were high risk loans that were mis-classified at healthy.

Impacts to the Business from the Confusion Matrix:
107 of the false positives represents potential lost opportunities for the bank because these are the loans that were classified as high-risk when they are actually healthy.
37 of the false negatives represents the potential for financial loss because these are the loans that were classified as healthy when they are actually high-risk.

Recommendation: 
At this time, I would not recommend moving this model into production.
Instead, I would resample the test data in an attempt to rebalance the support levels and run the test again.