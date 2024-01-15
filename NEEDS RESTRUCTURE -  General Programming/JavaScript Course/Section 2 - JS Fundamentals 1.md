
# alert("String") 

![[Pasted image 20230423175206.png]]

Displays some message on the screen.

# Defining a variable and checking it

![[Pasted image 20230423175444.png]]
- Here we print after the if statement is true.


![[Pasted image 20230423175529.png]]
- We changed the contents of js, so the if statement is no longer true.

# Where to place JS scripts in HTML and how to print stuff to the console

![[Pasted image 20230423180746.png]]

OR

![[Pasted image 20230423180953.png]]

![[Pasted image 20230423180806.png]]

![[Pasted image 20230423180751.png]]


# Variables

## 'let'

Function-oriented

![[Pasted image 20230423181238.png]]


![[Pasted image 20230423181244.png]]

![[Pasted image 20230423181526.png]]

## Constants 

![[Pasted image 20230425121552.png]]
- The "const" keyword creates a variable that cannot be changed from its initial value. They tried to do it in this example, so JS gave that error.

## Alternative to 'let' - 'var'

Block-oriented
![[Pasted image 20230425122021.png]]


# Objects and primitives

![[Pasted image 20230425120620.png]]

![[Pasted image 20230425120635.png]]
![[Pasted image 20230425120658.png]]

![[Pasted image 20230425120828.png]]

## typeof variable

![[Pasted image 20230425121203.png]]
- Returns the type of the variable.


# String literals - building strings easier

![[Pasted image 20230809170325.png]]

Instead of doing this and worrying about + signs and spaces and quotations:
![[Pasted image 20230809170232.png]]

You can use string literals to build them easily!
![[Pasted image 20230809170354.png]]

You can use those symbols for **any** type of string. You can fully replace using normal quote signs.
![[Pasted image 20230809170449.png]]
![[Pasted image 20230809170503.png]]


Multi-line strings are easier with this symbol too (you just press ENTER instead of having to type backslash n):
![[Pasted image 20230809170539.png]]

# Type conversion | coercion

## Correct type conversion

You can easily convert variables of a type to another like so:
![[Pasted image 20230809172149.png]]
![[Pasted image 20230809172154.png]]
*Note: After that Number(inputYear) operation, the original value of inputYear has not changed. I.E. inputYear remains a string, instead of being changed into a number.*

![[Pasted image 20230809172355.png]]
![[Pasted image 20230809172359.png]]

## Error in converting

![[Pasted image 20230809172435.png]]
![[Pasted image 20230809172440.png]]
*It means 'invalid number'.*


# Truthy and Falsy values

Basically values that aren't exactly true or false, but are about to be.

There are five of them in JavaScript:

> - 0
> - ' '
> - undefined
> - null
> - NaN



![[Pasted image 20231231194538.png]]

![[Pasted image 20231231194717.png]]
![[Pasted image 20231231194725.png]]


