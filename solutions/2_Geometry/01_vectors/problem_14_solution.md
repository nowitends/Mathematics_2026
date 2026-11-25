# Exercise 14. Closest Point on a Line

## Given

We are given a point:

$$
P=(4,1)
$$

The line passes through the origin and has direction:

$$
v=(1,2)
$$

We need to find the closest point on the line, calculate the distance, and check perpendicularity.

## Solution

### 1. Finding the Closest Point

I use the projection formula:

$$
Q=\operatorname{proj}_v P
=\frac{P\cdot v}{v\cdot v}v
$$

First, I calculate the dot products:

$$
P\cdot v=4(1)+1(2)=6
$$

$$
v\cdot v=1^2+2^2=5
$$

Now I substitute:

$$
Q=\frac65(1,2)
$$

Therefore:

$$
\boxed{Q=\left(\frac65,\frac{12}{5}\right)}
$$

This is the closest point on the line.

### 2. Calculating the Distance

I calculate the difference between P and Q:

$$
P-Q=(4,1)-\left(\frac65,\frac{12}{5}\right)
$$

$$
=\left(\frac{14}{5},-\frac75\right)
$$

Now I calculate its length:

$$
d=\sqrt{\left(\frac{14}{5}\right)^2+
\left(-\frac75\right)^2}
$$

$$
=\sqrt{\frac{196}{25}+\frac{49}{25}}
$$

$$
=\sqrt{\frac{245}{25}}
$$

Therefore:

$$
\boxed{d=\frac{7\sqrt5}{5}}
$$

### 3. Checking Perpendicularity

The vector from Q to P should be perpendicular to the direction of the line.

I check the dot product:

$$
(P-Q)\cdot v
$$

$$
=\left(\frac{14}{5},-\frac75\right)
\cdot(1,2)
$$

$$
=\frac{14}{5}-\frac{14}{5}
$$

$$
=0
$$

The dot product is zero, so the vectors are perpendicular.

## Conclusion

The closest point on the line is:

$$
Q=\left(\frac65,\frac{12}{5}\right)
$$

The distance from P to the line is:

$$
d=\frac{7\sqrt5}{5}
$$

The perpendicularity check is also correct because the dot product equals zero.