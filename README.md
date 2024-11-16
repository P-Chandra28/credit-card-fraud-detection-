# Movie-Genre-Multi-Label-Text-Classification

In this project, we are going to predict the fraudulent transactions of a credit card. In this we are using a dataset provided by the Kaggle for the training of the model. This dataset consists of 284807 credit card transactions in which up to 492 are fraud transactions. The data is now read by the model and the model describes the data shape and the description of the data. The following data gives the outliers(fraudulent transactions), genuine and the outliers fraction.

<img height=400 src=".\week 1\results\dataread.png"/>

So to understand the correlation between all the given features we can use the correlation matrix(heatmap).This gives us a deeper understanding of the Data available to us. In the HeatMap we can clearly see that most of the features do not correlate to other features but there are some features that either has a positive or a negative correlation with each other. For example, V2 and V5 are highly negatively correlated with the feature called Amount. We also see some correlation with V20 and Amount.

<img src=".\week 1\results\heatmap.png"/>

Few evaulating parameters and metrics used to test the model accuracy.
* **Accuracy score**: In this accuracy score, it the proportion of correctly classified instances out of all instances. It’s suitable for balanced datasets but may mislead when classes are imbalanced.

* **Precision score**: This metric score evaluates how many of the predicted positive labels are actually correct. High precision is essential when false positives are costly.It's helpful in problems like spam detection, where marking a genuine email as spam is problematic.

* **Recall Score**: Recall focuses on capturing as many actual positives as possible. It gives us how many true positive have been measured by the model correctly.

* **F1 score**: F1-score balances precision and recall, offering a single measure that accounts for both. It’s especially useful when the dataset is imbalanced like in this case.
* **Mathews Correlation Coeeficient(MCC)**: MCC is a balanced metric for evaluating binary classification models, especially useful for imbalanced datasets. It considers all parts of the confusion matrix (TP, TN, FP, FN) and provides a single score ranging from -1 to 1:
1: Perfect predictions
0: Random predictions
-1: Completely wrong predictions

The following images show the metric scores of random forest and the decision tree model  classification.

<img src=".\week 1\results\randomforest.png">
<img src=".\week 1\results\decisiontree.png">


#Visual representation of the confusion matrix of the random forest classification.

<img src=".\week 1\results\confmatrix.png">








