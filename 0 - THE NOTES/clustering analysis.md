---
type: topic
field: AI
short_desc: '"Organize samples into categories (clusters) by similarity."'
field_type: reinforcement learning
module: "6"
parent: main
---


202401112220
Status: #m6
Tags: [[AI]]

# clustering analysis

Clustering analysis is to partition a set of data points into groups such that points  
within the same group (a cluster) are more similar than to those in other groups  
(different clusters).

We just group them into categories basically.

![[Pasted image 20240111222251.png]]

# Clustering vs Classification

![[Pasted image 20240111222331.png]]

# Clustering algorithms

![[Pasted image 20240111222414.png]]

# Hierarchical Clustering

Hierarchical clustering is a method of cluster analysis which seeks  
to build a hierarchy of clusters.

![[Pasted image 20240111222534.png]]

## Proximity Matrix

The method depicted here is the agglomerative clustering.

![[Pasted image 20240111222627.png]]

So the cells just represent how close the data points are to each other. You can see that A-B is 1 and A-C is 2.8. It makes sense look at the graphs.

![[Pasted image 20240111222718.png]]

So, we can group A and B.

![[Pasted image 20240111222742.png]]
![[Pasted image 20240111222757.png]]

And we can do the same with D and E because they are very close to each other (distance of 2).

![[Pasted image 20240111222832.png]]
![[Pasted image 20240111222844.png]]

![[Pasted image 20240111222901.png]]
![[Pasted image 20240111222910.png]]

And so on until we have gone through each short distances and put our data points into hierarchical clusters.

The thing on the right is called a [[dendrogram]].

# Different types of hierarchical clustering

## Agglomerative (bottom up) clustering

![[Pasted image 20240111223311.png]]

The dendrogram is built from the bottom level by merging similar pair of samples/clusters. It stops when all the data samples are merged into one single cluster/ the root cluster.

### Basic Algorithm for agglomerative hierarchical clustering

![[Pasted image 20240111223428.png]]

# Divisive (top down) clustering

![[Pasted image 20240111223353.png]]

Starts with all data points in one cluster, the root, then continues splitting into subsets until clusters with a single sample remain.

# Data linkage measures
  
Linkage measure defines the distance between two clusters in a unique way.

![[Pasted image 20240111223559.png]]

Remember that the absolute value of C1 means how many data samples in total you have in cluster 1, like 1000 samples.

![[Pasted image 20240111223639.png]]

![[Pasted image 20240111223649.png]]

![[Pasted image 20240111223656.png]]
![[Pasted image 20240111223707.png]]

# How to choose the linkage measure

No single criterion!  
● single linkage is fast, and can perform well on  
non-globular data, but it performs poorly in the  
presence of noise.  
● average and complete linkage perform well on  
cleanly separated globular clusters, but have mixed  
results otherwise.  
● Ward’s is the most effective method for noisy data.
# References

1. [[unsupervised learning]]
2. [[supervised learning]]
3. [[cluster validity]]