---
type: topic
field: logic
short_desc: '"The collection of states that an AI agent can reach in path finding starting from the initial state."'
field_type: search logic
module: "6"
parent: "[[solution finding]]"
---
20240122102
Status: #m6
Tags: [[logic]]

# search space

Set of all states reachable from the initial state by any sequence of action.

![[Pasted image 20240104180308.png]]

This is an example taken from [[a star search algorithm]]. The search space here is the matrix of all white and black squares, while the red rectangle just refers to how the A* algorithm restricted the search space. For this note, just overlook the red rectangle.
# sound search space

A search space is considered **sound** if every path in the abstract search space corresponds to a path in the real environment.
# complete search space

A search space is considered **complete** if every path in the real environment corresponds to a path in the abstract search space.

# References

1. [[solution finding]]
2. [[initial state]]
3. [[a star search algorithm]]
4. [[search tree (graph)]]
5. [[graph search]]
