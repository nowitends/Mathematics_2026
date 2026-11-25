# Exercise 7. A Line Relative to a Plane

## Given

We are given a line:

$$
L:(x,y,z)=(1,1,0)+t(1,-1,0)
$$

And a plane:

$$
\Pi:x+y+z=2
$$

We need to determine the position of the line relative to the plane.

## Solution

### 1. Finding the Direction and Normal Vectors

The direction vector of the line is:

$$
v=(1,-1,0)
$$

The normal vector of the plane is:

$$
n=(1,1,1)
$$

### 2. Calculating the Dot Product

I calculate:

$$
v\cdot n=1(1)+(-1)(1)+0(1)
$$

$$
=1-1+0
$$

$$
\boxed{v\cdot n=0}
$$

This means that the direction vector is perpendicular to the normal vector.

Therefore, the line is parallel to the plane or lies in it.

### 3. Checking a Point on the Line

A point on the line is:

$$
P=(1,1,0)
$$

I substitute it into the plane equation:

$$
1+1+0=2
$$

The equation is correct.

Therefore, the point lies in the plane.

### 4. Final Decision

The direction vector is parallel to the plane, and one point of the line belongs to the plane.

Therefore, the whole line lies in the plane.

## Conclusion

The line lies in the plane.

$$
\boxed{L\subset\Pi}
$$