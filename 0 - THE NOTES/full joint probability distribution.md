---
type: topic
field: AI
short_desc: '"Note explaining all the different types of probabilities we can derive from a full joint probability table."'
field_type: probabilistic reasoning
module: "6"
parent: main
---
20240122101
Status: #m6
Tags: [[AI]]. [[probability]]

# full joint probability distribution

![[Pasted image 20240105135420.png]]

A **full join probability distribution** assigns a value (probability) for each [[random variable]].

>[!note] Note
>The three random variables headache, fever and covid are called **binary random variables**, since their values can only be "Yes" or "No".

We can derive a lot of probability types based on this kind of table. They are as follows in the next sections.
# Joint Probability

They worked based on [[joint probability]]. 

# Marginal Probability

One important thing we can derive from these tables are the [[marginal probability|marginal probabilities]] (click here for an example of how to calculate it). 

>[!note] Note
> We can apply marginalization to one or more [[random variable|RVs]].

# Disjunction Probability

[[disjunction probability|Disjunction probabilities]] are useful for one event between two events occurring.

$$  P(A \space or \space B) = P(A) + P(B) - P(A, B) $$

They are also useful for more complex operations, such as:

$$P(Condition1,!Condition2) \lor (Condition3, Condition2)$$

>[!note] Note
>In order to select your probabilities to sum, each table entry must pass the condition given, such as $$(Condition1, \lnot Condition2)\lor(Condition3,Condition2)$$
>Click [[disjunction probability#Example of the more complex formula|here]] for a detailed example of how to select these values.

# Vectors of Probability, or the "Probability Distribution"

[[vector of probability - probability distribution|The vectors of probability]] are another useful thing we can derive from the full joint probability table. They help in representing the probabilities of our tables into an array to make it easier to view the data.

$$\textbf P(condition) = [P(condition), P(\lnot condition)]$$
>[!note] Note
>- They are always written with a bold letter, but the probabilities inside are written in normal letters.
>- The sum of all the probabilities in this vector is always 0.
>- When we say that we 'calculate the matrix of probabilities of a table or [[data frame]]', we mean that we want to establish the [[vector of probability - probability distribution]] for that table

# Conditional Vectors of Probability, or "Conditional Distribution"

[[conditional vector of probability - conditional distribution|The conditional distribution]] is also important. It's the same as using the [[vector of probability - probability distribution|vectors of probability]], but applying the [[conditional probability]] to them.

>[!note] Note
>There are two distinct formulas we can apply here:
>1. $\textbf P(Condition1|condition2) = [P(condition1|condition2), P(\lnot condition1|condition2)]$
>2. $\textbf P(Condition1|Condition2) = [[P(condition1|condition2), P(\lnot condition1|condition2)], P(condition1| \lnot condition2), P(\lnot condition1|\lnot condition2)]]$
>So, be very careful how you capitalize that given condition, cause it can lead to different arrays. There is a distinction here because the first one is referring to 'covid' as a value, while the second one refers to 'Covid' as a [[random variable]].
>Also, the second one is known as ** estimating matrix of conditional probabilities for the data frame P.**

# Number of Parameters for a table formula

>[!success] Forumla
>$2^{n}-1$, where $n$ is the number of [[random variable|random variables]].


# References

1. [[random variable]]
2. [[joint probability]]
3. [[marginal probability]]
4. [[disjunction probability]]
5. [[conditional probability]]
6. [[vector of probability - probability distribution]]
7. [[data frame]]
8. [[conditional vector of probability - conditional distribution]]
9. [[conditional probability]]
10. [[bayesian network]]
