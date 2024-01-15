---
type: topic
field: math
field_type: probability
parent: "[[conditional probability]]"
short_desc: "\"When two random variables have outcomes that are not dependent on each other. This note also goes over conditional independence, which is crucial for Bayesian Networks and reducing full joint probability tables' complexity.\""
module: 4, 6
---
202401100233
Status: #m6
Tags: [[math]] 

# independence rv

[[random variable|Random variables]] A and B are said to be **independent** if they fulfil any of the properties:
$$P(A|B)=P(A)$$
$$P(B|A)=P(B)$$
$$P(A,B)=P(A)*P(B)$$
$$P(A,B)=P(A|B)*P(B) = P(A)*P(B)$$
*We derived the second to last one based on the last one.*

# conditional independence

>[!success] Main conclusion the examples will be based on:
>When we have around three [[random variable|RVs]] and one of the is Boolean, we can say that the two other random variables are dependent (the red line) on each other **when the Boolean variable is not yet known**. Once we know the value of the Boolean, then the two other variables become independent, as we only look at the Boolean variable to determine the probability of each random variable.
>![[Pasted image 20240110153354.png]]
>![[Pasted image 20240110153319.png]]
>- We can say that for the relation $P(A|B,C) = P(A|C)$ that $A$ and $B$ are **conditionally independent on $C$** (because either $A$ and $B$ are dependent when we don't know $C$, or they are **independent** once we know $C$). ![[Pasted image 20240110153801.png]]


>[!TLDR] Three random variables in our probability with independence in mind
>![[Pasted image 20240110154019.png]]
>Here we applied the [[probability product rule (chain rule)#Chain Rule|chain rule]] to extend the probabilities.
>Then, we used the fact that in this scenario, $A$ and $B$ are **conditionally independent on C**, and therefore we can remove $B$ in the second $=$ for the $P(A|B,C)$.
>This is very useful in [[full joint probability distribution]], where we have a bunch of [[random variable|RVs]]

>[!TLDR] Why exactly is independence useful in full joint distributions?
>Because we can reduce the number of rows in our [[full joint probability distribution]] table, reducing its complexity by a significant amount:
>![[Pasted image 20240110154449.png]]
>Where they say 2 + 2 + 1 = 5, they refer to 2 rows + 2 rows +1 row = 5 total rows. So parameters here means "rows".
### Coin toss example to illustrate the point

Let's consider the example of two people, Alice (noted by $A$) and Bob (noted by $B$), tossing a coin that can have two values: HEAD ($H$) or TAIL ($T$). 

We are suspecting that the dice may be biased towards always resulting in $H$. In this case, we can say that the two events, Alice's toss ($A$) and Bob's toss ($B$) are **DEPENDENT** (not independent). 

This is because if we see that $A$ results in $H$, then it is highly likely that $B$ will also result in an $H$, since we suspect that the coin is biased towards $H$.

So, we can write this relation as follows:

$P(B=H|A=H)>P(B=H)$

This is **dependence**. If $B$ rolled by himself before $A$, then we wouldn't have a reference point for our suspicion and so the probability of $B$ being $H$ will be smaller than once we know that $A$ got an $H$. 

### Introducing a Boolean variable C

We can also introduce a third [[random variable]], $C$, that represents the statement *the coin is biased towards heads*. It can have two values: $TRUE$ or $FALSE$.

In the beginning, before $A$ happened, we can conclude that $A$ and $B$ are dependent on each other because we cannot give $C$ a value just yet.

![[Pasted image 20240110152352.png]]

The red line represents the relation that $A$ and $B$ are **dependent**.

So, at this initial point, the probability of $B$ can be written as:
$P(B|C) = P(B|A,C)$

So, we can gather information from $A$ and determine the value of $C$ in order to determine $B$. Once we know that $A$ lands on $H$, then we can give $C$ the value $TRUE$ and safely disregard $A$ from calculating the probability of $B$ being $H$.

This is because we have already concluded that the coin is biased towards heads.

After this, even if $A$ lands on $HEADS$ or $TAILS$, nothing will change my belief that the coin is biased towards head. Therefore, at this stage when we know that $C$ is $TRUE$, the random variables $A$ and $B$ are **independent**.

![[Pasted image 20240110152906.png]]

So at this point, our $P(B|C) \not = P(B|A,C)$ -> we just eliminate the A.
# Examples
![[Pasted image 20240110023822.png]]
# References

1. [[joint probability]]
2. [[conditional probability]]
3. [[probability product rule (chain rule)]]
4. [[full joint probability distribution]]
5. [[random variable]]
6. [[bayesian networks]]
