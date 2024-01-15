---
type: topic
field: math
field_type: probability
parent: "[[conditional probability]]"
short_desc: '"Solving probability for distributions such as P(A,B).."'
module: "6"
---

202401100145
Status: #m6
Tags: [[math]] 

# probability product rule

It's a method used to calculate $P(A,B)$ instead of grabbing it from a table.

# probability chain rule

It's a very powerful rule that holds true regardless of the distribution $X_1,\dots,X_n$.

The **chain rule** states that instead of specifying all [[joint probability|joint probabilities]] $P(X_1,\dots,X_n)$, you can specify only $P(X_{1),}P(X_2|X_{1),}P(X_3|X_1,\dots,X_2),\dots,P(X_n|X_1,\dots,X_{n-1})$.

This is very useful when working with large data structures, or [[full joint probability distribution|full joint probability distributions]].
# Formula

## Product Rule

>[!success] Formula
>$$P(A,B) = P(A|B)*P(B)=P(B|A)*P(A)$$
>$$P(A|B) = \frac {P(A,B)}{P(B)}$$
## Chain Rule

$$For \space n \space variables \space X_{1,}X_2,\dots,X_n:$$
$$P(X_1,\dots,X_{n})= P(X_1,\dots,X_{n-1})*P(X_n|X_1,\dots,X_{n-1})=$$
$$= P(X_{1,\dots,}X_{n-2})*P(X_{n-1}|X_1,\dots,X_{n-2})*P(X_n|X_1,\dots,X_{n-1})=$$
>[!success] Formula
>$$P(X_1,\dots,X_{n-2})=\prod_{i=1}P(X_i|X_1,\dots,X_{i-1})$$
>That symbol just says "the product of every i starting from 1".


# Examples

![[Pasted image 20240110014855.png]]

## Product Rule

$$P(headache, covid) = P(headache|covid) * P(covid) = P(covid|headache)*P(headache)$$

## Chain Rule

![[Pasted image 20240110021458.png]]

So we can calculate this [[vector of probability - probability distribution|vector of probability]] using [[conditional probability]].  All fine 'til here. 

But what if we want to calculate $P(\lnot covid|headache)$?

We can use a combination of the [[conditional probability#Bayes' Theorem|Baye's Theorem (Rule)]] and [[probability product rule (chain rule)#Product Rule|Product Rule]]:

![[Pasted image 20240110021934.png]]


# References

1. [[random variable]]
2. [[conditional probability]]
3. [[full joint probability distribution]]
4. [[joint probability]]
5. [[conditional probability]]