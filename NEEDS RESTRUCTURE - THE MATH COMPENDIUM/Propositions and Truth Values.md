
# Proposition

**A proposition** is a statement whose meaning can be given in terms of *true* and *false*.

*0* means *false*.
*1* means *true*.

# Proposition Connectives

![[Pasted image 20230911152732.png]]

[[Reader Introduction to Mathematics-1.pdf#page=22|Table of Connectives + Examples 1.2.3 and 1.2.4]]

# Truth Tables

### Implications

![[Pasted image 20230911152843.png]]

p -> q is called **an implication**.

If *p*, then *q*.

We usually make a general statement:
- `If it rains today, I take my umbrella with me.`

This statement is composed of:
1. **THE HYPOTHESIS** (or *p*)
	- `If it rains today`
2. **THE CONCLUSION** (or *q*)
	- `I take my umbrella with me`

Both the **hypothesis** and the **conclusion** have their own combinations for *true* and *false*.

They get combined into the overall statement *p -> q* to determine a final truth value in relation to the original statement.

If the **hypothesis** *p* is **false**, then it does not matter what truth value the **conclusion** has. The statement *p -> q* will always be true.
- We laid the condition `IF HYPOTHESIS`, so if you violate that from the beginning the statement still holds either way.
- We would be saying `It is not raining today`, so it does not matter what I do as I only cared about the event `It is raining today`.

Otherwise, the **conclusion** *q* must be true, otherwise I am not acting as I planned:
- `It is raining and I said I would take my umbrella, but I won't for some reason.`

#### Note

![[Pasted image 20230911154120.png]]

*p -> q* and *!q -> !p* are **logically equivalent**, as they have the same values in the truth table.

### Complex Statements

![[Pasted image 20230911153933.png]]

It's pretty easy. Break it down into smaller expressions and work from left to right.

Remember to **first apply negation of a proposition or statement** and then move on.

# Logically Equivalent Propositions

Two **propositions** *s1* and *s2* are **logically equivalent (l.e.)** if *s1* is true if and only if *s2* is true.

![[Pasted image 20230911154412.png]]

In a truth table, the columns corresponding to logically equivalent propositions are identical.

# Tautology

A **tautology** is a statement that **is always true**.

If two propositions are **logically equivalent** then the statement **s1 <-> s2** is a **tautology**, and the other way around too.

**Note**:
- *s1 <-> s2* is a proposition that might be true or false
- *s1 <=> s2* indicates that *s1 <-> s2* is always true.

# Contradiction

A **contradiction** is a statement that is always false.

![[Pasted image 20230911154835.png]]

# Counterexample

A **counterexample** to a **statement** is a [[Sets]|set]] of propositions that make the statement **false**.

![[Pasted image 20230911155007.png]]

Like row number 4 here.
