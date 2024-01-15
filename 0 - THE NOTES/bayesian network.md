---
type: topic
field: AI
short_desc: '"A way to encode probability distributions."'
field_type: probabilistic reasoning
module: "6"
parent: main
---


202401101634
Status: #m6
Tags: [[AI]]

# bayesian network

It's a way of representing the [[full joint probability distribution|probability distribution]]. It is a way of encoding the knowledge that we have in a way that a computer can analyze.

The Bayesian networks are, thus, a simple graphical notation for [[independence rv#conditional independence|conditional independence]] assertions and hence for compact specification of [[full joint probability distribution|full joint probability distributions]].

The structure of this network tells us the relation among nodes. Each node represents a variable that can either be $TRUE$ or $FALSE$. So they are **Boolean random variables**.

Make sure to also look at the examples because you really learn how to work with them along with the [[probability product rule (chain rule)|chain rule]].
# Syntax

A mathematical [[graph]]:
- **Nodes** = [[random variable|random variables]]
- **Edges** = form a directed, acyclic [[graph]] (there are no loops in the graph) indicating how different variables are related. Usually they represent causality. A change in a variable typically influents another variable.
- A conditional distribution for each node given it's parents: $P(X_i|Parents(X_i))$
- Usually, a table ([[conditional probability table]]) gives the distribution over $X_i$ for every combination. This table is usually provided.

![[Pasted image 20240110203858.png]]

>[!note] Note
>Remember that [[marginal probability|marginalization]] means just not accounting for a variable in a [[joint probability]].
# Notation

![[Pasted image 20240110163752.png]]

The joint probability distribution here:
$P(L, R, W)$, for $L$ = Win Lottery, $R$ = Rain, $W$ = Wet Ground.

Given this graph:
$P(L,R,W) = P(L)P(R)P(W|R)$

So $L$ has no connection with $R$ or $W$ and it is reflected by our equation. Look at the arrow.

![[Pasted image 20240110164302.png]]

If we add another variable $S$, then our equation will look like:
$$P(L,R,W,S) = P(L)*P(R)*P(W|R)*P(S|W)$$
> [!note] Note on Independence
> - We can see that $L$ and $R$ are the [[independence rv|independent]] [[random variable|random variables]]
> - And that $W$ and $S$ are **dependent** variables.

# Motivation

**Modelling** direct relationships is crucial:
- It reduces the number of parameters (rows) in the model.
- Simplifies reasoning.

Relationships between variables will remain complex, and critical: we have many unknowns which are all (indirectly) dependent on each other.

Bayesian Networks are used for:
- reasoning under uncertainty
- modelling large [[full joint probability distribution]]
- reasoning with such networks.

# Independence in Bayesian Networks

Because this note is already huge, refer to this note for more information:
[[independence in bayesian networks]].

# Examples

## General Example

![[Pasted image 20240110164712.png]]

## How a larger network would look like

![[Pasted image 20240110164852.png]]

## Example of a Bayesian network in natural language

![[Pasted image 20240110204226.png]]

## The Earthquake Example - Burglary if Alarm

### Modelling

![[Pasted image 20240110204718.png]]

Look at the probabilities for having an earthquake and for being a victim of burglary. They are 0.001 (1 in 1000) and 0.02 (2 in 100). **You don't need to store the probabilities for $\lnot e$ and for $\lnot b$ because you can just do "1 - the respective probability" to infer them.** 

This applies to the last two rows, for example, because they are complimentary. So, you don't really need to store both of them, just one of them. Could apply to other probabilities too.

That table over there is the [[conditional probability table]].

![[Pasted image 20240110205609.png]]

This is the [[conditional probability#Bayes' Theorem|Bayes' Formula]]. We have to find $P(b,a)$ first, which can be calculated with the [[probability product rule (chain rule)#Chain Rule|chain rule]].
### Step 1 - Calculate $P(b,a)$ with the chain rule

![[Pasted image 20240110205913.png]]

This line is just logical. If we didn't do it like this, there would be no way of calculating $P(b,a)$ because we would either need the Bayes' Theorem or for it to be given to us, and if you look at the table, there are three columns, not two, so we can't just extract the values from the table.

Therefore, we will apply the chain rule.

![[Pasted image 20240110205933.png]]

We applied the chain rule first to $P(e,b,a)$ and then to $P(\lnot e, b, a)$.

![[Pasted image 20240110210014.png]]
![[Pasted image 20240110210033.png]]
![[Pasted image 20240110210725.png]]
Then we can just get our values from the table.

### Step 2 - Calculate $P(a)$

This is the probability of the alarm going off.

![[Pasted image 20240110210523.png]]

Again, just logical.

![[Pasted image 20240110210550.png]]

Here again we have to use the chain rule because we don't have information on just the probability of the alarm going off.

![[Pasted image 20240110210651.png]]

In the same fashion we plug in the numbers we have. Some come from the table and the others, such as the $P(e)$ or $P(b)$ were just given in the beginning.

![[Pasted image 20240110210807.png]]

### Step 3 - Plug in $P(b,a)$ and $P(a)$ and calculate

$$P(b|a) = \frac{P(b,a)}{P(a)} = \frac{0.019}{0.291} \approx 0.6535$$
## The Earthquake example - Burglary if (Alarm and Earthquake)

$$P(b|a,e)=?$$

![[Pasted image 20240110211331.png]]

$P(a,e) = P(b, a, e) + P(\lnot b, a, e)$ -> just for your understanding.

See the first example for the steps to take.

### Conclusion based on the two Earthquake Examples

$$P(b) = 0.02 < P(b|a,e) = - 0.0678 < P(b|a) = 0.6535$$

This illustrates the [[independence rv|independence]] of our variables. Alarm is dependent on the burglary, but burglary is not necessarily tied to both the alarm and the earthquake at the same time. 

## The large scary formula with the parent nodes

![[Pasted image 20240110212256.png]]

$P(x_1)$, $P(x_2)$ and $P(x_3)$ are just parent nodes that are independent, that's why they are written like that in the equation.

The others are simply represented by a [[conditional probability]] of themselves as posteriors and their parent nodes as priori, like the case for $P(x_4|x_{1} , x_{2}, x_{3})$, since those 3 nodes are the parents of $x_4$.

>[!success] Why this formula is important for our [[conditional probability table]]
>- To determine the number of rows we might need in our table, we would have to use the [[full joint probability distribution#Number of Parameters for a table formula|number of parameters for a table formula]], which is $2^{n}-1$, or $2^{7}-1=127$ rows (parameters) for binary variables. This is a lot.
>- With this network, we simply calculate it as $1+1+1+8+4+2+4=21$ rows (parameters). 

![[Pasted image 20240110215257.png]]

![[Pasted image 20240110215311.png]]

## Example Entering College

Consider two characteristics of a person. Being smart, denoted by binary variable $S$, and being an athlete, denoted by binary variable $A$.  

Let's assume that 40% of the population is smart, and 10% of the population is an athlete.  

Furthermore, let's denote the fact that someone entered college with the binary variable $C$. If you are smart you have higher chances of entering college as well as if you are an athlete.  

Let's say these probabilities are:
![[Pasted image 20240110215808.png]]

How would this graphical model look, and what would the factorization imply?

### First, we model

![[Pasted image 20240110215917.png]]

$$p(C,A,S) = p(C|A,S)p(A)p(S)$$

Questions:
1. What is the probability that an athlete is smart?
2. What is the probability of meeting a smart person in college?
3. What is the probability of meeting a smart person in college if that person is an athlete?

### Answering questions

1. What is the probability that an athlete is smart?
	- $p(s|a)=p(s)=0.4$ , because $s$ and $a$ are independent we don't need to use Bayes' and we take the value from "Let's assume that 40% of the population is smart"
2. What is the probability of meeting a smart person in college?
	- $p(s|c)=\frac{p(c,s)}{p(c)}=0.83$
	- ![[Pasted image 20240110222033.png]]
	
3. What is the probability of meeting a smart person in college if that person is an athlete?
	- You do it the same for $p(s|a,c) = 0.403$
# References

1. [[full joint probability distribution]]
2. [[graph]]
3. [[independence rv]]
4. [[marginal probability]]
5. [[conditional probability]]
6. [[conditional probability table]]
7. [[independence in bayesian networks]]