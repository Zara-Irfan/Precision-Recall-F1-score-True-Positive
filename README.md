Precision, Recall, F1 Score, and True Positives

This document explains the key performance metrics used to evaluate classification models. These metrics go beyond simple accuracy and help us understand how well a model is performing, especially when the dataset is imbalanced.

True Positive (TP)

A True Positive occurs when the model correctly predicts the positive class.

Example: If the model predicts “Dog” and the actual label is also “Dog”, that’s a TP.

Precision

Definition: Out of all the samples the model predicted as positive, how many were actually positive?

Formula:

Precision
=
TP
TP + FP
Precision=
TP + FP
TP
	​


Meaning: Precision answers “When the model says YES, how often is it correct?”

Example: In spam detection, if precision is high, it means most emails flagged as spam are really spam.

Recall (Sensitivity or True Positive Rate)

Definition: Out of all the actual positive samples, how many did the model correctly identify?

Formula:

Recall
=
TP
TP + FN
Recall=
TP + FN
TP
	​


Meaning: Recall answers “Out of all real YES cases, how many did the model catch?”

Example: In medical testing, a high recall means fewer sick patients go undetected.

⚖️ F1 Score

Definition: The harmonic mean of Precision and Recall.

Formula:

𝐹
1
=
2
×
Precision
×
Recall
Precision + Recall
F1=2×
Precision + Recall
Precision×Recall
	​


Meaning: F1 balances both Precision and Recall.

Useful when classes are imbalanced and you want a single score combining both.

Why These Metrics Matter

Accuracy alone can be misleading.
Example: If 95% of emails are not spam, a model that predicts “Not Spam” always will be 95% accurate but useless.

Precision, Recall, and F1 Score provide a deeper understanding of model strengths and weaknesses.

Summary

True Positive (TP): Correct positive prediction.

Precision: How reliable positive predictions are.

Recall: How many actual positives are detected.

F1 Score: Balance between Precision and Recall.
