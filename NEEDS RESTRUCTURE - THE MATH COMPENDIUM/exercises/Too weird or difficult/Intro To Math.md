
# Chapter 2

### Exercise 2.5 b

To prove that there exists a unique prime of the form n2−1n2−1 for n∈Nn∈N, you need to demonstrate two things:

1. Existence: Show that there is at least one value of nn for which n2−1n2−1 is prime.
2. Uniqueness: Show that there cannot be more than one prime of this form.

Let's start with the first part:

**Existence:** Consider n=2n=2. In this case, n2−1=22−1=4−1=3n2−1=22−1=4−1=3. We know that 3 is a prime number. So, for n=2n=2, we have n2−1=3n2−1=3, which is a prime number.

Now, let's move on to the second part:

**Uniqueness:** Assume, for the sake of contradiction, that there exist two distinct values of nn, say n1n1​ and n2n2​, such that n12−1n12​−1 and n22−1n22​−1 are both prime numbers, and n1≠n2n1​=n2​.

Then, we have:

n12−1=pn12​−1=p (where pp is a prime number)

and

n22−1=qn22​−1=q (where qq is a prime number)

Now, let's subtract these two equations:

(n12−1)−(n22−1)=p−q(n12​−1)−(n22​−1)=p−q

Simplifying, we get:

n12−n22=p−qn12​−n22​=p−q

Using the difference of squares formula, we can factor the left side:

(n1−n2)(n1+n2)=p−q(n1​−n2​)(n1​+n2​)=p−q

Since both n1n1​ and n2n2​ are positive integers, it follows that n1−n2n1​−n2​ and n1+n2n1​+n2​ are also positive integers.

Now, notice that the right side, p−qp−q, is a difference between two prime numbers, and it is a positive integer.

However, the left side, (n1−n2)(n1+n2)(n1​−n2​)(n1​+n2​), is a product of two positive integers, which means it is a positive integer as well.

So, we have a positive integer on both sides of the equation, which means:

(n1−n2)(n1+n2)=p−q(n1​−n2​)(n1​+n2​)=p−q

is a nontrivial factorization of a positive integer (p−qp−q).

This contradicts the fundamental theorem of arithmetic, which states that every positive integer greater than 1 can be factored into prime numbers in a unique way (up to the order of the factors).

Therefore, our assumption that there exist two distinct values of nn such that n2−1n2−1 is prime leads to a contradiction.

Hence, there is only one prime of the form n2−1n2−1 for n∈Nn∈N, and that prime is 3 (when n=2n=2).

:)

