---
type: topic
field: logic
field_type: predicate logic
short_desc: '"A way to apply a universal constant to CNFing some predicate logic."'
module: "6"
parent: "[[CNF Conjunctive Normal Form]]"
---

20240121504
Status: #topic
Tags: [[AI]], [[logic]]

# skolemization


![[Pasted image 20240101210859.png]]

>[!note] Note
>We completely drop the (E)x part if we use the Skolem constant.

Here's a problem:

`(V)x Human(x) => (E)y Loves(x,y)`

Would this be replaced by `(V)x Human(x) => Loves(x,S)`?

No, because `y` depends on `x`, and is therefore a **function** of `x`.

The solution is to introduce the **Skolem** function:
`(V)x Human(x) => Loves(x,S(x))`

# What is Skolemization
 
 Skolemization transforms a formula in first-order logic to an equisatisfiable formula (a formula that is satisfiable if and only if the original formula is satisfiable) that does not contain existential quantifiers (∃∃). This is done by replacing each existential quantifier with a Skolem function.
    
# **How Skolemization Works:**
    
- If an existential quantifier ∃y appears in a formula, and is not in the scope of any universal quantifier (∀), it is replaced with a constant, known as a Skolem constant.
- If an existential quantifier ∃y is within the scope of one or more universal quantifiers, for instance ∀x∃y, the existential quantifier is replaced with a Skolem function. The arguments of the Skolem function are the universally quantified variables in whose scope the existential quantifier exists.

>[!tldr] TLDR
>Skolemization is used to convert from `P(x, y)` to `P(x, f(x))` and to generalize the quanitifiers. We drop the universal quantifier, since formulas become implicitly quantified.

# **Purpose of Skolemization:**

-  **Facilitates Reasoning:** By eliminating existential quantifiers, Skolemization simplifies the structure of logical formulas, making them more amenable to automated reasoning and proofs.
 - **Preserves Satisfiability:** The process does not preserve logical equivalence, but it preserves satisfiability, which is crucial in theorem proving and model checking.

# **When to Use Skolemization:**
    
- **Automated Theorem Proving:** It's used in algorithms for automated theorem proving, where it's essential to simplify the formula to make the process of finding proofs more efficient.
- **Logic Programming:** In logic programming and computational logic, Skolemization is used to handle existential quantifiers that cannot be directly represented or processed.

![[Pasted image 20240102162656.png]]

>[!tip] Example of Skolemization
> Consider a formula: `∀x∃y(P(x,y))`. Skolemization replaces `y` with a Skolem function `f(x)`.
> It results in `∀x(P(x,f(x)))`.


# References

[[CNF Conjunctive Normal Form]]
[[predicate logic]]