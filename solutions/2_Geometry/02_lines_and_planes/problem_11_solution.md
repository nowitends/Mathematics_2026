# Exercise 11. Plane Containing a Line and a Point

## Given

The line is:

$$
(x,y,z)=(1,0,2)+t(1,1,-1)
$$

The point is:

$$
P=(0,2,1)
$$

We need to find the plane containing the line and the point.

## Solution

### 1. Finding Two Direction Vectors

A point on the line is:

$$
A=(1,0,2)
$$

The direction vector of the line is:

$$
v=(1,1,-1)
$$

I find another vector from A to P:

$$
w=P-A
$$

$$
w=(0-1,2-0,1-2)
$$

$$
w=(-1,2,-1)
$$

### 2. Finding the Normal Vector

I use the cross product:

$$
n=v\times w
$$

$$
n=(1,1,-1)\times(-1,2,-1)
$$

$$
\boxed{n=(1,2,3)}
$$

### 3. Finding the Plane Equation

I use the point A and the normal vector:

$$
1(x-1)+2(y-0)+3(z-2)=0
$$

Simplifying:

$$
x-1+2y+3z-6=0
$$

Therefore:

$$
\boxed{x+2y+3z=7}
$$

### 4. Checking the Line

I substitute the line coordinates:

$$
x=1+t,\quad y=t,\quad z=2-t
$$

$$
(1+t)+2t+3(2-t)=7
$$

$$
7=7
$$

The whole line lies in the plane.

### 5. Checking the Point

I substitute P=(0,2,1):

$$
0+2(2)+3(1)=7
$$

$$
7=7
$$

The point also lies in the plane.

## Conclusion

The plane equation is:

$$
\boxed{x+2y+3z=7}
$$

Both the line and the given point lie in this plane.