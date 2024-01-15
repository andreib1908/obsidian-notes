---
type: topic
field: AI
field_type: probabilistic reasoning
parent: "[[vector of probability - probability distribution]]"
short_desc: '"A note related to mathematics."'
module: "6"
---

202401082349
Status: #m6
Tags: [[math]] 

# conditional vector of probability - conditional distribution

Depicts the possible outcomes for all the given values of a [[random variable]].

It's the same as a [[vector of probability - probability distribution]], but applied for [[conditional probability]].


# Formula

$$\textbf P(A|b) = [P(a|b), P(\lnot a|b)]$$
$$\textbf P(A|B) = [[P(a|b), P(\lnot a|b)], P(a| \lnot b), P(\lnot a|\lnot b)]]$$
>[!warning] Lowercase priori condition $P(A|b)$
>$$\textbf P(A|b) = \frac {\textbf P(a, b)} {P(b)} = \frac {\textbf P(a,b)}{\alpha}, where \space \alpha = \sum\limits P(a,b) $$
>You can calculate $\textbf P(A,b)$ with [[vector of probability - probability distribution#Formula|the vector of probability with lowercase form]].

>[!warning] Uppercase priori condition $P(A|B)$
$$\textbf P(A|B) = [\frac {[P(a, b), P(\lnot a, b)]} {\alpha \space of \space b}, \frac {[P(a, \lnot b), P(\lnot a, \lnot b)]} {\alpha \space of \space \lnot b}] $$

# Examples

## First two easier formulas

![[Pasted image 20240105135420.png]]

$$\textbf P(Headache|covid) = [P(headache|covid), P(\lnot headache|covid)] = [0.73,0.27]$$
$$\textbf P(Headache|Covid) = [[P(headache|covid), P(\lnot headache|covid)], [P(headache, \lnot covid), P(\lnot headache, \lnot covid)]] = [[0.73,0.27], [0.29, 0.71]]$$

## Third harder formula

![[Pasted image 20240109001007.png]]
![[Pasted image 20240109001028.png]]

$P(covid) = 0.25 + 0.05 + 0.10 + 0.01 = 0.41$

At the last '=' sign, we divide each member of the array by the constant $\alpha$, which you can calculate as either $P(covid)$ or:
$\alpha = 0.3 + 0.11$ -> taken from the $\textbf P(Headache, covid)$.

They both get you 0.41.

## Fourth very hard formula

![[Pasted image 20240109002143.png]]

![[Pasted image 20240109002200.png]]
# References

1. [[random variable]]
2. [[conditional probability]]
3. [[full joint probability distribution]]
4. [[vector of probability - probability distribution]]