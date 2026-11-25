# Exercise 8. Two Systems with the Same Coefficient Matrix

## Given Systems

We are given two systems:

**First system:**

$$
\begin{cases}
2x+y=5\\
x-y=1
\end{cases}
$$

**Second system:**

$$
\begin{cases}
2x+y=1\\
x-y=4
\end{cases}
$$

The task is to solve both systems using elimination and compare the steps. I also need to explain which parts of the calculations are the same and why.

## Solution

### First System

First, I write the system as an augmented matrix:

$$
\left[
\begin{array}{cc|c}
2&1&5\\
1&-1&1
\end{array}
\right]
$$

I eliminate $x$ from the second row using:

$$
R_2\rightarrow R_2-\frac{1}{2}R_1
$$

After this operation, I get:

$$
\left[
\begin{array}{cc|c}
2&1&5\\
0&-\frac{3}{2}&-\frac{3}{2}
\end{array}
\right]
$$

From the second row:

$$
-\frac{3}{2}y=-\frac{3}{2}
$$

Therefore:

$$
y=1
$$

Now I substitute this value into the first equation:

$$
2x+y=5
$$

$$
2x+1=5
$$

$$
2x=4
$$

$$
x=2
$$

The solution of the first system is:

$$
\boxed{(x,y)=(2,1)}
$$

### Second System

Now I solve the second system:

$$
\begin{cases}
2x+y=1\\
x-y=4
\end{cases}
$$

I write it as an augmented matrix:

$$
\left[
\begin{array}{cc|c}
2&1&1\\
1&-1&4
\end{array}
\right]
$$

I use the same row operation as before:

$$
R_2\rightarrow R_2-\frac{1}{2}R_1
$$

The new matrix is:

$$
\left[
\begin{array}{cc|c}
2&1&1\\
0&-\frac{3}{2}&\frac{7}{2}
\end{array}
\right]
$$

From the second row:

$$
-\frac{3}{2}y=\frac{7}{2}
$$

Therefore:

$$
y=-\frac{7}{3}
$$

Now I substitute this value into the first equation:

$$
2x+y=1
$$

$$
2x-\frac{7}{3}=1
$$

$$
2x=\frac{10}{3}
$$

$$
x=\frac{5}{3}
$$

The solution of the second system is:

$$
\boxed{(x,y)=\left(\frac{5}{3},-\frac{7}{3}\right)}
$$

## Comparing the Two Systems

Both systems have the same coefficient matrix:

$$
A=
\begin{pmatrix}
2&1\\
1&-1
\end{pmatrix}
$$

The same row operation is used in both cases:

$$
R_2\rightarrow R_2-\frac{1}{2}R_1
$$

The coefficients in the resulting second row are also the same:

$$
\begin{pmatrix}
0&-\frac{3}{2}
\end{pmatrix}
$$

However, the last number in the augmented matrix is different because the right-hand side values are different.

This is why the elimination steps for the coefficients are the same, but the final solutions are different.

## Conclusion

The solutions are:

**First system:**

$$
\boxed{(x,y)=(2,1)}
$$

**Second system:**

$$
\boxed{(x,y)=\left(\frac{5}{3},-\frac{7}{3}\right)}
$$

Both systems use the same coefficient matrix, so the elimination steps for the variables are the same. Only the right-hand side changes, which leads to different solutions.