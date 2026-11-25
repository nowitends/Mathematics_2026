# Exercise 4. Plane Through Three Points

## Given

We are given three points:

$$
A=(1,0,0)
$$

$$
B=(0,1,0)
$$

$$
C=(0,0,1)
$$

We need to find the plane through these three points using the cross product.

## Solution

### 1. Constructing Two Vectors

First, I calculate AB:

$$
AB=B-A
$$

$$
AB=(0-1,1-0,0-0)
$$

$$
AB=(-1,1,0)
$$

Now I calculate AC:

$$
AC=C-A
$$

$$
AC=(0-1,0-0,1-0)
$$

$$
AC=(-1,0,1)
$$

### 2. Finding the Normal Vector

I use the cross product:

$$
n=AB\times AC
$$

$$
n=
\begin{vmatrix}
i&j&k\\
-1&1&0\\
-1&0&1
\end{vmatrix}
$$

$$
n=(1,1,1)
$$

Therefore:

$$
\boxed{n=(1,1,1)}
$$

### 3. Finding the Plane Equation

I use point A and the normal vector:

$$
1(x-1)+1(y-0)+1(z-0)=0
$$

Simplifying:

$$
x-1+y+z=0
$$

Therefore:

$$
\boxed{x+y+z=1}
$$

### 4. Checking All Three Points

For A=(1,0,0):

$$
1+0+0=1
$$

For B=(0,1,0):

$$
0+1+0=1
$$

For C=(0,0,1):

$$
0+0+1=1
$$

All three points satisfy the plane equation.

## Conclusion

The normal vector is:

$$
n=(1,1,1)
$$

The equation of the plane is:

$$
\boxed{x+y+z=1}
$$

All three points lie on this plane.