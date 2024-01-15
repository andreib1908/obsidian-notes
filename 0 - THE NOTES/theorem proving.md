---
type: topic
field: logic
field_type: theorem proving logic
short_desc: '"Entailment, modus ponens, unit resolution rule and so on. The steps to prove a theorem."'
module: "6"
parent: main
---

20240121633
Status: #m6
Tags: [[logic]]

# Important distinction |= vs |-

![[Pasted image 20240102163546.png]]

# Proof by resolution in Propositional Logic

*KB |- Alpha* = 'Alpha follows from KB.'

![[Pasted image 20231120225518.png]]

>[!important] The Falsum / 'Empty' Clause
>![[Pasted image 20240101155525.png]] 
>This thing is called the *FALSUM*, also known as *THE EMPTY CLAUSE*. It's when you have a step like *Empty(2,3)*. If you reach that step through contradiction you basically proved that the sentence Alpha follows from the set of true sentences KB.

>[!todo] Steps to prove a theorem
>1. Add *not alpha* and aim to prove through contradiction that *not alpha* in relation to *KB* will lead to an *Empty Clause*.
>2. Rewrite Knowledge Base (KB) in CNF: [[CNF Conjunctive Normal Form]]
>3. https://utwente.yuja.com/V/Video?v=511711&node=2298714&a=151328799 -> go to 12:00 for the rest of explanation on how to prove (really useful). Basically just use the [[resolution rule]].

You really have to go through each step slowly, as they are all important.


>[!success] Sound Proof
>The proof is considered **sound** if it is proven by resolution that Alpha follows from KB, then KB |= Alpha.

>[!success] Complete Proof
>If KB |= Alpha then it can be proven by resolution that Alpha follows from KB.


# Proof by resolution for Predicate Logic

![[Pasted image 20240102162951.png]]

It's pretty much the same mechanism as in propositional logic, but there are a couple of weird things you need to keep track of. It's especially tricky to use [[skolemization]], but necessary. 

You should watch the video (13 minutes, but it's worth it): https://utwente.yuja.com/V/Video?v=511811&node=2298827&a=1897260479

>[!success] Sound Proof
>The proof is considered **sound** if it is proven by resolution that Alpha follows from KB, then KB |= Alpha.

>[!success] Refutation-Complete Proof
>If KB |= Alpha then it can be proven by resolution that Alpha follows from KB. Resolution cannot be used to generate all logical consequences of a set of sentences.


# References

Notes/Topics:
[[modus ponens]]
[[resolution rule]]
[[CNF Conjunctive Normal Form]]

Video for theorem proving in [[theorem proving#How to prove KB - Alpha|propositional logic]]:
https://utwente.yuja.com/V/Video?v=511711&node=2298714&a=151328799

Video for theorem proving in [[theorem proving#Proof by resolution for Predicate Logic|predicate logic]]:
https://utwente.yuja.com/V/Video?v=511811&node=2298827&a=1897260479

Use: 
[[logic rules cheat sheet]]