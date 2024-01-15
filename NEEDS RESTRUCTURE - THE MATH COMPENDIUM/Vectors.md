
Prerequisite lesson for this: [[Coordinate Planes]]

# Definition

Vectors usually describe *forces*, where we have *directions* and *lengths* to signify magnitudes in the chosen unit of measurement.

![[Pasted image 20231024135920.png]]

![[Pasted image 20231024135900.png]] 

### Equal Vectors

![[Pasted image 20231024135944.png]]

# Component Form - Two dimensional and Three dimensional vectors

If **v** is a *two-dimensional* vector in the plane and has its *initial point* at the **origin** and its *terminal point* at `(v1, v2)`, then the **component form** of **v** is:
- `v = <v1, v2>`

If **v** is a *three-dimensional* vector in the plane and has its *initial point* at the **origin** and its *terminal point* at `(v1, v2, v3)`, then the **component form** of **v** is:
- `v = <v1, v2, v3>`

So a 2d vector is a tuple of real numbers, while a 3d vector is an ordered triple of real numbers.

The numbers `v1, v2 and v3` are called the **components of v**.

![[Pasted image 20231024140702.png]]
![[Pasted image 20231024140735.png]]

# The length (magnitude) of a vector

![[Pasted image 20231024140921.png]]

when `v = <v1, v2, v3>`.

# Scalar multiplication and addition

![[Pasted image 20231024141136.png]]
![[Pasted image 20231024141351.png]]

### Geometric Representations - Scalar Multiplication

![[Pasted image 20231024141652.png]]
					![[Pasted image 20231024141659.png]]

### Geometric Representations - Triangle and Parallelogram Laws

![[Pasted image 20231024141511.png]]

				![[Pasted image 20231024141827.png]]

# Properties of Vector Operations

![[Pasted image 20231024141902.png]]
![[Pasted image 20231024141953.png]]

# Unit Vectors

The vector of length 1 is always called the **unit vector**. The standard unit vectors are:
- `i = <1, 0, 0>`
- `j = <0, 1, 0>`
- `k = <0, 0, 1>`

![[Pasted image 20231024142129.png]]
![[Pasted image 20231024142220.png]]

# The direction of a nonzero vector v

![[Pasted image 20231024142755.png]]

[[Vectors#The length (magnitude) of a vector|Length of vector v section]]; [[Vectors#Unit Vectors|Unit Vectors section]]

`v = <v1, v2, v3>`

I think that we are given either the component form or the length of the vector in the exercise when we have to calculate the direction of the vector. Like here:

![[Pasted image 20231024144313.png]]
![[Pasted image 20231024144340.png]]

But, at least, this is how you would normally calculate both of them separately. 

### CHATGPT suggestion - Normalizing your vectors

Apparently, when you calculate the component form of v with `v = v1*i + v2 * j+ v3 * k`, you can *'normalize'* the vectors so your resulting unit vector has **the same direction and length** as your original vector. This makes it easier to work in Physics and more applied scenarios of vectors, as we work independent of units of measurement.

You can normalize your vector by dividing each component by the length of the vector:
`v = (v1/|v|) * i + (v2/|v|) * j + (v3/|v|) * k`

This is not necessary if you only work in Maths, but keep it in mind if you are applying the direction formula to forces, or real-world scenarios.

# Expressing a vectors in terms of its length and direction

![[Pasted image 20231024144450.png]]

It takes into account [[Vectors#The direction of a nonzero vector v|the direction of a vector]] and its [[Vectors#The length (magnitude) of a vector|length]] to express it in the equation of step 2.

# The midpoint of a line segment P1P2

![[Pasted image 20231024144633.png]]

				![[Pasted image 20231024144641.png]]

#maths #calculus1a #vector


