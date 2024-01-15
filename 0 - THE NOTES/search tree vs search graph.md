---
type: topic
field: logic
short_desc: '"A note related to logic."'
field_type: search logic
module: "6"
parent: "[[search tree (graph)]]"
---
20240122102
Status: #m6
Tags: [[logic]], [[comparisson]], [[tree]], [[graph]]

# search tree vs search graph

![[Pasted image 20240103132834.png]]

`BFS` = [[breadth first tree algorithm]]
`DFS` = [[depth first tree algorithm]]

The main difference between *tree search* and *graph search* lies in the use of a [[searching example from start to goal#Second approach - Utilizing a Depth First Search Algorithm|closed list]].

>[!success] Benefits of a closed list
>1. **Search Efficiency:** Prevents expanding states that were expanded before. No duplicates.
>2. Prevents searching in loops

>[!failure] Main drawback of a closed list
>Requires more memory due to bookkeeping.

# Using tree search (no closed list) over graph search

When the problem (the action space or [[search space]]) is tree-shaped, no loops occur in the problem specification, so we can use tree search.

>[!note] Note for my Romanian homies
>Tree search este folosit pentru grafuri neorientate (arbori) si graph search este folosit pentru grafuri orientate.

# References

1. [[breadth first tree algorithm]]
2. [[depth first tree algorithm]]
3. [[searching example from start to goal#Second approach - Utilizing a Depth First Search Algorithm|closed list]]
4. [[search space]]