---
type: topic
field: logic
short_desc: "\"In trees and graphs, it's the shortest possible distance from the initial state to the end state.\""
field_type: search logic
module: "6"
parent: "[[a star search algorithm]]"
---

20240122102
Status: #m6
Tags: [[logic]]

>[!TLDR] Why are heuristic functions useful?
>A good heuristic function can reduce the space and time complexity dramatically!

# heuristic function

Usually denoted by `h(n)`. 

The heuristic function refers to the estimated cost of the cheapest path from the state at node n to goal state.

# admissible heuristic function

>[!tldr] Admissible
>- The function `h` never overestimates the cost, i.e. `h` is an optimistic estimate.
>- [[search tree (graph)|tree search]] is [[optimality|optimal]] if `h` is admissible.
>- [[graph search]] is [[optimality|optimal]] if `h` is consistent (aka *monotonic*).

# consistent heuristic function
 
>[!tldr] Consistent
>- `h(n) <= cost(n, a, n') + h(n')` with `n'` being the *one-step successor of n* ([[triangle inequality]])
>- ![[Pasted image 20240104175258.png]]
>- [[graph search]] is [[optimality|optimal]] if `h` is consistent (aka *monotonic*).
# References

1. [[initial state]]
2. [[goal state]]
3. [[a star search algorithm]]
4. [[search tree (graph)]]
5. [[graph search]]
6. [[optimality]]
7. [[triangle inequality]]
