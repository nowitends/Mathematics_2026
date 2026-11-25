# Exercise 11. Decomposition into Parallel and Perpendicular Components

## Given Vectors

We are given:

$$
u=(3,4), \quad v=(1,2)
$$

We need to decompose u into parallel and perpendicular components. Then we check that their sum is u and that the perpendicular component has a zero dot product with v.

## Solution

### 1. Finding the Parallel Component

First, I use the projection formula:

$$
u_{\parallel}=\frac{u\cdot v}{v\cdot v}v
$$

I calculate the dot products:

$$
u\cdot v=3(1)+4(2)=11
$$

$$
v\cdot v=1^2+2^2=5
$$

Now I substitute:

$$
u_{\parallel}=\frac{11}{5}(1,2)
$$

Therefore:

$$
\boxed{u_{\parallel}=
\left(\frac{11}{5},\frac{22}{5}\right)}
$$

### 2. Finding the Perpendicular Component

I subtract the parallel component from u:

$$
u_{\perp}=u-u_{\parallel}
$$

$$
=(3,4)-\left(\frac{11}{5},\frac{22}{5}\right)
$$

$$
=\left(\frac{15}{5}-\frac{11}{5},
\frac{20}{5}-\frac{22}{5}\right)
$$

Therefore:

$$
\boxed{u_{\perp}=
\left(\frac45,-\frac25\right)}
$$

### 3. Checking the Sum

The first condition is:

$$
u=u_{\parallel}+u_{\perp}
$$

I add the two components:

$$
=\left(\frac{11}{5},\frac{22}{5}\right)
+\left(\frac45,-\frac25\right)
$$

$$
=\left(\frac{15}{5},\frac{20}{5}\right)
$$

$$
=(3,4)
$$

This is equal to the original vector u.

### 4. Checking Perpendicularity

The second condition is:

$$
u_{\perp}\cdot v=0
$$

I calculate:

$$
=\frac45(1)-\frac25(2)
$$

$$
=\frac45-\frac45=0
$$

So the perpendicular component is really perpendicular to v.

### 5. Explanation

These are two different checks.

The first check shows that both components together give the original vector. The second check shows that the perpendicular component has a 90-degree angle with v.

## Conclusion

The two components are:

$$
u_{\parallel}=\left(\frac{11}{5},\frac{22}{5}\right)
$$

$$
u_{\perp}=\left(\frac45,-\frac25\right)
$$

Both conditions are satisfied.