---
type: topic
field: logic
field_type: theorem proving logic
module: "6"
short_desc: "\"It's a rule used to eliminate opposite literals of two disjuncts. For example, we have p v q; not q, therefore we eliminate q and get p.\""
parent: main
---

20240121615
Status: #m6 
Tags: [[logic]]

# The Unit Resolution Rule

The main idea is that you eliminate opposite literals of two disjuncts.

![[Pasted image 20231120220111.png]]

Here we are saying that:
- We are looking at *p V q* and we know it is **true** (or that "it is the case")
- We also know that *not q* is also **true**
- We can deduce then that *p* is **true**, or *p "is the case"*.

In the example we say that one morning *we want to have either tea or coffee*. However, we want to go on an insane caffeine break, so we impose a rule on ourselves that **is always true**, which is (*not coffee* is **true**). So, because we need the caffeine break and we want to drink something that morning, the only logical conclusion is that *we must have tea*, or that *tea is true*/*tea 'is the case'*.

# General Resolution Rule

More complex version of what is above. Same logic applies.

![[Pasted image 20231120220547.png]]

![[Pasted image 20231120220859.png]]

Here they just say that given the resolution rule and we know that we have a pair of disjunct literals, which is *li = not mj* or *not li = mj*, then **we cancel those literals out**. That's why you see *l1 or ... or li-1 or li+1... or mj-1 or mj+1* instead of *l1 or ... or li-1 or **li** or li+1... or mj-1 or **mj** or mj+1*, so without *li* and *mj* because they got canceled out.


![[Pasted image 20231120225300.png]]

But the resolution rule only works with CNF:

![[Pasted image 20231120225320.png]]

# Resolution Rule in Predicate Logic

![[Pasted image 20240101210441.png]]

![[Pasted image 20240102162916.png]]

So if the [[literal|literals]] are exactly the same, you just remove them from your list or whatever.

You need to work with these to understand them: [[Predicate logic - Batch 1 Lecture 2]]
# References
[[modus ponens]]
[[theorem proving]]
[[Propositions and Truth Values]]
[[predicate logic]]

