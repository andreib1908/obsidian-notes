---
type: topic
module: "6"
field: logic
field_type: predicate logic
short_desc: '"Substituting variables within our predicate terms."'
parent: "[[model in predicate logic]]"
---
20240122102
Status: #m6
Tags: [[logic]]

# The Unification Mechanism

If you have the two predicates:
- `Knows(John, x)`
- `Knows(John, Jane)`

They are not the same but they can be made the same if we substitute `Jane` for `x`. This is called **unification**.

![[Pasted image 20240101184430.png]]

![[Pasted image 20240101192927.png]]

![[Pasted image 20240101193105.png]]

[[most general unifier (mgu)]]

# Unification with functions. Occurs Check.

`Loves(x, S(x))` and `Loves(y,z)` can be unified:
-> `{y/x, z/S(x)}`
-> And you get the unified [[literal]] `Loves(x,S(x))`.

There is a problem with `Loves(x,S(x))` and `Loves(y,y)`. This unification fails because in general `x != S(x)`.

![[Pasted image 20240101193930.png]]

So basically they just want to say that if the function passes the **occurs check**, only then the unification can be carried out.

# References

1. [[modus ponens]]
2. [[resolution rule]]
3. [[predicate logic]]
4. [[model in predicate logic]]
5. [[most general unifier (mgu)]]