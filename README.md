# Card-Fraud-Detection



For this part of the question, your dataset is a subset of the credit card fraud detection dataset [3]. The dataset contains only numerical input variables which are the result of the PCA transformation, i.e. features V1, V2, ... V28 are the principal components obtained from PCA. The only feature which has not been transformed with PCA is Amount. The Class column is the response variable and it takes value 1 in case of fraud and 0 otherwise.
You will use the following files:
• q4-train-dataset.csv • q4-test-dataset.csv




F1, F2, precision, recall and accuracy for full batch sized in logistic regression. The interpretation of the weights in logistic regression differs from the interpretation of the weights in linear regression, since the outcome in logistic regression is a probability between 0 and 1. The weights do not influence the probability linearly any longer. The weighted sum is transformed by the logistic function to a probability[1]. During the prediction we multiply PCA values of features so if any feature has higher value(with absolute) affecting more the prediction. So V4, V5, V9, V10, V11, V17, V22, V25, V26, V28 becomes most important 10 features according to dataset. When you check for dataset, you can see that they have biggest absolute values. For this part, some learning rate values. 
Q 4.3) NPV, FPR, FDR, F1 and F2 score might be a better measure to use
if we need to seek a balance between precision and recall and there is an uneven class distribution (large number of Actual Negatives). Let us think a

prediction case having huge number of true negative values. It would have huge accuracy but for example positive here represents fraud case. So in this model it is better idea to user NPV, FPR, FDR, F1 and F2 score to get better predictions instead of precision or recall.
