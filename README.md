# CreditCardFraudDetection
The dataset covers credit card transactions done by European cardholders in September 2013. 
In this dataset, we have 492 frauds out of 284,807 transactions that occurred in the last two days. The dataset is heavily skewed, with the positive class (frauds) accounting for only 0.172 percent of all transactions. 

It only has numerical input variables that have undergone a PCA transformation. We are unable to give the original features and further background information about the data owing to confidentiality concerns. The major components derived with PCA are features V1, V2,... V28; the only features not changed with PCA are 'Time' and 'Amount.' The seconds elapsed between each transaction and the first transaction in the dataset are stored in the feature 'Time.'The transaction Amount is represented by the feature 'Amount,' which can be utilized for example-dependent cost-sensitive learning. The answer variable is called 'Class,' and it has a value of 1 when there is fraud and 0 when there isn't. 

We recommend testing accuracy using the Area Under the Precision-Recall Curve because of the class imbalance ratio (AUPRC). For unbalanced categorization, the accuracy of the confusion matrix is meaningless.
