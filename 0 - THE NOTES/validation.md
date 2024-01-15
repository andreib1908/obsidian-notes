---
type: topic
field: AI
short_desc: '"A note related to artificial intelligence concepts."'
field_type: machine learning
module: "6"
parent: "[[generalization]]"
---


202401111340
Status: #m6
Tags: [[AI]]

# validation

We want to validate our data.

# Procedures

![[Pasted image 20240111134149.png]]

- $D$: This represents the entire available dataset which is composed of samples. Each sample has features (inputs) and an associated label (output). The dataset is indexed by $μ$ running from 1 to $P$, where $P$ is the total number of samples in the dataset.
    
- ${ξ^{μ},S^{μ}}$: Each sample in the dataset $D$ consists of a feature vector $ξ^μ$ and a label $S^μ$. The superscript $μ$ is the index of the sample.
    
- $D_{training}$​: This is the [[training set]]. It is a subset of $D$ used to train the model. It consists of $Q$ samples, which are randomly selected from $D$. This set helps the model learn the underlying patterns in the data.
    
- $D_{test}$: This is the [[test set]]. It is the complementary subset of $D$ that is not used in training. It usually consists of the remaining $P−Q$ samples (though this specific split is not detailed in the slide). This set is used to evaluate the [[generalization]] performance of the model, meaning how well the model performs on unseen data.
    
- $μ=1$ to $Q$: This indicates that the [[training set]] $D_{training}$​ contains samples indexed from 1 to $Q$.
    
- $μ=Q+1$ to $P$: This indicates that the [[test set]] $D_{test}$​ contains samples indexed from $Q+1$ to $P$, the remaining samples after the [[training set]].

# Strategies for validation

## n-fold cross-validation

![[Pasted image 20240111142527.png]]

![[Pasted image 20240111142551.png]]
![[Pasted image 20240111142610.png]]

![[Pasted image 20240111142712.png]]


# Problems

**Lack of data**: can we afford to *waste* example data *only* for validation?
- Labeled data sets are very uncommon because they are time-expensive.

**Representative results**: 
- Lucky/unlucky set composition can give misleading outcomes.

**Validation of results:**
- How safe is the prediction? Error bars of the estimates?

# Error measure

[[error measure]]
# References

1. [[generalization]]
2. [[supervised learning]]
3. [[training set]]
4. [[validation set]]
5. [[test set]]
6. [[over-fitting]]
7. [[error measure]]