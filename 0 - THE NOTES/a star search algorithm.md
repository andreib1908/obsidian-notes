---
type: topic
field: computer science
short_desc: '"An algorithm for tree data structures where the node with the lowest cost is expanded first."'
field_type: search logic
module: "6"
parent: "[[informed search strategies (heuristic)]]"
---

20240122102
Status: #m6
Tags: [[logic]]

>[!TLDR] TLDR - The A* search algorithm
>- **Formula:** $f(n) = g(n) + h(n)$
>- **Algorithm**: Choose the next node that has the smallest f(n).

>[!warning] A Star Search Requirements
>- Environment should be fully observable and static.
>- [[search space|Search space]] modelling should be both [[search space#sound search space|sound]] and [[search space#complete search space|complete]].

>[!tldr] A* Search Terminology - Completeness
>- A* Search is complete when it always finds a solution, if there is one.

>[!TLDR] A Star Search Terminology - Commitment
>A Star Search is an example of [[blind commitment]]. The plan (route) is not updated during the execution. For instance, traffic jam info or moving obstacles are not taken into account.

# 'a star' search algorithm

Also written as 'A* search'.

Let `n` be the node we are trying to evaluate. Relevant to this algorithm are the following three functions:
1. `g(n)` -> The cost to reach the node `n` from the [[initial state|start state]]
2. `h(n)` -> the *estimated* cost to get from the node `n` to the [[goal state|goal]]. h(n) is also called [[heuristic function|a heuristic]].
3. `f(n)` -> The function of the A* algorithm. It is the estimated cost of the cheapest solution through `n`. 

>[!TLDR] The A* search algorithm
>- **Formula:** f(n) = g(n) + h(n)
>- **Algorithm**: Choose the next node that has the smallest f(n).

![[Pasted image 20240103153237.png]]

# Example

![[Pasted image 20240103153946.png]]

[[manhattan distance]]

- `(2,2)` has a g(n) = 0 and h(n) = 4 (the path (3,2), (4,2), (4,3), (4,4)) so f((2,2)) = 0 + 4 = 4
- `(1,2)` has g(n) = 1 (it's one node away from start) and h(n) = 5 ((2,2), (3,2), (4,2), (4,3), (4,4)) so f((1,2)) = 1 + 5 = 6
- and so on...

![[Pasted image 20240104173612.png]]

>[!tldr] TLDR
>We always want to expand the lowest cost node first, and choose it as well.


>[!tldr] Conclusion
>- The A* algorithm reduces search space (we limit ourselves to the red rectangle below in our example).
>- The effectiveness of the algorithm depends on how we choose our heuristic function h(n).

![[Pasted image 20240104173905.png]]

## Another example

![[Pasted image 20240104174222.png]]

Apparently, there's a guy who solved this on github:
https://github.com/kevinrosalesdev/Searching-Algorithms
# References

Notes:
1. [[informed search strategies (heuristic)]]
2. [[search space]]
3. [[initial state]]
4. [[goal state]]
5. [[heuristic function]]

Video explanation (not the best but it's good enough):
https://utwente.yuja.com/V/Video?v=511819&node=2298835&a=2013541133 

Github guy:
https://github.com/kevinrosalesdev/Searching-Algorithms