---
type: topic
field: math
field_type: probability
parent: 
short_desc: '"Probability of random variable or event A happening given that event B is true or happened."'
module: 4, 6
---
202401082318
Status: #m6
Tags: [[math]] 

# conditional probability

It's the [[joint probability]] of an event occurring, or [[random variable|RV]], **given** that another event, or [[random variable|RV]] had occurred, or is true.

It's also known as the *posterior probability*.
# Formula

## General
$$P(A|B) = \frac {P(A \cap B)} {P(B)} = \frac {P(A,B)} {P(B)}$$
## Bayes' Theorem

$$P(A|B) = \frac {P(B|A)*P(A)} {P(B)}$$

>[!warning] CONDITION
>$$P(B) > 0$$

![[Pasted image 20240110021959.png]]

# Examples

![[Pasted image 20240108232411.png]]
## Using the general formula

$$P(headache|covid)= \frac {P(headache,covid)} {p(covid)}$$
$$P(headache|covid)= \frac {0.25+0.05}{0.25+0.05+0.10+0.01} = 0.30/0.41$$

# References

1. [[full joint probability distribution]]
2. [[random variable]]
3. [[joint probability]]
