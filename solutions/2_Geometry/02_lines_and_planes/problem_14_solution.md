# Exercise 14. Contrast: Intersection and Parallelism

## Given

The starting point is:

$$
P=(0,0,1)
$$

The direction vectors are:

$$
v_1=(2,1,-1)
$$

$$
v_2=(2,1,0)
$$

The plane is:

$$
z=0
$$

## Solution

### 1. First Line

The first line is:

$$
L_1=(0,0,1)+t(2,1,-1)
$$

Its coordinates are:

$$
x=2t,\quad y=t,\quad z=1-t
$$

To find the intersection with the plane, I set z=0:

$$
1-t=0
$$

$$
t=1
$$

I substitute t=1:

$$
x=2,\quad y=1,\quad z=0
$$

Therefore, the intersection point is:

$$
\boxed{(2,1,0)}
$$

The first line intersects the plane at one point.

### 2. Second Line

The second line is:

$$
L_2=(0,0,1)+t(2,1,0)
$$

Its coordinates are:

$$
x=2t,\quad y=t,\quad z=1
$$

The z-coordinate is always 1.

The plane has z=0, so the line never reaches the plane.

The direction vector has no z-component, which means it is parallel to the plane.

Therefore, the second line is parallel to the plane and has no common points with it.

## Conclusion

- The first line intersects the plane at (2,1,0).
- The second line is parallel to the plane and does not intersect it.

The difference is the z-component of the direction vectors.