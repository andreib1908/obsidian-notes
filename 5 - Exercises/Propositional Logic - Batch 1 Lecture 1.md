This is tied to the first batch:

![[Pasted image 20240101194555.png]]

Questions: [[Tutorial_1_Prop_logic_Questions.pdf]]
With Answers: [[Tutorial_1_Prop_logic_Answers.pdf]]

My attempt.

# Exercise 1

![[Pasted image 20240101195059.png]]

=> 4 models (the true values) => B

# Exercise 2
![[Pasted image 20240101200306.png]]
 => 7 => D
# Exercise 3
[[theorem proving]]
Can we prove `bread`?

1. bread v earlyMeeting
2. (tea v coffee) ^ juice
3. earlyMeeting => yoghurt
4. yoghurt => !coffee
5. !yoghurt

Getting CNF:
7. tea v coffee, juice
8. !earlyMeeting v yoghurt
9. !yoghurt v !coffee

Full set of KB with the next steps. So we try to prove `bread` with contradiction:
1. bread v earlyMeeting
2. tea v coffee, juice
3. !earlyMeeting v yoghurt
4. !yoghurt v !coffee
5. !yoghurt
6. `!bread`
7. !earlyMeeting(3, 5)
8. bread(1, 7)
9. empty(6, 8)


# Exercise 4

1. K V L
2. K => M
3. !L

Prove M

1. K V L
2. !K V M
3. !L
4. !M
5. K(1,3)
6. M(2,5)
7. EMPTY(4,6)

=> Through contradiction, we have proven M.

# Exercise 5

![[Pasted image 20240102182330.png]]
![[Pasted image 20240102182339.png]]

# Exercise 6

The answer is C because it has two positive literals, namely r and v.

Horn clauses can only have one positive literal (at most). [[horn clauses]]

# Exercise 7

I think that for problem-solving and algorithmically thinking, this naming convention would, indeed, make the machine a better reasoner than a human. An example that comes to mind is the [[wumpus world]], where a machine can easily reason what the best course of action will be at any given time to avoid being eaten by the wumpus, potentially having a 100% success rate. Human players may look at the same semantics and take extra time or not even get them at all.

However, for ambiguous wording such as 'young', or 'large', or when morality might be involved, the humans will be better reasoners. They themselves have experienced being 'young' or seeing 'large' objects, giving them an edge for reasoning.