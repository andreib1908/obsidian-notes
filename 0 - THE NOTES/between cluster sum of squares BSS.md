---
type: topic
field: AI
short_desc: '"The metric used here to quantify separation is the Between Cluster Sum of Squares (BSS). It measures the variance between the clusters, or in other words, how spread out the clusters are from each other."'
field_type: machine learning
module: "6"
parent: "[[error measure]]"
---


202401111549
Status: #m6
Tags: [[AI]]

# between cluster sum of squares BSS

![[Pasted image 20240111155246.png]]

**Separation** refers to the extent to which different clusters are distinct from each other. It is a measure of how well the clustering algorithm has partitioned the different data points into clearly distinct groups.

# Formula

$$BSS = \sum\limits_{i}\lvert C_{i}\rvert(m-m_{i})^{2}$$
# References

1. [[error measure]]