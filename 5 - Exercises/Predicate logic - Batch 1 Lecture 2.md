---
type: exercise
field: AI
field_type: AI + logic
module: "6"
points_earned: 0/7
---
20240121837
Status: #m6
Tags: [AI], [logic], [exercise]

# Exercise 1

You can see P(x) = "x is a man" and Q(x) = "x is mortal"

1. All P's are Q's: (V)xP(x) -> Q(x) 
2. Some P's are Q's: (V)x(P(x) -> Q(x)) v (E)xP(x) -> !Q(x)
3. No P's are Q's: (V)xP(x) -> ! Q(x)
4. Some P's are not Q's: (E)xP(x)^!Q(x)

Solution:
1. yes
2. no. (E)x(P(x) ^ Q(x))
3. yes
4. yes
# Exercise 2

Small(x), Happy(x), Dog(x), Home(x)

1. (E)xSmall(x)^Happy(x)^Dog(x)^Home(x)
2. (V)x(Small(x) ^ Dog(x) ^ Home(x)) -> Happy(x)

Solution:
1. yes
2. yes
# Exercise 3

- P(x)
- Q(x)
- !(V)x(P(x) ^ Q(x)) = (E)x(!P(x) v ! Q(x))

Which model satisfies the last sentence?

1. No objects and relations P,Q
2. One object a and relations P,Q
3. One object a and relations P,Q with a belongs to P and a belong to Q.

Answer: b

Solution:
correct. read the solution in the PDF for more info
# Exercise 4

- Food(x): x is something to eat
- Person(x): x is a person
- Likes(x,y): x likes y

1. (V)x(Food(x) => (E)y (Person(y) ^ Likes(y,x) ))
2. (E)x(Food(x) ^ (V)y (Person(y) => Likes(y,x) ))

Solution:
# Exercise 5

Solution:

# Exercise 6

Solution:
# Exercise 7

Solution:

# References

PDF with only questions: [[Tutorial_2_Pred_Logic_Questions.pdf]]

PDF with answers: [[Tutorial_2_Pred_Logic_Answers.pdf]]

