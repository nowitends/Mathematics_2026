# Exercise 7 – Inverse of a Product

## Question

Given:

$$
A=\begin{pmatrix}1&1\\0&1\end{pmatrix},
\quad
B=\begin{pmatrix}2&0\\0&3\end{pmatrix}
$$

Compute $(AB)^{-1}$ and $B^{-1}A^{-1}$.

## Solution

### 1. Calculate AB

$$
AB=
\begin{pmatrix}1&1\\0&1\end{pmatrix}
\begin{pmatrix}2&0\\0&3\end{pmatrix}
$$

$$
AB=
\begin{pmatrix}2&3\\0&3\end{pmatrix}
$$

### 2. Calculate the Determinant

$$
\det(AB)=(2)(3)-(3)(0)
$$

$$
\det(AB)=6
$$

Since the determinant is not zero, the inverse exists.

### 3. Calculate the Inverse of AB

$$
(AB)^{-1}
=
\frac{1}{6}
\begin{pmatrix}3&-3\\0&2\end{pmatrix}
$$

Therefore:

$$
\boxed{
(AB)^{-1}=
\begin{pmatrix}
\frac12&-\frac12\\
0&\frac13
\end{pmatrix}
}
$$

### 4. Calculate B⁻¹ and A⁻¹

$$
B^{-1}=
\begin{pmatrix}
\frac12&0\\
0&\frac13
\end{pmatrix}
$$

$$
A^{-1}=
\begin{pmatrix}
1&-1\\
0&1
\end{pmatrix}
$$

### 5. Calculate B⁻¹A⁻¹

$$
B^{-1}A^{-1}
=
\begin{pmatrix}
\frac12&0\\
0&\frac13
\end{pmatrix}
\begin{pmatrix}
1&-1\\
0&1
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
\frac12&-\frac12\\
0&\frac13
\end{pmatrix}
$$

Therefore:

$$
\boxed{(AB)^{-1}=B^{-1}A^{-1}}
$$

### 6. Conclusion

Both results are equal.

The inverse of a product reverses the order of the matrices.

This confirms the inverse-of-a-product property.