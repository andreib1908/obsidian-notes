---
type: topic
module: "6"
field: logic
field_type: predicate logic
short_desc: "\"The set of true rules that use quantifiers or predicates such as 'Student(x).\""
main_topic: "[[predicate logic]]"
parent: "[[model in prop logic - knowledge base (kb)]]"
---
20240122102
Status: #m6
Tags: [[logic]]

# Syntax and definitions

Models contain:
- **Objects** - domain elements
- **Relations** among them.

Interpretation maps syntax to elements in the semantic domain, specifying referents for:
> **constant symbols** -> *objects*
> **predicate symbols** -> *relations*
> **function symbols** -> *functional relations*

*'->' means 'mapped to'*

![[Pasted image 20240101182451.png]]

## Example

[[wumpus world]]
![[Pasted image 20240101182714.png]]
> The domain of interpretation refers to the outside world.


# Semantics of Quantifiers

![[Pasted image 20240101183410.png]]

So, if we had a list like `[boy1, boy2, boy3]` and a model `m = 'plays soccer'`, then for `(V)x P(x)` to be true in `m`, then all three boys must play soccer. You get the idea for the existential one too.

## Example

![[Pasted image 20240101183659.png]]

So here all we're really saying is that we can replace the `x` with any individual part of our knowledge base (model). 

In the previous example of syntax, we mapped `wumpus` to `Wumpus`:
![[Pasted image 20240101183837.png]]

And so, we can replace `x`.

# References

1. [[model in prop logic - knowledge base (kb)]]
2. [[predicate logic]]
