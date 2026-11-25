# Exercise 13. Do Four Points Lie in One Plane?

## Given Points

We are given four points:

$$
A=(0,0,0)
$$

$$
B=(1,2,0)
$$

$$
C=(0,1,1)
$$

$$
D=(2,5,1)
$$

We need to check if all four points lie in the same plane.

## Solution

### 1. Constructing AB and AC

First, I calculate AB:

$$
\overrightarrow{AB}=B-A
$$

$$
=(1,2,0)
$$

Now I calculate AC:

$$
\overrightarrow{AC}=C-A
$$

$$
=(0,1,1)
$$

### 2. Finding the Normal Vector

I calculate the cross product:

$$
n=\overrightarrow{AB}\times\overrightarrow{AC}
$$

$$
=
\begin{vmatrix}
i&j&k\\
1&2&0\\
0&1&1
\end{vmatrix}
$$

Expanding the determinant:

$$
n=(2(1)-0(1),
0(0)-1(1),
1(1)-2(0))
$$

Therefore:

$$
\boxed{n=(2,-1,1)}
$$

### 3. Constructing AD and Checking the Dot Product

First, I calculate AD:

$$
\overrightarrow{AD}=D-A
$$

$$
=(2,5,1)
$$

Now I check the dot product with the normal vector:

$$
\overrightarrow{AD}\cdot n
=2(2)+5(-1)+1(1)
$$

$$
=4-5+1
$$

$$
\boxed{\overrightarrow{AD}\cdot n=0}
$$

### 4. Checking if D Lies in the Plane

The dot product is zero, which means AD is perpendicular to the normal vector.

Therefore, AD lies in the plane determined by A, B and C.

So point D also lies in the same plane.

## Conclusion

Since:

$$
\overrightarrow{AD}\cdot n=0
$$

point D belongs to the plane determined by A, B and C.

Therefore, all four points lie in the same plane.