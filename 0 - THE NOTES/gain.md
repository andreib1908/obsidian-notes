---
type: topic
field: AI
short_desc: '"A note related to artificial intelligence concepts."'
field_type: AI + logic
module: "6"
parent: "[[information gain]]"
---



202401111814
Status: #m6
Tags: [[AI]]

# gain

[[information gain]]

# Formula

$$Gain(S,A)=Entropy(S)-\sum\limits_{v\in A} \frac {\lvert S_{v} \rvert} {\lvert S \rvert } * Entropy(S_{v})$$
# Examples

![[Pasted image 20240111181855.png]]

Now we have to split the dataset into only the values that have a $yes$ in fever.

![[Pasted image 20240111181949.png]]

![[Pasted image 20240111182003.png]]

- 5/20 is because we have 5 rows with fever yes out of 20 overall rows
- -3/5 because we have 3 rows in our 5 rows that are covid yes
- -2/5 same reasoning for covid no

![[Pasted image 20240111182157.png]]

This is if we want to calculate the entropy for fever no.

![[Pasted image 20240111182237.png]]

We go back to the formula and we calculate the gain.
# References

1. [[information gain]]
2. [[entropy]]