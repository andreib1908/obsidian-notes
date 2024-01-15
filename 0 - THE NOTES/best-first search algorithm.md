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

# best-first search algorithm

In [[informed search strategies (heuristic)]], this is the general approach.

It's an instance of the [[search tree (graph)]].

The node is expanded based on an [[evaluation function]], f(n).

The node with the lowest cost is expanded first.

>[!information] The Heuristic Function
>Most Best-first search algorithms use a **heuristic** function *h(n)*:
>- h(n) = estimated cost of the cheapest path from the state at node n to goal state.
# References

1.  [[informed search strategies (heuristic)]]
2. [[search tree (graph)]]
3. [[heuristic function]]