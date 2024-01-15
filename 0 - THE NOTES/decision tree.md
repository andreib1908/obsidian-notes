---
type: topic
field: AI
short_desc: '"A note related to artificial intelligence concepts."'
field_type: AI + logic
module: "6"
parent:
---


202401111615
Status: #m6
Tags: [[AI]]

# decision tree

In [[supervised learning]], you are given a function of the type $f(x)=y$ where we have to map the input x to an output y. The $f$ is the decision tree, usually.

Decision trees are a form of structuring a data table with labels so we can infer an output as quickly as possible.

It's a tree-like model to fit the data.

![[Pasted image 20240111161749.png]]

>[!warning] Note
>There can be multiple decision trees for the same dataset!

![[Pasted image 20240111162319.png]]

>[!warning] Possible problem - overfitting
>Deeper decision trees can lead to [[over-fitting]]
# Terminology

Training Data:
![[Pasted image 20240111162009.png]]

Model: Decision Tree
![[Pasted image 20240111162050.png]]

# Building a decision tree

To build (induce) a decision tree we need:
1. Data
2. An algorithmic method to select the best attribute at the root of the tree
3. Repeat the process recursively.

## Algorithmic Method

There are several, but the one we're going to use is [[information gain]].
# Examples

Given this table:
![[Pasted image 20240111161737.png]]

## First type of decision tree for the same dataset

We can model a decision tree:
![[Pasted image 20240111161749.png]]

Teacher's scribbles to understand input and output:

![[Pasted image 20240111161835.png]]

## Second type

![[Pasted image 20240111162235.png]]
# References

1. [[over-fitting]]