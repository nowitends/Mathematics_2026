# Exercise 12. Intersection Line of Two Planes

## Given

The two planes are:

$$
x+y+z=3
$$

$$
x-y+z=1
$$

We need to find their intersection line and its direction vector in two ways.

## Solution

### 1. Finding the Intersection Line

I subtract the second equation from the first:

$$
(x+y+z)-(x-y+z)=3-1
$$

$$
2y=2
$$

$$
y=1
$$

I substitute y=1 into the first equation:

$$
x+1+z=3
$$

$$
x+z=2
$$

I choose x=t. Then:

$$
z=2-t
$$

Therefore, the parametric equation is:

$$
\boxed{(x,y,z)=(0,1,2)+t(1,0,-1)}
$$

### 2. Finding the Direction Vector from the Equations

From the parametric equation, the direction vector is:

$$
\boxed{v=(1,0,-1)}
$$

### 3. Finding the Direction Vector Using Cross Product

The normal vectors of the planes are:

$$
n_1=(1,1,1)
$$

$$
n_2=(1,-1,1)
$$

I calculate their cross product:

$$
v=n_1\times n_2
$$

$$
v=(2,0,-2)
$$

Dividing by 2:

$$
\boxed{v=(1,0,-1)}
$$

### 4. Comparing the Results

Both methods give the same direction vector.

## Conclusion

The intersection line is:

$$
\boxed{(x,y,z)=(0,1,2)+t(1,0,-1)}
$$

The two methods give the same direction because the cross product of the normal vectors is perpendicular to both normals.