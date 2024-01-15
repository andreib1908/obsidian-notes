---
type: topic
field: AI
short_desc: '"A note related to artificial intelligence concepts."'
field_type: probabilistic reasoning
module: "6"
parent: "[[bayesian network]]"
---


202401102224
Status: #m6
Tags: [[AI]]

# independence in bayesian networks

Determining (conditional) independences in the factorization of a [[full joint probability distribution]] is not easy.

Independence of nodes in a [[graph]] can be found mechanically by operations on the [[graph]].

For the set of nodes $A$, $B$, $C$:
>[!success] Notation 
>$$A \perp B | C$$
>if all the paths from $A$ to $B$ are [[independence in bayesian networks#When is a path blocked?|blocked]].

>[!note] Note
>In the context of independence, the symbol $\perp$ means independence. So in the formula above we mean that the node in $A$ *"is independent"* of the node in $B$, *"given the value in $C$"*.

# Types of nodes related to dependence

![[Pasted image 20240110223507.png]]
## Sequential

![[Pasted image 20240110223452.png]]

Sequential ($W=A$ in the case of the big graph):
- A is intermediary between cause $E$ an effect $C$

## Divergent

![[Pasted image 20240110223637.png]]

Divergent($W=E$):
- $E$ is common cause of the effects $R$ and $A$

## Convergent

![[Pasted image 20240110223738.png]]

Convergent($W=A$):
- A is common effect of causes $E$ and $B$.

# When is a path blocked? d-separation

![[Pasted image 20240110224512.png]]

# Examples

![[Pasted image 20240110224522.png]]
# References

1. [[bayesian network]]
2. [[conditional probability]]
3. [[conditional probability table]]
4. [[probability product rule (chain rule)]]
5. [[independence rv]]