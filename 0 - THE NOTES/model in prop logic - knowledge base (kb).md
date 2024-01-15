---
type: topic
module: "6"
field: logic
field_type: propositional logic
short_desc: '"Also known as knowledge base (KB). Through linear separation, determine what category data points will fall under with logic."'
main_topic: "[[machine learning]]"
parent: main
---
20240122102
Status: #m6
Tags: [[logic]]

# model in prop logic - knowledge base (kb)

Abstract representations about the world. Also known as **knowledge base (KB)**.

![[Pasted image 20231231153217.png]]

![[Pasted image 20231230171645.png]]

![[Pasted image 20240101143746.png]]

-> Basically, a given set of true rules.


![[Pasted image 20240101144200.png]]


![[Pasted image 20240101145413.png]]

In this example:
- M(p) = {(**p is true**, q is true), (**p is true**, q is false)}
- M(q) = {(p is true, **q is true**), (p is false, **q is true**)}
- M(p^q) = {(**p is true**, **q is true**)}
- M(q^p) = {(**p is true**, **q is true**)}
- Also, the statements p^q and q^p are [[logical equivalence|logically equivalent (l.e.)]] because M(p^q) = M(q^p).

> **A MODEL REFERS ONLY TO TRUE VALUES. THAT IS WHY A MODEL WITH NO TRUE VALUES IS NULL.**
> ![[Pasted image 20240101150425.png]]

# References

1. 
