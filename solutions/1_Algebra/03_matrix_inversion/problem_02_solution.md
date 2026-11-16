# Exercise 2 – Formula for a 2×2 Matrix

## Question

Find the inverse of

$$
A =
\begin{pmatrix}
3 & 2 \\
5 & 4
\end{pmatrix}
$$

using the formula for a 2×2 matrix.

At the end, check the result by computing one product with A.

## Solution

### 1. Calculate the determinant

For a 2×2 matrix:

$$
A =
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
$$

The determinant is:

$$
\det(A)=ad-bc
$$

For the given matrix:

$$
\det(A)=(3)(4)-(2)(5)
$$

$$
=12-10
$$

$$
\boxed{\det(A)=2}
$$

Since the determinant is not zero, the inverse exists.

### 2. Apply the inverse formula

The inverse formula for a 2×2 matrix is:

$$
A^{-1}=
\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}
$$

Substituting the values:

$$
A^{-1}=
\frac{1}{2}
\begin{pmatrix}
4 & -2 \\
-5 & 3
\end{pmatrix}
$$

Therefore:

$$
\boxed{
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}
}
$$

### 3. Verify the result

To verify the inverse, calculate $AA^{-1}$:

$$
AA^{-1}=
\begin{pmatrix}
3 & 2 \\
5 & 4
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
6-5 & -3+3 \\
10-10 & -5+6
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
$$

Thus:

$$
\boxed{AA^{-1}=I}
$$

### 4. Conclusion

The determinant of A is 2, which is nonzero. Therefore, the inverse exists.

The calculated inverse gives the identity matrix when multiplied by A.

Hence, the result is correct.