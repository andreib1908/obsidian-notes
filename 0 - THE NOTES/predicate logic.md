---
type: topic
field: logic
field_type: predicate logic
short_desc: '"Using variables, connectives and quantifiers to reason what steps need to be taken. General notions and syntax."'
module: "6"
parent: main
---

20240122102
Status: #m6
Tags: [[logic]]


# What is predicate logic

![[Pasted image 20240101175427.png]]

- Predicates : 'Human' or 'Mother'
- Quantifiers : V or E
- Variables : 'x' or 'y'
- There is also a different modelling, where 'Mother' is a function. It's the 'Mother(x)'
# Syntax

![[Pasted image 20240101175932.png]]
![[Pasted image 20240101180044.png]]

So we have:
- constants
- predicates
- functions
- variables
- connectives
- equality
- quantifiers

And classifications, such as:
1. Atomic Sentence:
	- predicate(term1, ..., termN)
	- term1=term2
2. Term:
	- function(term1, ..., termK)
	- constant
	- variable
3. Examples:
	- Location(Wumpus, Square(1,3))
		- Here Square(1,3) is a function. Not in the mathematical sense, it just build another term.
		- Wumpus is a term.
	- North(Wumpus, Agent)

*I wrote these down again so I can search for these terms and find this note.*


![[Pasted image 20240101180616.png]]

- Complex Sentences:
	- "For all x it holds that if x passes AI, then x is smart."
	- "For all x it holds that if x is human, then there exists some y for which it holds that x loves y."

# Exercises

Exercise How do we model the sentence "All Students who take the course on AI are smart"?:
- My solution: (V) x Student(x) ^ AI(x) => Smart(x)
- Their solution:![[Pasted image 20240101181022.png]]

Exercise: How do we model the sentence "There is a student who takes AI and is smart."
- My solution: (E)x Student(x) ^ Takes(x, AI) ^ Smart (x)
- They had the same solution :)

![[Pasted image 20240101181336.png]]


# References

1. [[Predicates and Quantifiers]]
2. [[first order logic (FOPL)]]