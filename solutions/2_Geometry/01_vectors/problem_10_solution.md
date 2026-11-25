# Exercise 10. Triangle Area from Vectors

## Given Points

We are given three points:

$$
A=(0,0,0)
$$

$$
B=(2,1,0)
$$

$$
C=(1,3,2)
$$

We need to construct AB and AC, calculate the area of the parallelogram using the cross product, and then find the area of the triangle.

## Solution

### 1. Finding the Vectors AB and AC

First, I subtract the coordinates of A from B:

$$
\overrightarrow{AB}=B-A
$$

$$
=(2-0,1-0,0-0)
$$

$$
\overrightarrow{AB}=(2,1,0)
$$

Now I calculate AC:

$$
\overrightarrow{AC}=C-A
$$

$$
=(1-0,3-0,2-0)
$$

$$
\overrightarrow{AC}=(1,3,2)
$$

### 2. Calculating the Cross Product

I use the cross product:

$$
\overrightarrow{AB}\times\overrightarrow{AC}
=
\begin{vmatrix}
i&j&k\\
2&1&0\\
1&3&2
\end{vmatrix}
$$

Expanding the determinant:

$$
=(1\cdot2-0\cdot3,\,
0\cdot1-2\cdot2,\,
2\cdot3-1\cdot1)
$$

$$
=(2,-4,5)
$$

### 3. Finding the Parallelogram Area

The area of the parallelogram is the length of the cross product:

$$
A_p=|\overrightarrow{AB}\times\overrightarrow{AC}|
$$

$$
=\sqrt{2^2+(-4)^2+5^2}
$$

$$
=\sqrt{4+16+25}
$$

$$
\boxed{A_p=\sqrt{45}=3\sqrt{5}}
$$

### 4. Finding the Triangle Area

A triangle is half of a parallelogram with the same base and height.

Therefore, I divide the parallelogram area by 2:

$$
A_t=\frac{1}{2}A_p
$$

$$
A_t=\frac{1}{2}\cdot3\sqrt{5}
$$

$$
\boxed{A_t=\frac{3\sqrt{5}}{2}}
$$

### 5. Geometrical Explanation

The cross product gives the area of the parallelogram formed by the two vectors.

The triangle uses the same base and height, but its area is half of the parallelogram.

## Conclusion

The vectors are:

$$
\overrightarrow{AB}=(2,1,0)
$$

$$
\overrightarrow{AC}=(1,3,2)
$$

The parallelogram area is:

$$
\boxed{3\sqrt{5}}
$$

The triangle area is:

$$
\boxed{\frac{3\sqrt{5}}{2}}
$$

We divide by 2 because the triangle is half of the parallelogram.