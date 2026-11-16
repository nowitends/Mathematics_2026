# Exercise 1 – Definition of the Inverse

## Question

For the matrices

$$
A = \begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix},
\qquad
B = \begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix}
$$

check, without using a formula, whether $B = A^{-1}$.

Compute $AB$ and $BA$ and relate the result to the definition of the inverse.

## Solution

### 1. Compute AB

Using matrix multiplication:

$$
AB =
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
2-1 & -2+2 \\
1-1 & -1+2
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
$$

Therefore:

$$
\boxed{AB=I}
$$

### 2. Compute BA

Similarly:

$$
BA =
\begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
2-1 & 1-1 \\
-2+2 & -1+2
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
$$

Therefore:

$$
\boxed{BA=I}
$$

### 3. Conclusion

The inverse of a matrix is defined by the property:

$$
AB=BA=I
$$

Since both products are equal to the identity matrix:

$$
\boxed{B=A^{-1}}
$$

Thus, B is the inverse of A.

This exercise demonstrates the definition of a matrix inverse through multiplication without using an inverse formula.