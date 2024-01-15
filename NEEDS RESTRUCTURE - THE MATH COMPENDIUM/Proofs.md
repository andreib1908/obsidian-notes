
# Proofs

Proofs are **watertight** arguments that hold in **in all possible cases** that can be considered.

### Recommended steps for findings proofs

1. Determine what **you are given** and **what you can assume** about the problem.
2. Write down the **mathematical definitions** of what you have to show.
3. See if the statement is reasonable (try it with examples). If you think the statement isn't, try to come up with [[Propositions and Truth Values#Counterexample|counterexamples]].
4. If the statement isn't clear, browse through related theorems and examples.
5. When you think the statement is clear, analyze why it is the case. Write it in the form of *mathematical* steps.
6. See if the proof holds at the end and if it is reasonable.

#### Important example

[[Reader Introduction to Mathematics-1.pdf#page=40|Example 2.1.1 - Good for beginning]]

# Even and Odd Numbers

Let:
- *n* be an [[Sets#Sets of Numbers|integer]], or *n* **in** *Z*

- *n* is **even** if there exists an integer *k* in *Z*, such that *n* = 2 * *k*
- *n* is **odd** if there exists an integer *k* in *Z*, such that *n* = 2 * *k* + 1

![[Pasted image 20230917193350.png]]

# Good vs Wrong proofs

[[Reader Introduction to Mathematics-1.pdf#page=41|Example 2.1.3 - good proof]]

[[Reader Introduction to Mathematics-1.pdf#page=41|Example 2.1.4 - proof that can go wrong]]

*Essentially, before you start proving something, you must ensure that the hypothesis is reasonable and check the conditions of your steps. Else you end up with something like 4=3*

# Counterexample 

Also see: [[Propositions and Truth Values#Counterexample]]

- It satisfies the conditions of the theorem (hypothesis)
- It **does not** satisfy the **theorem's conclusion**

-> This leads to showing that **the theorem is not true in general**.

### Example

Prime number = "positive integer which has two divisors, 1 and itself"

Prime numbers: {2, 3, 5, 7...}

Take the statement:
`All prime numbers are odd.`

A **counterexample** for this would be the number 2. This means that the statement is False.

Also, check [[Reader Introduction to Mathematics-1.pdf#page=43|Statement 2.2.3]] for checking/removing unnecessary conditions through counterexamples.

# Proof by Contradiction

![[Pasted image 20230918115954.png]]
![[Pasted image 20230918120011.png]]

So, after we negate the initial theorem, if we prove that the contradiction is false, then the original Theorem must be true.

# Direct Proof

**Direct proof** is a sequence of logical arguments that deduce the conclusion from the givens of the theorem.

![[Pasted image 20230918123503.png]]

# Proof by cases

![[Pasted image 20230918124523.png]]


# Mathematical Induction

Let:
- *n* in *N* ([[Sets#Sets of Numbers]])
- *S(n)* is a [[Propositions and Truth Values#Complex Statements|statment]]

Induction steps:
a) Check if *S(1)* is true for every positive integer *n*
	- This is also called the **induction hypothesis**
b) Assume that each *k* **in** *N*, if *S(k)* is true
	- then prove that *S(k+1)* is also true.

The steps are called:
- Step a) -> **BASIS STEP**
- Step b) -> **INDUCTION STEP**

[[Reader Introduction to Mathematics-1.pdf#page=47|Example 2.6.2]]

## Divisibility

Let:
- *m* and *d* be integers

We say that *m* is divisible by *d* if there exists an integer *l* in *Z* such that:
- *m* = *dl*

[[Reader Introduction to Mathematics-1.pdf#page=49|Example 2.6.5.]]










