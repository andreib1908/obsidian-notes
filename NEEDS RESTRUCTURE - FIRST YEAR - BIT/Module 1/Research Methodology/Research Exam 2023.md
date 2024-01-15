# Part A

## Q1 - Y

D 

## Q2 - Y

A

## Q3 - Y

B

# Part B

## Q4 - Y

B

## Q5 - N

C, *but could also be A*
**it was A yes**
## Q6 - Y

B

# Part C

## Q7  - Y

B

## Q8  - Y

C

## Q9 - N

A
**it was C, you thought of it**

# Part D

## Q10 - Y

A

## Q11 - Y

C

## Q12 - N

D, *but it could be B*
**it was C actually**

# Part E

## Q13 - Y

D, *B potentially*

## Q14 - Y

B

## Q15 - N

C
**it was D, ratio**

# PART F

## Q16 - Y

A

## Q17 - Y

A

## Q18 - N

C
**it's D, the tiebraker is looking at the second most important weight**

## Q19 - Y

```python
def getScores(list_of_weights, list_of_scores):  
    result = 0  
    for index in range(len(list_of_scores)):  
        result += list_of_scores[index]**2 * list_of_weights[index]  
    return result  
  
  
list_of_weight = [10, 4, 6, 8]  
print(getScores(list_of_weight, [7, 3, 10, 1]))  
print(getScores(list_of_weight, [3, 10, 7, 3]))  
print(getScores(list_of_weight, [10, 8, 8, 8]))  
print(getScores(list_of_weight, [10, 6, 1, 10]))
```

1134 for A
856 for B
2152 for C
1950 for D

=> C is best

## Q20 - N

D
**it was B**







