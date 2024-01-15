---
type: topic
field: AI
field_type: probabilistic reasoning
parent: 
short_desc: '"An array of probabilities (numerical)."'
module: "6"
---

202401082330
Status: #m6
Tags: [[math]] 

# vector of probability

Also known as **the probability distribution of a table or data frame**.

It's an array made of multiple probabilities. It's always denoted by a 'P' written in bold: $\textbf P$.

>[!note] Note
>The sum of all probabilities within this array is always 1.

# Formula

$$\textbf P(condition) = [P(condition), P(\lnot condition)]$$

# Examples

![[Pasted image 20240108233319.png]]

$$\textbf P(Headache) = [P(headache), P(\lnot headache)] = [0.47, 0.53]$$

$$\textbf P(Headache, Covid) = [[P(headache, covid), P(headache, \lnot covid)], [P(\lnot headache, covid) P(\lnot headache, \lnot covid)]]$$
# References

1.  [[full joint probability distribution]]
2. [[random variable]]