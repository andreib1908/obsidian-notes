---
type: topic
field: logic
field_type: theorem proving logic
short_desc: "\"The form we must bring a sentence to. It's step number 2 in theorem proving (the KB |- Alpha thing).\""
module: "6"
parent: "[[theorem proving]]"
---
20240122102
Status: #m6
Tags: [[logic]]

# CNF in Propositional Logic

![[Pasted image 20231120225704.png]]

It is a conjunction of disjunctions.

![[Pasted image 20231120225756.png]]
**IMPLICATIONS ARE NOT ALLOWED IN CNF**

# CNF in Predicate Logic

![[Pasted image 20240101210704.png]]
![[Pasted image 20240101210724.png]]

The removal of quantifiers then requires [[skolemization]].

Then every remaining variable is universally quantified  
• Thus, universal quantifiers can be dropped,  i.e., formulas become implicitly universally quantified  
– Also for rules in Prolog!

# References

1. [[prolog]]
2. [[theorem proving]]
3. [[Propositions and Truth Values]]
4. [[Predicates and Quantifiers]]