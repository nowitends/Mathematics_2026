# Exercise 12 – Finding Inverses Without Starting from Scratch

## Question

It is known that:

$$
A^{-1}=
\begin{pmatrix}
2 & -1\\
-3 & 2
\end{pmatrix}
$$

Without finding A, calculate:

1. $(3A)^{-1}$
2. $(A^T)^{-1}$
3. $(A^2)^{-1}$

## Solution

### 1. Calculate the Inverse of 3A

Using the property:

$$
(3A)^{-1}=\frac{1}{3}A^{-1}
$$

Substituting the values:

$$
(3A)^{-1}
=
\frac{1}{3}
\begin{pmatrix}
2 & -1\\
-3 & 2
\end{pmatrix}
$$

Therefore:

$$
\boxed{
(3A)^{-1}=
\begin{pmatrix}
\frac{2}{3} & -\frac{1}{3}\\
-1 & \frac{2}{3}
\end{pmatrix}
}
$$

### 2. Calculate the Inverse of the Transpose

Using the property:

$$
(A^T)^{-1}=(A^{-1})^T
$$

Taking the transpose:

$$
(A^T)^{-1}
=
\begin{pmatrix}
2 & -3\\
-1 & 2
\end{pmatrix}
$$

Therefore:

$$
\boxed{
(A^T)^{-1}=
\begin{pmatrix}
2 & -3\\
-1 & 2
\end{pmatrix}
}
$$

### 3. Calculate the Inverse of A Squared

Using the property:

$$
(A^2)^{-1}=(A^{-1})^2
$$

Substituting the values:

$$
(A^2)^{-1}
=
\begin{pmatrix}
2 & -1\\
-3 & 2
\end{pmatrix}
\begin{pmatrix}
2 & -1\\
-3 & 2
\end{pmatrix}
$$

Multiplying:

$$
=
\begin{pmatrix}
4+3 & -2-2\\
-6-6 & 3+4
\end{pmatrix}
$$

Therefore:

$$
\boxed{
(A^2)^{-1}=
\begin{pmatrix}
7 & -4\\
-12 & 7
\end{pmatrix}
}
$$

### 4. Conclusion

All three results were calculated using inverse matrix properties.

We did not need to find the original matrix A.

Therefore, the results are correct.