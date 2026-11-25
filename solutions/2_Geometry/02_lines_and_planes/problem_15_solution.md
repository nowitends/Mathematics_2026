# Exercise 15. Complete Classification of a Line Relative to a Plane

## Given

The line is:

$$
L:p+tv
$$

The plane is:

$$
\Pi:n\cdot x=d
$$

We need to describe the three possible cases.

## Solution

I substitute the line into the plane equation:

$$
n\cdot(p+tv)=d
$$

Using the dot product:

$$
n\cdot p+t(n\cdot v)=d
$$

### 1. One Intersection Point

If:

$$
n\cdot v\neq 0
$$

There is one solution for t:

$$
t=\frac{d-n\cdot p}{n\cdot v}
$$

This means the line intersects the plane at one point.

Example:

The plane is:

$$
x+y+z=3
$$

The line is:

$$
(x,y,z)=(0,0,0)+t(1,0,0)
$$

Substituting into the plane:

$$
t=3
$$

The intersection point is:

$$
\boxed{(3,0,0)}
$$

### 2. Parallel with No Common Points

If:

$$
n\cdot v=0
$$

and

$$
n\cdot p\neq d
$$

The line is parallel to the plane but does not lie in it.

Example:

The plane is:

$$
z=0
$$

The line is:

$$
(x,y,z)=(0,0,1)+t(1,2,0)
$$

The z-coordinate is always 1.

Therefore, the line never reaches the plane.

There are no common points.

### 3. The Line Lies in the Plane

If:

$$
n\cdot v=0
$$

and

$$
n\cdot p=d
$$

The line is completely inside the plane.

Example:

The plane is:

$$
z=0
$$

The line is:

$$
(x,y,z)=(1,2,0)+t(2,1,0)
$$

The z-coordinate is always 0.

Both the starting point and the direction keep the line in the plane.

Therefore, the whole line lies in the plane.

## Conclusion

There are three possible cases:

1. If n·v is not zero, there is one intersection point.
2. If n·v is zero and n·p is not equal to d, the line is parallel to the plane with no common points.
3. If n·v is zero and n·p equals d, the line lies in the plane.

These conditions help us understand the position of a line relative to a plane without solving unnecessary equations.