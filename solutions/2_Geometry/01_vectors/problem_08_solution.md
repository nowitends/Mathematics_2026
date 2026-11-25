# Exercise 8. Linear Combination and Checking the Result

## Given Vectors

We are given:

$$
w=(5,1), \quad u=(1,1), \quad v=(2,-1)
$$

We need to check if w can be written as:

$$
w=au+bv
$$

If possible, we need to find a and b, reconstruct w, and explain the geometric meaning.

## Solution

### 1. Finding the Coefficients

First, I substitute the vectors into the equation:

$$
(5,1)=a(1,1)+b(2,-1)
$$

This gives two equations:

$$
a+2b=5
$$

$$
a-b=1
$$

From the second equation:

$$
a=1+b
$$

Now I substitute this into the first equation:

$$
1+b+2b=5
$$

$$
3b=4
$$

$$
b=\frac{4}{3}
$$

Then:

$$
a=1+\frac{4}{3}
$$

$$
a=\frac{7}{3}
$$

### 2. Reconstructing the Vector

Now I put the values of a and b into the original equation:

$$
w=\frac{7}{3}u+\frac{4}{3}v
$$

$$
=\frac{7}{3}(1,1)+\frac{4}{3}(2,-1)
$$

$$
=\left(\frac{7}{3},\frac{7}{3}\right)
+\left(\frac{8}{3},-\frac{4}{3}\right)
$$

$$
=\left(\frac{15}{3},\frac{3}{3}\right)
$$

$$
\boxed{w=(5,1)}
$$

This is the same as the given vector.

### 3. Geometrical Meaning

The vector w can be made by combining u and v with the coefficients a and b.

This means that w can be reached using these two vector directions.

## Conclusion

The vector w can be written as a linear combination of u and v.

The coefficients are:

$$
\boxed{a=\frac{7}{3}, \quad b=\frac{4}{3}}
$$

The result is correct because we get the original vector w.