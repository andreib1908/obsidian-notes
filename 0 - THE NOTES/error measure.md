---
type: topic
field: AI
short_desc: '"A note related to artificial intelligence concepts."'
field_type: AI + logic
module: "6"
parent:
---


202401111519
Status: #m6
Tags: [[AI]]

# error measure

![[Pasted image 20240111151914.png]]

# Error Strategies for Supervised Learning

## For classification - confusion matrix

[[confusion matrix]]

## For regression - Sum of squared errors SSE

[[sum of squared errors SSE]]

# Error Strategies for Unsupervised learning

## For Clustering - Within sum squared errors (WSS)

[[within sum squared errors WSS]]

## For Clustering - Between cluster sum of squares (BSS)

[[between cluster sum of squares BSS]]

# Examples

## Unsupervised learning - WSS and BSS

![[Pasted image 20240111155632.png]]

![[Pasted image 20240111155639.png]]

We are given a data size with 4 relevant sample points: $1$, $2$, $4$ and $5$.

The number $3$ is at the center of the dataset, so it becomes the **centroid**.

### K = 1 cluster - we look for one cluster

![[Pasted image 20240111155843.png]]

![[Pasted image 20240111160826.png]]
### K = 2 cluster - we look for two clusters

![[Pasted image 20240111160734.png]]

![[Pasted image 20240111160836.png]]
### Total

![[Pasted image 20240111160814.png]]

![[Pasted image 20240111160848.png]]

![[Pasted image 20240111160903.png]]

# References

1. [[data classification]]
2. [[regression]]
3. [[confusion matrix]]
4. [[sum of squared errors SSE]]
5. [[supervised learning]]
6. [[unsupervised learning]]