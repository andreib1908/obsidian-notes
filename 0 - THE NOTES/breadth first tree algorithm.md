---
type: topic
field: computer science
short_desc: '"An algorithm for tree data structures where we first expand on descendants, layer by layer."'
field_type: search logic
module: "6"
parent: "[[search tree (graph)]]"
---

20240122102
Status: #m6
Tags: [[logic]]

![[Breadth First Algorithm GIF.gif]]
# breadth first algorithm

First the root node is expanded, then all their successors and then their successors and so on.

It looks something like:
1. Find root node a
2. Check node a, find nodes b and c
3. Check node b, find nodes d and e
4. Check node c, find nodes f and g
5. Check node d
6. Check node e, find node b
7. Check node f
8. Check node g
9. Check node h

>[!TLDR] TLDR
>We expand layer by layer.


# References

1. [[search tree (graph)]]
