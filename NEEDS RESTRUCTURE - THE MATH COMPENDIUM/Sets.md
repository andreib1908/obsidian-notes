
# Definition

**Sets** are a **collection** of:
- *Well-Defined*
- *Unordered*
- *Distinct*
elements.

They can be **equal** to each other if they have **the same elements**.
- {1, 3, 4} = {4, 1, 3}
## Examples

- {1, 3, 4}
- A = {1,3,4}, B = {1,4,3}, C = {1,3}
	- A = B
	- A != C

# Elements of a set

If an element *x* is part of a [[Sets#Definition|set]] *A*, then we can write it as:
- ![[Pasted image 20230910143447.png]]
## Different Notations

- *C* = {2,4,5,8...}
- *C* = {x | x is a positive, even integer}
- *A* = {{1}, {2}, {3}, {1,2}, {2, 3}, {1,2,3}}
	- 1 **is not** in *A*, but {1} **is** in *A* (as elements)
- *D* = {x | f(x) > 0}
	- This means *D* is the [[Sets#Definition|set]] of all *x* elements **such that** (the *'|'* symbol) the function f(x) is always greater than 0.

# The Empty Set (NULL)

**The empty set** is a [[Sets#Definition|set]] **without** elements.

![[Empty_set_symbol.svg.png]]

It can also be written as *{}*.

## Properties 

- *{}* != {*{}*}, since *{}* **is not** in *{}* as an element
- *{}* != {0}
- 0 **is** in {0}

# Cardinality of a Set

The **cardinality** of a [[Sets#Definition|set]] is the number of elements:
- {1, 2, 3} has **cardinality** 3
- {1, 2} has **cardinality** 2

# Finite Sets

A [[Sets#Definition|set]] *A* is finite when it has a finite number of *n* elements (or none).
- *n* is the [[Sets#Cardinality of a Set|cardinality]] of *A*

*Example*:
- {1, 2, 3, 4}
# Infinite Sets

A [[Sets#Definition|set]] *A* is finite when it has an infinite number of *n* elements.
- *n* is the [[Sets#Cardinality of a Set|cardinality]] of *A*

*Example*:
- {1, 2, 3...}
- The [[Sets#Definition|set]] of all **Natural** numbers

# Sets of Numbers

- **Natural Numbers** *N*
	- [1, infinity] but not 0
	- 1, 2, 3, 4,...
- **Integers** *Z*
	- Includes *N*
	- [-infinity, infinity]
	- -1, -6, 5, 13 etc.
- **Rational Numbers** *Q*
	- Includes *Z*
	- [-infinity, infinity]
	- 1/2, 4/15, -3/2 etc.
- **Real Numbers** *R*
	- Includes *Q*
	- Periodic Numbers
		- 1.3333333333333...
		- 3.145145145145....
	- Square roots
		- sqrt(2)
	- Pi


# Extreme Values of sets

Let's use *X* = {4, 5, 6} and *I* = `[3, 4]` ([[Intervals|interval explanation]]).
## Upper Bound

The **upper bound** of a [[Sets#Definition|set]] *X* is any number *u* in *R* such that *u* >= *x* for every *x* in *X*.

### The Supremum

- The *smallest* *possible* [[Sets#Upper Bound|upper bound]]. 
	- sup(*X*) <= *u* for any [[Sets#Upper Bound|upper bound]] *u* of *X*

sup(*X*) = 6
sup(*I*) = 4

### The Maximum
- *X* is bounded above
- sup(*X*) **is** in *X*

We call it **max(*X*)**.

max(*X*) = 6
max(*I*) = 4

but if *I* = `[3, 4)`
max(*I*) does not exist

However, if we had `[3, infinity)`, we would have no sup or max.

#### ChatGPT - supremum, but no maximum

Consider the set of all real numbers that are less than 1:

A={x∈R:x<1}A={x∈R:x<1}

In this set, there is no maximum element because there is no single real number that is greater than or equal to all the elements in the set. However, the set has a supremum, and the supremum is 1.

The supremum, or least upper bound, of the set A is the smallest real number that is greater than or equal to all the elements in the set. In this case, 1 is the supremum because it is the smallest real number that is greater than or equal to all the numbers in the set (since all numbers in the set are less than 1). However, 1 is not actually an element of the set, so the set has no maximum element.

## Lower Bound

The **lower bound** of a [[Sets#Definition|set]] *X* is any number *l* in *R* such that *l* <= *x* for every *x* in *X*.

### The Infimum

- The *greatest* *possible* [[Sets#Lower Bound|lower bound]]. 
	- inf(*X*) >= *l* for any [[Sets#Lower Bound|upper bound]] *l* of *X*

### The Minimum
- *X* is bounded below
- inf(*X*) **is** in *X*

We call it **min(*X*)**.


#### ChatGPT - infimum but no minimum

Consider the set of all real numbers greater than or equal to -1 but less than 1:

B={x∈R:−1≤x<1}B={x∈R:−1≤x<1}

In this set, there is no maximum element because no element in the set is greater than or equal to all the other elements. However, the set has an infimum, and the infimum is -1.

The infimum, or greatest lower bound, of the set B is the largest real number that is less than or equal to all the elements in the set. In this case, -1 is the infimum because it is the largest real number that is less than or equal to all the numbers in the set (since all numbers in the set are greater than or equal to -1). However, -1 is an element of the set, so the set has no maximum element.

Check [[Reader Introduction to Mathematics-1.pdf#page=11|Example 1.1.13, 1.1.14, 1.1.15]] from reader.

## General rules for NOT having a supremum or infimum

1. **Empty Set**: If the set is empty, there are no elements, and therefore, there is no maximum.
    
2. **Open Interval**: In open intervals, such as (a, b), there is no maximum because there is no endpoint that is included in the interval. For example, in the open interval (1, 2), there is no maximum value because no element in the interval is greater than or equal to all other elements.
    
3. **Unbounded Interval**: In unbounded intervals, like (-∞, a) or (b, ∞), there is no maximum because the interval extends infinitely in one direction, and there is no endpoint.
    
4. **Discrete Set with No Maximum Element**: In some sets of discrete values, there may not be a maximum if there is no single element that is greater than or equal to all other elements. For example, the set {1, 2, 3, 4, ...} of natural numbers has no maximum because there is always a larger natural number.

# Universal Set

The universal set is usually denoted by *U* and is the set of all possible values in your context.

So *U* can be the set of all dogs in Enschede, while *A* is the set of all Golden Retrievers in Enschede. 

Or:
![[Pasted image 20230911152234.png]]

It depends on the context.

# Complement

The **complement** of a set is everything else not part of the **set you are working with**.

So if *A* = {n | 4 < n < 6}, then *U* in this scenario would be:
- *A 'complement'* = `(-inf, 4]` united `[6, inf]`

![[Pasted image 20230911152026.png]]
![[Pasted image 20230911152040.png]]

# Difference

The difference between two **sets** *A* and *B* is the set of elements found in *A* but not in *B*.

![[Pasted image 20230911152141.png]]
![[Pasted image 20230911152148.png]]

![[Pasted image 20230911152156.png]]

Also note:
![[Pasted image 20230911152209.png]]

Check [[Reader Introduction to Mathematics-1.pdf#page=18|Example 1.1.36]]



#set #emptyset #finiteset #infiniteset #cardinality #maths #introtomath #setsofnumbers #upperbound
#lowerbound #infimum #supremum #maximum #minimum