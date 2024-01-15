---
type: topic
field: logic
short_desc: '"A note related to logic."'
field_type: search logic
module: "6"
parent: "[[search strategy]]"
---


20240122102
Status: #m6
Tags: [[logic]], [[tree]], [[graph]]

# Abstract datatype for Environment

Consider the following environment in which an [[agent]] has to go from 'Start' to the 'Goal' and it has some obstacles in the middle. The agent would like to go in an [[optimality|optimal]] way by picking the shortest path (lowest [[path cost]], if we say that each square has a cost of 1).

![[Pasted image 20240103114411.png]]

The components of our environment are as follows:
1. Matrix E of size 5x5:
	1. E(i,j) = 0 means 'free cell'
	2. E(i,j) = 2 means 'obstacle'
	3. E(i,j) = 1 means 'agent is in cell (i,j)'
2. For the current state of the environment E(i,j) = 0 for all i,j except:
	1. E(3,2) = E(3,3) = E(3,4) = 2 i.e. 'the obstacles'

[[action of agent|Actions]]: left, down, right, up

Design decision: is action left allowed in In(1,3)? If yes what is the effect? 

Action left applicable in In(i,j) with i>1 except for (i,j) in {(4,2),(4,3),(4,4)}.

Action down applicable in In(i,j) with j>1 except for (i,j) in {(3,5)}. 

Action right applicable in In(i,j) with i<5 except for (i,j) in {(2,2),(2,3),(2,4)}. 

Action up applicable in In(i,j) with j<5 except for (i,j) in {(3,1)}.

Additional info: Goal state In(4,4) and Initial state In(2,2).

# Organize the data into a graphical representation

![[Pasted image 20240103115028.png]]

- 2 axis world
- 4 possible [[action of agent|actions]]: left, down, right, up

- [[initial state|initial state]] is (2,2)
- [[goal state]] is (4,4)

# First approach - Utilizing the Breadth First Search Algorithm

First, initialize frontier using start/initial node (node corresponding to initial state:

frontier=`[((2,2),Xx)]` 

Loop based on [[breadth first tree algorithm]]:
1. If `frontier=[]` then return failure 
2. Remove head node n from frontier 
3. If n contains goal state then return solution 
4. Expand n, add resulting nodes to the tail of the frontier 18 

Xx: Additional node info depending on search strategy

![[Pasted image 20240103115424.png]]

>[!note] Note
>We remove the node we processed. In this step, we removed the node (2,2) from the frontier queue.


![[Pasted image 20240103115433.png]]

![[Pasted image 20240103115445.png]]

And so on until you find your goal.

![[Pasted image 20240103115509.png]]

You will construct a tree that looks like this, since we added each new node at the end of our queue. This is the [[first in first out (FIFO) queue]].

>[!failure] Problems with this approach
>1. We have repeated states in our tree, like (2,2).
>2. This is an uninformed search strategy. The information regarding the goal state being in the cell (4,4) was not used at all.
>3. Could lead to an infinite loop.


![[Pasted image 20240103120007.png]]

Therefore, we have to find a solution for repeated states.

# Second approach - Utilizing a Depth First Search Algorithm

First, initialize the closed list and frontier using initial state:
- frontier = `[((2,2), xx)]`
- closed = `[]`

>[!note] Note
>We use the closed list to keep track of already processed nodes. It's a form of book-keeping.

Loop, based on the [[depth first tree algorithm]]:
1. If `frontier =[]` then return failure
2. Remove head node *n* from frontier and add corresponding state to closed
3. If *n* contains goal state then return solution
4. Expand *n*, add resulting nodes to the head of the frontier if the state is not in frontier and not in closed.

xx: Additional info depending on search strategy.

![[Pasted image 20240103130705.png]]

The steps look like this:
1. `frontier[]; closed = []`
2. `frontier[((2,2), xx)]; closed = []`
3. `frontier[((1,2), xx), ((2,1) ,xx), ((2,3), xx)]; closed = [((2,2), xx)]`. Now we go as far as possible down the tree, left-most.
4. `frontier[((1,1), xx), ((1,3), xx)]; closed = [((2,2), xx), ((2,1), xx), ((2,3), xx)]`
5. `frontier[((1,3), xx)], closed = [((2,2), xx), ((2,1), xx), ((2,3), xx), ((1,1), xx)]`
6. `frontier[((1,4), xx)], closed = [((2,2), xx), ((2,1), xx), ((2,3), xx), ((1,1), xx), ((1,3), xx)]`
7. `frontier[((2,4), xx), ((1,5), xx)], closed = [((2,2), xx), ((2,1), xx), ((2,3), xx), ((1,1), xx), ((1,4), xx)]`
8. and so on...

>[!note] Note
>- Here, when we reached (1,1) we went back one step above to (1,2) and then we went down again towards (1,3).
>- We didn't go to (2,1) as the second picture below illustrates because (2,1) had already been placed into the closed list after we went down one level after (2,2).
>- Same explanation to why from (1,2) we went into (1,3) instead of (2,2).

![[Pasted image 20240103131629.png]]
![[Pasted image 20240103131637.png]]

**THE RESULTING PATH AND TREE**
![[Pasted image 20240103131926.png]]

>[!failure] Still, this is not the most optimal path-finding algorithm
>![[Pasted image 20240103132035.png]]
>As humans, we can see that it would have been much more efficient to go into (2,1), then (3,1), and finally (4,1).

# Example where you could do both DFS and BFS

![[Pasted image 20240103150217.png]]

# References

1. [[agent]]
2. [[optimality]]
3. [[path cost]]
4. [[action of agent]]
5. [[initial state]]
6. [[goal state]]
7. [[breadth first tree algorithm]]
8. [[first in first out (FIFO) queue]]
9. [[depth first tree algorithm]]