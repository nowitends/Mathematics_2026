# Exercise 10. Projection of a Point onto a Plane

## Given

We are given:

$$
P=(2,1,3)
$$

The plane is:

$$
x+y+z=3
$$

We need to find the orthogonal projection, the reflection of P, and check the midpoint.

## Solution

### 1. Finding the Normal Vector

From the plane equation, the normal vector is:

$$
n=(1,1,1)
$$

### 2. Finding the Projection

I use the projection formula:

$$
Q=P-\frac{n\cdot P-3}{n\cdot n}n
$$

First, I calculate:

$$
n\cdot P=2+1+3=6
$$

And:

$$
n\cdot n=1+1+1=3
$$

Now I substitute:

$$
Q=(2,1,3)-\frac{6-3}{3}(1,1,1)
$$

$$
Q=(2,1,3)-(1,1,1)
$$

Therefore:

$$
\boxed{Q=(1,0,2)}
$$

### 3. Finding the Reflection

The reflection point is found by:

$$
P'=2Q-P
$$

Substituting:

$$
P'=2(1,0,2)-(2,1,3)
$$

$$
=(2,0,4)-(2,1,3)
$$

Therefore:

$$
\boxed{P'=(0,-1,1)}
$$

### 4. Checking the Midpoint

I calculate the midpoint between P and P':

$$
M=\frac{P+P'}{2}
$$

$$
M=\frac{(2,1,3)+(0,-1,1)}{2}
$$

$$
\boxed{M=(1,0,2)}
$$

Now I check if the midpoint is on the plane:

$$
1+0+2=3
$$

The result is correct.

Therefore, the midpoint lies on the plane.

## Conclusion

The orthogonal projection is:

$$
\boxed{Q=(1,0,2)}
$$

The reflection point is:

$$
\boxed{P'=(0,-1,1)}
$$

The midpoint is also (1,0,2), and it lies on the plane.