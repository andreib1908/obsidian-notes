---
type: topic
field: AI
short_desc: '"A note related to artificial intelligence concepts."'
field_type: AI + logic
module: "6"
parent: "[[path finding]]"
---

20240122101
Status: #m6
Tags: [[AI]]

# problem formulation

- The process of deciding what actions and states to consider, given a goal.

>[!TLDR] Initial state
>It's the position of the [[agent]] at start:
>- ln(A)

>[!TLDR] Actions
>The possible actions available to the agent:
>- ln(A), {Go(X), Go(Y), Go(Z)}

>[!TLDR] Transition model
>What each action does:
>- RESULT(ln(A), Go(X)) = ln(X)

>[!TLDR] Goal test
>Tests if a given state is the goal state.

>[!TLDR] Path cost
>Assigns a numbers cost to each path.


# References

1. [[path finding]]
2. [[goal-based agent]]
3. [[solution finding]]