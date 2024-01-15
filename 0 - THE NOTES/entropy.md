---
type: topic
field: AI
short_desc: '"Entropy is a measure of chaos in the dataset."'
field_type: machine learning
module: "6"
parent: main
---


202401111627
Status: #m6
Tags: [[AI]]

# entropy

Entropy is a measure of chaos in the dataset. The less chaos the better. The more chaos, the more information needed to tell the class of a datapoint/example.

# Formula - Shannon's Entropy

$$E(S)=\sum\limits_{i=1}^{c}-P_{i}Log_2(P_i)$$

$S$ = dataset
$c$ = a class, so we apply the sum for each class in our dataset
$P_{i}$ = the probability of the $i_{th}$ class

# Examples

![[Pasted image 20240111163319.png]]

Here we have two classes -> $Yes$ and $No$ (look at the $Covid$) column.

![[Pasted image 20240111181312.png]]

![[Pasted image 20240111181345.png]]

# References

1. [[information gain]]