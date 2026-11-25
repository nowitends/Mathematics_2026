# Exercise 9. Cross Product as a Perpendicular Direction

## Given Vectors

We are given:

$$
u=(1,2,0), \quad v=(0,1,3)
$$

We need to calculate u × v, check if it is perpendicular to both vectors, and compare it with v × u.

## Solution

### 1. Calculating the Cross Product

I use the cross product formula:

$$
u\times v=
\begin{vmatrix}
i&j&k\\
1&2&0\\
0&1&3
\end{vmatrix}
$$

Expanding the determinant:

$$
u\times v=
(2\cdot3-0\cdot1,\,
0\cdot0-1\cdot3,\,
1\cdot1-2\cdot0)
$$

Therefore:

$$
\boxed{u\times v=(6,-3,1)}
$$

### 2. Checking Perpendicularity to u

I calculate the dot product:

$$
(u\times v)\cdot u
$$

$$
=6(1)+(-3)(2)+1(0)
$$

$$
=6-6+0=0
$$

So the cross product is perpendicular to u.

### 3. Checking Perpendicularity to v

Now I calculate:

$$
(u\times v)\cdot v
$$

$$
=6(0)+(-3)(1)+1(3)
$$

$$
=0-3+3=0
$$

So the cross product is also perpendicular to v.

### 4. Calculating v × u

Now I change the order of the vectors:

$$
v\times u=
\begin{vmatrix}
i&j&k\\
0&1&3\\
1&2&0
\end{vmatrix}
$$

$$
v\times u=(-6,3,-1)
$$

Therefore:

$$
\boxed{v\times u=-(u\times v)}
$$

### 5. Comparing the Results

The two results have opposite directions but the same length.

Changing the order of the vectors changes the direction of the cross product.

## Conclusion

The cross product is:

$$
u\times v=(6,-3,1)
$$

It is perpendicular to both original vectors because both dot products are zero.

Also:

$$
v\times u=(-6,3,-1)
$$

This shows that changing the order changes the sign of the result.