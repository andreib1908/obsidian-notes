---
type: topic
field: math
field_type: probability
parent: 
short_desc: '"Probability of one event happening between two events A and B, but not both at the same time."'
module: 4, 6
---


202401082225
Status: #m6
Tags: [[math]] 

# disjunction probability

*disjunction* =
1. a lack of correspondence or consistency. 
	- "there is a **disjunction between** the skills taught in education and those demanded in the labour market"
2. LOGIC
	- the relation of two distinct alternatives.

One of two events, or [[random variable|RVs]], is occurring, but not both at the same time.
# Formulas

## General Formula

$$  P(A \space or \space B) = P(A) + P(B) - P(A, B) $$
## Deriving from 1 - opposite probability
$$P(A\space or \space !B) = 1 - P(!A \space or \space B)$$
## More complex conditions

$$P(Condition1,!Condition2) \lor (Condition3, Condition2)$$
# Example

![[Pasted image 20240108224908.png]]

## Example of the first two formulas

$$P(Headache = yes \space or \space Covid = no) = ?$$

### First solution
$$P(Headache = yes \space or \space Covid = no) = P(Headache=yes) + P(Covid=no) - P(Headache=yes, Covid=no)$$
$$P(Headache=yes) = 0.25 + 0.12 + 0.05+0.05 = 0.47$$
$$P(Covid=no) = 0.12+0,05+0.10+0.32=0.59$$
$$P(Headache = yes,Covid = no) = 0.12 + 0.05 = 0.17$$
$$=> P(Headache = yes \space or \space Covid = no) = 0.47 + 0.59 - 0.17 = 0.89$$
### Second solution

$$P(Headache \space or \space !Covid) = 1 - P(!Headache, Covid)$$

## Example of the more complex formula
![[Pasted image 20240108230759.png]]
$$P(headache, \lnot covid) \lor (fever,covid) = 0.25+0.12+0.05+0.10=0.52$$

Here we selected all the probabilities of the rows that passed either the first part of the condition, which is $(headache, \lnot covid)$, or the second part $(fever, covid)$, based on the logical $\lor$ operator. You can see them highlighted in red.

# References

1.  [[full joint probability distribution]]
2. [[random variable]]
3. [[Propositions and Truth Values]]

