# Exercise 13. Closest Point on a Plane

## Given

The point is:

$$
P=(3,0,0)
$$

The plane is:

$$
x+2y+2z=4
$$

We need to find the closest point on the plane, calculate the distance, and check perpendicularity.

## Solution

### 1. Finding the Normal Vector

From the plane equation, the normal vector is:

$$
n=(1,2,2)
$$

### 2. Finding the Closest Point

I use the projection formula:

$$
Q=P-\frac{n\cdot P-4}{n\cdot n}n
$$

First, I calculate:

$$
n\cdot P=1(3)+2(0)+2(0)=3
$$

And:

$$
n\cdot n=1^2+2^2+2^2=9
$$

Now I substitute:

$$
Q=(3,0,0)-\frac{3-4}{9}(1,2,2)
$$

$$
Q=(3,0,0)+\frac19(1,2,2)
$$

Therefore:

$$
\boxed{Q=\left(\frac{28}{9},\frac29,\frac29\right)}
$$

### 3. Checking the Plane

I substitute Q into the plane equation:

$$
\frac{28}{9}+2\left(\frac29\right)
+2\left(\frac29\right)=4
$$

$$
\frac{36}{9}=4
$$

The point lies on the plane.

### 4. Calculating the Distance

I use the distance formula:

$$
d=\frac{|3-4|}{\sqrt{1^2+2^2+2^2}}
$$

$$
d=\frac{1}{3}
$$

Therefore:

$$
\boxed{d=\frac13}
$$

### 5. Checking Perpendicularity

I calculate the vector from P to Q:

$$
Q-P=
\left(\frac19,\frac29,\frac29\right)
$$

This vector is:

$$
Q-P=\frac19(1,2,2)
$$

It is a multiple of the normal vector.

Therefore, the segment is perpendicular to the plane.

## Conclusion

The closest point is:

$$
\boxed{Q=\left(\frac{28}{9},\frac29,\frac29\right)}
$$

The distance is:

$$
\boxed{d=\frac13}
$$

The segment is perpendicular to the plane because it has the same direction as the normal vector.