---
type: topic
field: AI
field_type: AI + logic
short_desc: '"An example of an AI agent within a simulated environment."'
module: "6"
parent: main
---

20240122101
Status: #m6
Tags: [[AI]]

# wumpus world

**Goal:**
– Agent should find the gold, and climb out of the  
Wumpus cave with the gold  
– Avoid pits (it cannot get out anymore), avoid  
Wumpus (it will get eaten)  
– Use as few actions as possible

**Environment Type**  
– Discrete: finite number of distinct states and  
actions  
– Static: no changes in the evironment during the  
game (except by the agent),  
– “Single agent”: Wumpus does not move  
– Partially observable: agent only perceives what is in  
its own square, does not have full knowledge of  
the environment at the start

**[[actuator|Actuators]]:**
– Forward; move one square forward in direction the  
agent faces if no wall in front, otherwise stay put  
– TurnLeft, TurnRight; turn direction the agent is facing  
– Grab; pick up the gold when on gold square.  
– Shoot; fire arrow in direction the agent is facing,  
either hits (and kills) Wumpus or hits wall; only one  
arrow. Wumpus does not move!  
– Climb, to climb out of the wumpus cave, only from  
square [1,1].

**[[sensor|Sensors:]]**  
– Stench, in squares adjacent (not  
diagonal) to the wumpus there is stench.  
– Breeze, squares adjacent to a pit will have a  
Breeze.  
– Glitter, on the square with gold the agent will  
perceive a glitter.  
– Bump, when hitting the wall.  
– Scream, when the wumpus is killed.  
Transmitted to agent as list of five items, e.g.,  
[Stench, none, Glitter, none, none]

![[Pasted image 20231231144403.png]]

# References

1. 