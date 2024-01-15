---
type: topic
field: AI
short_desc: '"A note related to artificial intelligence concepts."'
field_type: machine learning
module: "6"
parent: "[[error measure]]"
---


202401111520
Status: #m6
Tags: [[AI]]

# confusion matrix

![[Pasted image 20240111152133.png]]

![[Pasted image 20240111152145.png]]
1. **Generic Confusion Matrix (Left):** This is the standard format of a confusion matrix for a binary classifier, which has two classes: Positive and Negative. It shows the four possible outcomes of prediction:
    
    - True Positives (TP): The cases when the model correctly predicts the positive class.
    - True Negatives (TN): The cases when the model correctly predicts the negative class.
    - False Positives (FP): The cases when the model incorrectly predicts the positive class (also known as Type I error).
    - False Negatives (FN): The cases when the model incorrectly predicts the negative class (also known as Type II error).
2. **Normalized Confusion Matrix (Right):** This matrix shows the same information as the generic one but in a normalized format, which means the numbers represent proportions rather than counts. Each cell in the matrix shows the proportion of predictions in that category relative to the total number of true labels. For example, if there are 100 positive cases and the model predicts 90 of them correctly, the TP cell would show 0.90. This type of matrix is particularly useful when the class distribution is imbalanced because it allows you to see the relative rates of correct and incorrect predictions.
# Formula

>[!Success] Accuracy
>$$Acc=\frac {TP+TN}{TP+TN+FP+FN}$$

>[!success] Precision
>$$Precision = \frac{TP}{TP+FP}$$

>[!success] $F_{score}$
>$$F_{score}=2 * \frac{Precision*Recall}{Precision+Recall}$$

>[!success] Recall/Sensitivity/TruePositiveRate
>$$Recall \space or \space Sensitivity \space or \space TruePositiveRate= \frac{TP}{TP+FN}$$

>[!success] Specificity/TrueNegativeRate
>$$Specificity \space or \space TrueNegativeRate = \frac{TN}{TN+FP}$$
# References

1. [[validation]]
2. [[error measure]]
3. [[supervised learning]]