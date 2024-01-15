---
type: topic
field: AI
short_desc: "\"\rWhat is the “goodness” of the resulting clusters?\""
field_type: reinforcement learning
module: "6"
parent: "[[cluster validity]]"
---


202401112238
Status: #m6
Tags: [[AI]]

# cluster validity

Aspects of cluster validity:
-  Determine the ‘correct’ number of clusters  
-  Compare different clustering algorithms  
-  Evaluate how well the results of a cluster analysis fit the data without reference to external information

# Measures

### Internal Index

**Internal Index:** measure the goodness of a clustering structure without external
information.

![[Pasted image 20240111224053.png]]

[[within sum squared errors WSS]]
[[between cluster sum of squares BSS]]

![[Pasted image 20240111224130.png]]

![[Pasted image 20240111224337.png]]

> [!success] Silhouette Score Formula
> $$Silhouette_{score} = \frac{1}{n}\sum\limits_{i=1}^{n} \frac {b_{i}-a_{i}} {max(a_{i}b_{i})}$$

![[Pasted image 20240111224408.png]]
### External Index

**External Index:** measure the extent to which cluster labels match externally
supplied class labels.

![[Pasted image 20240111224425.png]]

[[confusion matrix]]

![[Pasted image 20240111224438.png]]

# References

1. [[clustering analysis]]
2. [[within sum squared errors WSS]]
3. [[between cluster sum of squares BSS]]
4. [[confusion matrix]]