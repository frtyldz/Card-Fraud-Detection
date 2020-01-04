# Card-Fraud-Detection



For this part of the question, your dataset is a subset of the credit card fraud detection dataset [3]. The dataset contains only numerical input variables which are the result of the PCA transformation, i.e. features V1, V2, ... V28 are the principal components obtained from PCA. The only feature which has not been transformed with PCA is Amount. The Class column is the response variable and it takes value 1 in case of fraud and 0 otherwise.
You will use the following files:
• q4-train-dataset.csv • q4-test-dataset.csv




F1, F2, precision, recall and accuracy for full batch sized in logistic regression. The interpretation of the weights in logistic regression differs from the interpretation of the weights in linear regression, since the outcome in logistic regression is a probability between 0 and 1. The weights do not influence the probability linearly any longer. The weighted sum is transformed by the logistic function to a probability[1]. During the prediction we multiply PCA values of features so if any feature has higher value(with absolute) affecting more the prediction. So V4, V5, V9, V10, V11, V17, V22, V25, V26, V28 becomes most important 10 features according to dataset. When you check for dataset, you can see that they have biggest absolute values. For this part, some learning rate values. Here is the output
126
True Positive: 47
True Negative: 63
False Positive: 0
False Positive: 16
Precision: 1.0
Recall: 0.746031746031746
FDR: 0.0
NPV: 0.7974683544303798
FPR: 0.0
f1: 1.1454545454545455
f2: 1.0535117056856187
REAL->     Pos.        Neg.
|--------------------------| Pos.|47 0 |
 Neg.|16 63 | |--------------------------|
Test Accuracy for learn rates of 0.00001 in 1000
iterations:
87.3015873015873
126
True Positive: 48
True Negative: 63
False Positive: 0
False Positive: 15
Precision: 1.0
Recall: 0.7619047619047619
FDR: 0.0
NPV: 0.8076923076923077
FPR: 0.0
f1: 1.135135135135135
f2: 1.05
REAL-> Pos. Neg. |--------------------------| Pos.|48 0 |
Neg.|15 63 | |--------------------------|
Test Accuracy for learn rates of 0.0001 in 1000 iterations:
88.09523809523809
126
True Positive: 49
True Negative: 62
False Positive: 1
False Positive: 14
Precision: 0.98
Recall: 0.7777777777777778
FDR: 0.02
NPV: 0.8157894736842105
FPR: 0.015873015873015872
f1: 1.1150442477876106
f2: 1.0430463576158941
REAL->     Pos.        Neg.
|--------------------------| Pos.|49 1 | Neg.|14 62 |

      |--------------------------|
Test Accuracy for learn rates of 0.001 in 1000 iterations:
88.09523809523809
126
True Positive: 52
True Negative: 58
False Positive: 5
False Positive: 11
Precision: 0.9122807017543859
Recall: 0.8253968253968254
FDR: 0.08771929824561403
NPV: 0.8405797101449275
FPR: 0.07936507936507936
f1: 1.05
f2: 1.0194174757281553
REAL->     Pos.        Neg.
|--------------------------| Pos.|52 5 | Neg.|11 58 |
     |--------------------------|
Test Accuracy for learn rates of 0.01 in 1000 iterations:
87.3015873015873
126
True Positive: 51
True Negative: 51
False Positive: 12
False Positive: 12
Precision: 0.8095238095238095
Recall: 0.8095238095238095
FDR: 0.19047619047619047
NPV: 0.8095238095238095
FPR: 0.19047619047619047
f1: 1.0
f2: 1.0
REAL->     Pos.        Neg.
|--------------------------| Pos.|51 12 | Neg.|12 51 |
     |--------------------------|
Test Accuracy for learn rates of 0.1 in 1000 iterations:

 80.95238095238095
Best learn rate is: 0.001
In here we see some increase and decrease in accuracy values. The reason for that is step size. If we choose big step size in gradient descent, we can pass over the total minimum value. Otherwise, we can never reach the maximum size so best learning rate becomes 0.001 which is somewhere in the middle of values tried.
As well as this one I tried with different iteration counts which are from 100 to 1000. Here is the output
126
True Positive: 49
True Negative: 62
False Positive: 1
False Positive: 14
Precision: 0.98
Recall: 0.7777777777777778
FDR: 0.02
NPV: 0.8157894736842105
FPR: 0.015873015873015872
f1: 1.1150442477876106
f2: 1.0430463576158941
REAL->     Pos.        Neg.
|--------------------------| Pos.|49 1 | Neg.|14 62 |
     |--------------------------|
Test Accuracy for learn rates of 0.1 in 100 iterations:
88.09523809523809
126
True Positive: 49
True Negative: 62
False Positive: 1
False Positive: 14

 Precision: 0.98
Recall: 0.7777777777777778
FDR: 0.02
NPV: 0.8157894736842105
FPR: 0.015873015873015872
f1: 1.1150442477876106
f2: 1.0430463576158941
REAL->     Pos.        Neg.
|--------------------------| Pos.|49 1 | Neg.|14 62 |
     |--------------------------|
Test Accuracy for learn rates of 0.1 in 200 iterations:
88.09523809523809
126
True Positive: 50
True Negative: 62
False Positive: 1
False Positive: 13
Precision: 0.9803921568627451
Recall: 0.7936507936507936
FDR: 0.0196078431372549
NPV: 0.8266666666666667
FPR: 0.015873015873015872
f1: 1.105263157894737
f2: 1.0396039603960394
REAL->     Pos.        Neg.
|--------------------------| Pos.|50 1 | Neg.|13 62 |
     |--------------------------|
Test Accuracy for learn rates of 0.1 in 300 iterations:
88.88888888888889
126
True Positive: 50
True Negative: 62
False Positive: 1
False Positive: 13
Precision: 0.9803921568627451
Recall: 0.7936507936507936

 FDR: 0.0196078431372549
NPV: 0.8266666666666667
FPR: 0.015873015873015872
f1: 1.105263157894737
f2: 1.0396039603960394
REAL->     Pos.        Neg.
|--------------------------| Pos.|50 1 | Neg.|13 62 |
     |--------------------------|
Test Accuracy for learn rates of 0.1 in 400 iterations:
88.88888888888889
126
True Positive: 51
True Negative: 61
False Positive: 2
False Positive: 12
Precision: 0.9622641509433962
Recall: 0.8095238095238095
FDR: 0.03773584905660377
NPV: 0.8356164383561644
FPR: 0.031746031746031744
f1: 1.0862068965517242
f2: 1.0327868852459017
REAL->     Pos.        Neg.
|--------------------------| Pos.|51 2 | Neg.|12 61 |
     |--------------------------|
Test Accuracy for learn rates of 0.1 in 500 iterations:
88.88888888888889
126
True Positive: 51
True Negative: 59
False Positive: 4
False Positive: 12
Precision: 0.9272727272727272
Recall: 0.8095238095238095
FDR: 0.07272727272727272
NPV: 0.8309859154929577

 FPR: 0.06349206349206349
f1: 1.0677966101694916
f2: 1.0260586319218243
REAL->     Pos.        Neg.
|--------------------------| Pos.|51 4 | Neg.|12 59 |
     |--------------------------|
Test Accuracy for learn rates of 0.1 in 600 iterations:
87.3015873015873
126
True Positive: 51
True Negative: 59
False Positive: 4
False Positive: 12
Precision: 0.9272727272727272
Recall: 0.8095238095238095
FDR: 0.07272727272727272
NPV: 0.8309859154929577
FPR: 0.06349206349206349
f1: 1.0677966101694916
f2: 1.0260586319218243
REAL->     Pos.        Neg.
|--------------------------| Pos.|51 4 | Neg.|12 59 |
     |--------------------------|
Test Accuracy for learn rates of 0.1 in 700 iterations:
87.3015873015873
126
True Positive: 51
True Negative: 58
False Positive: 5
False Positive: 12
Precision: 0.9107142857142857
Recall: 0.8095238095238095
FDR: 0.08928571428571429
NPV: 0.8285714285714286
FPR: 0.07936507936507936
f1: 1.0588235294117647

 f2: 1.0227272727272727
REAL->     Pos.        Neg.
|--------------------------| Pos.|51 5 | Neg.|12 58 |
     |--------------------------|
Test Accuracy for learn rates of 0.1 in 800 iterations:
86.5079365079365
126
True Positive: 52
True Negative: 58
False Positive: 5
False Positive: 11
Precision: 0.9122807017543859
Recall: 0.8253968253968254
FDR: 0.08771929824561403
NPV: 0.8405797101449275
FPR: 0.07936507936507936
f1: 1.05
f2: 1.0194174757281553
REAL->     Pos.        Neg.
|--------------------------| Pos.|52 5 | Neg.|11 58 |
     |--------------------------|
Test Accuracy for learn rates of 0.1 in 900 iterations:
87.3015873015873
126
True Positive: 52
True Negative: 58
False Positive: 5
False Positive: 11
Precision: 0.9122807017543859
Recall: 0.8253968253968254
FDR: 0.08771929824561403
NPV: 0.8405797101449275
FPR: 0.07936507936507936
f1: 1.05
f2: 1.0194174757281553
REAL->     Pos.        Neg.

 |--------------------------| Pos.|52 5 | Neg.|11 58 |
     |--------------------------|
Test Accuracy for learn rates of 0.1 in 1000 iterations:
87.3015873015873
We see some increase and decrease in the accuracy rates. But in total there is an increase when iteration count increases because with more iteration we have bigger chance to create better weights to serve prediction. We try more to reach best weights. Those trials have been made with full batch size which is 800 for this data. That means the weight value is updated once in 800 times. In the data given, I normalized the data to get higher accuracy. The position of the data cumulated in the plot was not near to the origin so we should normalize the data for better prediction.
Q 4.2) For this part I tried the batch size as 32 which shows better
chance to update the weights. We add learn rate times gradient value at each time to weights and less batch size give us the chance of updating more. The situation is even better for stochastic logistic regression whose batch size is one. The output for mini batch(32)
126
True Positive: 49
True Negative: 62
False Positive: 1
False Positive: 14
Recall: 0.7777777777777778
FDR: 0.02
NPV: 0.8157894736842105

 FPR: 0.015873015873015872
f1: 0
f2: 0
REAL->     Pos.        Neg.
|--------------------------| Pos.|49 1 | Neg.|13 63 |
     |--------------------------|
Test Accuracy for learn rates of 0.1 in 1000 iterations:
89.09523809523809
The output for stochastic one
126
True Positive: 49
True Negative: 62
False Positive: 1
False Positive: 14
Precision: 0.98
Recall: 0.7777777777777778
FDR: 0.02
NPV: 0.8157894736842105
FPR: 0.015873015873015872
f1: 1.1150442477876106
f2: 1.0430463576158941
REAL->     Pos.        Neg.
|--------------------------| Pos.|49 0 | Neg.|13 64 |
     |--------------------------|
Test Accuracy for learn rates of 0.1 in 1000 iterations:
90.09523809523809
Q 4.3) NPV, FPR, FDR, F1 and F2 score might be a better measure to use
if we need to seek a balance between precision and recall and there is an uneven class distribution (large number of Actual Negatives). Let us think a

prediction case having huge number of true negative values. It would have huge accuracy but for example positive here represents fraud case. So in this model it is better idea to user NPV, FPR, FDR, F1 and F2 score to get better predictions instead of precision or recall.
