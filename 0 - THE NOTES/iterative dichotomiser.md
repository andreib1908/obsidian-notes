---
type: topic
field: AI
short_desc: '"Algorithm for sorting out decision trees."'
field_type: machine learning
module: "6"
parent: "[[decision tree]]"
---


202401111823
Status: #m6
Tags: [[AI]]

# iterative dichotomiser

The algorithm works as follows:
1. Find the attribute/feature that provides the highest [[information gain]].
2. Create a node using the feature (provides the highest [[gain]])
3. Sort out the examples to the corresponding split
4. If all data points belong to the same class, create a leaf node.
5. If the data points have different classes, recurse.

![[Pasted image 20240111183041.png]]
# Example

![[Pasted image 20240111182747.png]]
![[Pasted image 20240111183100.png]]

# References

1. [[information gain]]
2. [[gain]]
3. [[decision tree]]