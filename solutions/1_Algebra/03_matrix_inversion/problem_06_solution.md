# Exercise 6 – Solving a System Using the Inverse

## Question

Solve:

$$
Ax=b
$$

where:

$$
A=
\begin{pmatrix}
2&1\\
1&3
\end{pmatrix},
\qquad
b=
\begin{pmatrix}
5\\
7
\end{pmatrix}
$$

using $x=A^{-1}b$. Then substitute the resulting vector back into the equation and check the result.

## Solution

### 1. Calculate the Determinant

For a 2x2 matrix:

$$
\det(A)=ad-bc
$$

Substituting the values:

$$
\det(A)=(2)(3)-(1)(1)
$$

$$
=6-1=5
$$

Therefore:

$$
\boxed{\det(A)=5}
$$

Since the determinant is not zero, the inverse exists.

### 2. Calculate the Inverse

The inverse formula is:

$$
A^{-1}=
\frac{1}{ad-bc}
\begin{pmatrix}
d&-b\\
-c&a
\end{pmatrix}
$$

Substituting the values:

$$
A^{-1}=
\frac15
\begin{pmatrix}
3&-1\\
-1&2
\end{pmatrix}
$$

Therefore:

$$
\boxed{
A^{-1}=
\begin{pmatrix}
\frac35&-\frac15\\
-\frac15&\frac25
\end{pmatrix}
}
$$

### 3. Calculate x

Using the formula:

$$
x=A^{-1}b
$$

Substituting the values:

$$
x=
\frac15
\begin{pmatrix}
3&-1\\
-1&2
\end{pmatrix}
\begin{pmatrix}
5\\
7
\end{pmatrix}
$$

$$
=
\frac15
\begin{pmatrix}
15-7\\
-5+14
\end{pmatrix}
$$

$$
=
\frac15
\begin{pmatrix}
8\\
9
\end{pmatrix}
$$

Therefore:

$$
\boxed{
x=
\begin{pmatrix}
\frac85\\
\frac95
\end{pmatrix}
}
$$

### 4. Verify the Result

Substitute x into the original equation:

$$
Ax=b
$$

$$
\begin{pmatrix}
2&1\\
1&3
\end{pmatrix}
\begin{pmatrix}
\frac85\\
\frac95
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
\frac{16}{5}+\frac95\\
\frac85+\frac{27}{5}
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
\frac{25}{5}\\
\frac{35}{5}
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
5\\
7
\end{pmatrix}
$$

Thus:

$$
\boxed{Ax=b}
$$

### 5. Conclusion

The solution is:

$$
\boxed{
x=
\begin{pmatrix}
\frac85\\
\frac95
\end{pmatrix}
}
$$

Substituting the result into the original equation gives the correct vector b.

Therefore, the solution is correct.