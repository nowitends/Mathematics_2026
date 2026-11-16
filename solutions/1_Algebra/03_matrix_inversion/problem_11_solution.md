# Exercise 11 – Parameter and Invertibility

## Question

For the matrix:

$$
A(t)=
\begin{pmatrix}
1&t\\
t&1
\end{pmatrix}
$$

Find all values of t for which the matrix is invertible. Give a formula for the inverse and explain what happens at the excluded values.

## Solution

### 1. Calculate the Determinant

For a 2x2 matrix:

$$
\det(A)=ad-bc
$$

For the given matrix:

$$
\det(A(t))=
\begin{vmatrix}
1&t\\
t&1
\end{vmatrix}
$$

$$
\det(A(t))=(1)(1)-(t)(t)
$$

$$
\boxed{\det(A(t))=1-t^2}
$$

### 2. Find the Values of t

The matrix is invertible when its determinant is not zero.

$$
1-t^2\neq 0
$$

$$
t^2\neq 1
$$

Therefore:

$$
\boxed{t\neq 1,\quad t\neq -1}
$$

The matrix is invertible for all other values of t.

### 3. Calculate the Inverse

Using the inverse formula:

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
A(t)^{-1}=
\frac{1}{1-t^2}
\begin{pmatrix}
1&-t\\
-t&1
\end{pmatrix}
$$

Therefore:

$$
\boxed{
A(t)^{-1}=
\frac{1}{1-t^2}
\begin{pmatrix}
1&-t\\
-t&1
\end{pmatrix}
}
$$

For:

$$
t\neq \pm1
$$

### 4. Explain the Excluded Values

When t = 1:

$$
A(1)=
\begin{pmatrix}
1&1\\
1&1
\end{pmatrix}
$$

The two rows are equal.

Therefore, the determinant is zero and the inverse does not exist.

When t = -1:

$$
A(-1)=
\begin{pmatrix}
1&-1\\
-1&1
\end{pmatrix}
$$

The second row is the negative of the first row.

Therefore, the determinant is zero and the inverse does not exist.

### 5. Conclusion

The matrix is invertible when:

$$
\boxed{t\neq 1,\quad t\neq -1}
$$

Its inverse is:

$$
\boxed{
A(t)^{-1}=
\frac{1}{1-t^2}
\begin{pmatrix}
1&-t\\
-t&1
\end{pmatrix}
}
$$

At t = 1 and t = -1, the inverse does not exist because the determinant is zero.