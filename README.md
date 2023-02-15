In the medical field, accuracy is not the ideal metric for the evaluation of diagnostic models.

Firstly, in biomedical image settings, the dataset is imbalanced. Therefore, calculating the accuracy of a model leads to an incorrect evaluation of models.
For example, suppose the ground truth of the whole dataset is 8 negative and 2 positive (which is the case in real life medical settings). A model that simply predicts every instance to be negative, achieves an accuracy score of 80% ((True Negative + True Positive) / (True Negative + True Positive + False Positive + False Negative)).

On the other hand, a model that detects all the positive cases (2 in this case) and gets 3 negative cases wrong achieves an accuracy score of 70%((5 + 2) / (5 + 2 + 0 + 3)).

At first glance, the first model might seem impressive, but it fails to detect any positive cases (the most important aspect in the medical field). However, the second model does not beat the accuracy score of the first one but gets all the positive cases right. Moreover, detecting cancer cells (positive samples) is of much more importance than negative cases.

Therefore, it is necessary to use different evaluation metrics to successfully evaluate the models. In this assignment of Coursera: Evaluation of Diagnostic Models, I have understood and calculated the different evaluation metrics.
