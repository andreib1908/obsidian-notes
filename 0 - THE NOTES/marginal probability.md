---
type: topic
field: AI
field_type: probabilistic reasoning
parent: 
short_desc: '"A note related to mathematics."'
module: "6"
---
202401082210
Status: #m6
Tags: [[math]] , [[AI]]

# marginal probability

*'to marginalize'* = To treat something as insignificant.

The **marginal probability** is a probability over a subset of [[random variable|random variables]].

![[Pasted image 20240108221224.png]]

Here, 'Covid' is marginalized
# Formula

$$\sum_{x \in \{\text{yes}, \text{no}\}} P(\text{Headache} = \text{yes}, \text{Fever} = \text{no}, \text{Covid} = x) $$


## The Example

`sum of x in {yes, no} of (P(Headache = yes, Fever = no, Covid = x)`

![[Pasted image 20240108221553.png]]

![[Pasted image 20240108221608.png]]

Here we wrote 'Covid = x' because that is the value we are trying to marginalize.

So, we look in the table where we have `Headache = yes` and where we have `Fever = no` regardless of what `Covid` may be. There are only two entries in the table that match this combination, which are rows 3 and 4 (if we start our indexing at 1).  

Then, we just replace and calculate:
`sum of x in {yes, no} of (P(Headache = yes, Fever = no, Covid = x) = 0.05 + 0.05 = 0.1`

# Marginalizing two or more random variables

We are not restricted to marginalizing one [[random variable]], like we had the `Covid = x` thing. We can do this for any number of [[random variable|RVs]] by just assigning variables.

![[Pasted image 20240108222103.png]]

>[!note] Same probability with short or extended notation
>- `P(Headache = yes) = sum of x in {yes,no} of (sum of y in {yes, no} of (P(Headache = yes, Fever = y, Covid = x)))`
>- The marginalization is applied to Fever and Covid.
>- Marginalizing both Fever and Covid means that we don't care what values they have as long as our Headache stays 'yes'.


# References

1. [[random variable]]
2. [[joint probability]]
3. [[full joint probability distribution]]