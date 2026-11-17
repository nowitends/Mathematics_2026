# Exercise 12 – Finding Inverses Without Starting from Scratch

## Question

It is known that

$$
A^{-1}=
\begin{pmatrix}
2&-1\\
-3&2
\end{pmatrix}
$$

Without finding $A$, compute $(3A)^{-1}$, $(A^T)^{-1}$, and $(A^2)^{-1}$. Justify each result using the appropriate property.

## Solution

### 1. Calculate (3A)⁻¹

Using the scalar inverse property:

$$
(kA)^{-1}=\frac{1}{k}A^{-1}
$$

Therefore:

$$
(3A)^{-1}=\frac{1}{3}A^{-1}
$$

Substitute the given inverse:

$$
(3A)^{-1}
=
\frac{1}{3}
\begin{pmatrix}
2&-1\\
-3&2
\end{pmatrix}
$$

$$
\boxed{
(3A)^{-1}=
\begin{pmatrix}
\frac23&-\frac13\\
-1&\frac23
\end{pmatrix}
}
$$

### 2. Calculate (Aᵀ)⁻¹

Using the transpose inverse property:

$$
(A^T)^{-1}=(A^{-1})^T
$$

We transpose the given inverse matrix:

$$
(A^T)^{-1}
=
\begin{pmatrix}
2&-1\\
-3&2
\end{pmatrix}^{T}
$$

$$
\boxed{
(A^T)^{-1}
=
\begin{pmatrix}
2&-3\\
-1&2
\end{pmatrix}
}
$$

### 3. Calculate (A²)⁻¹

Using the inverse of a product property:

$$
(A^2)^{-1}=(AA)^{-1}=A^{-1}A^{-1}
$$

Therefore:

$$
(A^2)^{-1}
=
\begin{pmatrix}
2&-1\\
-3&2
\end{pmatrix}
\begin{pmatrix}
2&-1\\
-3&2
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
4+3&-2-2\\
-6-6&3+4
\end{pmatrix}
$$

$$
\boxed{
(A^2)^{-1}
=
\begin{pmatrix}
7&-4\\
-12&7
\end{pmatrix}
}
$$

### 4. Verify the Results

Each result follows from a standard inverse property:

- Scalar multiplication: $(3A)^{-1}=\frac13A^{-1}$.
- Transpose: $(A^T)^{-1}=(A^{-1})^T$.
- Product: $(A^2)^{-1}=A^{-1}A^{-1}$.

These properties allow us to calculate all three inverses without finding the original matrix $A$.

**Conclusion**

The three results are obtained directly from inverse matrix properties. No full calculation of $A$ is necessary.