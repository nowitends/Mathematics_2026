# Exercise 12. A Normal Vector to a Plane

## Given Points

We are given three points:

$$
A=(1,0,2)
$$

$$
B=(2,1,0)
$$

$$
C=(0,3,1)
$$

We need to construct two vectors in the plane, find a vector perpendicular to both, and check it using dot products.

## Solution

### 1. Constructing Two Vectors

First, I calculate AB:

$$
\overrightarrow{AB}=B-A
$$

$$
=(2-1,1-0,0-2)
$$

$$
\overrightarrow{AB}=(1,1,-2)
$$

Now I calculate AC:

$$
\overrightarrow{AC}=C-A
$$

$$
=(0-1,3-0,1-2)
$$

$$
\overrightarrow{AC}=(-1,3,-1)
$$

### 2. Finding a Normal Vector

I use the cross product of the two vectors:

$$
n=\overrightarrow{AB}\times\overrightarrow{AC}
$$

$$
=
\begin{vmatrix}
i&j&k\\
1&1&-2\\
-1&3&-1
\end{vmatrix}
$$

Expanding the determinant:

$$
n=(1(-1)-(-2)(3),
(-2)(-1)-1(-1),
1(3)-1(-1))
$$

$$
\boxed{n=(5,3,4)}
$$

### 3. Checking Perpendicularity

First, I check the dot product with AB:

$$
n\cdot\overrightarrow{AB}
=5(1)+3(1)+4(-2)
$$

$$
=5+3-8=0
$$

Now I check the dot product with AC:

$$
n\cdot\overrightarrow{AC}
=5(-1)+3(3)+4(-1)
$$

$$
=-5+9-4=0
$$

Both dot products are zero.

This means that n is perpendicular to both vectors.

## Conclusion

The two vectors in the plane are:

$$
\overrightarrow{AB}=(1,1,-2)
$$

$$
\overrightarrow{AC}=(-1,3,-1)
$$

The normal vector is:

$$
\boxed{n=(5,3,4)}
$$

Both dot products are zero, so the normal vector is perpendicular to both vectors in the plane.