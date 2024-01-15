
There are two very important rules in counting:
- **Product rule**
- **Sum rule**

# Product Rule

Suppose that a procedure can be broken into a sequence of two tasks.

If there are *n1* ways to do the **first task** and, for each of these ways of doing the first task, there are *n2* ways to do the **second task**, then there are *n1n2* **ways** to do the procedure.

![[Pasted image 20230918162450.png]]

![[Pasted image 20230921112329.png]]
# Sum Rule

If a task can be done **either** in **one of n1 ways or in one of n2 ways**, where no element of the [[Sets#Definition|set]] of *n1* ways is the same as **any** of the set of *n2* ways, then there are *n1+n2* **ways** to do the task.

![[Pasted image 20230918162732.png]]

The separate set of tasks must be *disjoint* (their intersection is empty) for you to calculate them once. If 4 of the 18 cultural clubs also belong to the 35 sports clubs, then these four clubs would be counted twice in the sum 18+35.

So, if we only wanted the number of **distinct** clubs, we must subtract 4 from the sum:
- 18+35-4 = 49

This idea is called the **principle of inclusion-exclusion**.

![[Pasted image 20230920120559.png]]


![[Pasted image 20230921112218.png]]

# Very important distinction

![[Pasted image 20230921112353.png]]

- You use the **SUM RULE** for determining the **NUMBER OF CHOICES**
- You use the **PRODUCT RULE** for determining the **NUMBER OF PAIRS**
# Principle of Inclusion/Exclison

![[Pasted image 20230921112547.png]]

![[Pasted image 20230921112604.png]]

**You apply I/E when you need to find the number of choices in between two sets, but they are NOT DISJOINT.**
- I.e. sum rule traditionally only works on disjoint sets, otherwise you apply I/E

### Tricky Exercise to illustrate

![[Pasted image 20230921113145.png]]

The sets here are not **disjoint** because they may have some similar elements:
- take 'ai', for example. It can be found both in A and in B, as the *l* can be any letter, including vowels themselves.

You remove their intersection according to the I/E principle, which is calculated based on the [[Product Rule and Sum Rule (with Inclusion or Exclusion)#Product Rule|Product Rule]].