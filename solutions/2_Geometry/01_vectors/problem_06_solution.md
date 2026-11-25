# Exercise 6. Projection and Perpendicular Component

## Given Vectors

We are given:

$$
u=(4,2), \quad v=(1,1)
$$

We need to find the projection of u onto v, calculate the perpendicular component r, and check that r is perpendicular to v.

## Solution

### 1. Finding the Projection

I use the projection formula:

$$
\operatorname{proj}_v u =
\frac{u\cdot v}{v\cdot v}v
$$

First, I calculate the dot products:

$$
u\cdot v=4(1)+2(1)=6
$$

$$
v\cdot v=1^2+1^2=2
$$

Now I substitute:

$$
\operatorname{proj}_v u =
\frac{6}{2}(1,1)
$$

$$
=3(1,1)
$$

Therefore:

$$
\boxed{\operatorname{proj}_v u=(3,3)}
$$

### 2. Finding the Perpendicular Component

The question gives:

$$
r=u-\operatorname{proj}_v u
$$

I substitute the values:

$$
r=(4,2)-(3,3)
$$

$$
\boxed{r=(1,-1)}
$$

### 3. Checking Perpendicularity

To check if r is perpendicular to v, I calculate their dot product:

$$
r\cdot v=1(1)+(-1)(1)
$$

$$
r\cdot v=1-1=0
$$

Since the dot product is zero, the two vectors are perpendicular.

### 4. Geometrical Explanation

The projection is the part of u that goes in the direction of v.

The remaining vector r is perpendicular to v. Together, the projection and r give the original vector u.

## Conclusion

The results are:

$$
\operatorname{proj}_v u=(3,3)
$$

$$
r=(1,-1)
$$

And:

$$
r\cdot v=0
$$

So the perpendicularity condition is satisfied.