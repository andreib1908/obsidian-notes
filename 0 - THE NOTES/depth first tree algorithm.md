---
type: topic
field: computer science
short_desc: '"An algorithm for tree data structures where we first expand on descendants, but not layer by layer. We go as deep as possible with each descendent."'
field_type: search logic
module: "6"
parent: "[[search tree (graph)]]"
---

20240122102
Status: #m6
Tags: [[logic]]

![[Depth First Tree Algorithm GIF.gif]]

# depth first tree algorithm


From the root node, we expand the first descendent. Then we expand each descendent of that descendent, and only then, when we reach the bottom leaf node, we return to the second descendent of the root node and proceed.

It looks something like:
1. Check 1
2. Check 2
3. Check 3
4. Check 4
5. Check 5
6. Check 6
7. Check 7
8. Check 8
9. Check 9
10. Check 10

>[!TLDR] TLDR
>- We go as far down as possible.
>- First we check the left-most descendent, and then right-most.



# References

1. [[search tree (graph)]]
