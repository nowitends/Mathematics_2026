# Exercise 13 – Undoing a Composite Transformation

## Question

The matrices

$$
S=
\begin{pmatrix}
2&0\\
0&1
\end{pmatrix},
\qquad
H=
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
$$

describe nonuniform scaling and shear. For $T=HS$, find $T^{-1}$ in two ways:

1. First compute $T$, then its inverse.
2. Use the product inverse property $(HS)^{-1}=S^{-1}H^{-1}$.

Compare the results. Additionally, compute $H^{-1}S^{-1}$ and verify that the incorrect order gives a different matrix. Explain why, when undoing a composition of operations, we undo them from the end.

## Solution

### 1. Calculate T = HS

$$
T=HS
$$

$$
T=
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
\begin{pmatrix}
2&0\\
0&1
\end{pmatrix}
$$

$$
T=
\begin{pmatrix}
2&1\\
0&1
\end{pmatrix}
$$

### 2. Find the Inverse of T Directly

The determinant is:

$$
\det(T)=(2)(1)-(1)(0)=2
$$

Since the determinant is not zero, the inverse exists.

Using the inverse formula:

$$
T^{-1}
=
\frac12
\begin{pmatrix}
1&-1\\
0&2
\end{pmatrix}
$$

Therefore:

$$
\boxed{
T^{-1}=
\begin{pmatrix}
\frac12&-\frac12\\
0&1
\end{pmatrix}
}
$$

### 3. Find the Inverse Using the Product Rule

For a product of two invertible matrices, the inverse property is:

$$
(HS)^{-1}=S^{-1}H^{-1}
$$

First, calculate the inverse of S:

$$
S^{-1}=
\begin{pmatrix}
\frac12&0\\
0&1
\end{pmatrix}
$$

Now, calculate the inverse of H:

$$
H^{-1}=
\begin{pmatrix}
1&-1\\
0&1
\end{pmatrix}
$$

Multiply them in the correct order:

$$
S^{-1}H^{-1}
=
\begin{pmatrix}
\frac12&0\\
0&1
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
0&1
\end{pmatrix}
$$

Thus:

$$
\boxed{
S^{-1}H^{-1}=
\begin{pmatrix}
\frac12&-\frac12\\
0&1
\end{pmatrix}
}
$$

Both methods give the same result:

$$
T^{-1}=S^{-1}H^{-1}
$$

### 4. Calculate the Incorrect Order H⁻¹S⁻¹

Now calculate the reversed order:

$$
H^{-1}S^{-1}
=
\begin{pmatrix}
1&-1\\
0&1
\end{pmatrix}
\begin{pmatrix}
\frac12&0\\
0&1
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
\frac12&-1\\
0&1
\end{pmatrix}
$$

This is different from the correct inverse:

$$
H^{-1}S^{-1}
\neq
S^{-1}H^{-1}
$$

### 5. Verify the Correct Inverse

Multiply T by its correct inverse:

$$
TT^{-1}
=
\begin{pmatrix}
2&1\\
0&1
\end{pmatrix}
\begin{pmatrix}
\frac12&-\frac12\\
0&1
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
1&0\\
0&1
\end{pmatrix}
=I
$$

The reverse multiplication also gives:

$$
T^{-1}T=I
$$

The incorrect order does not give the identity matrix:

$$
T(H^{-1}S^{-1})
=
\begin{pmatrix}
\frac12&-1\\
0&1
\end{pmatrix}
\neq I
$$

### 6. Explanation of the Reversed Order

In $T=HS$, the matrix $S$ acts first and then $H$.

To undo this composition, we must first undo $H$ using $H^{-1}$ and then undo $S$ using $S^{-1}$.

This is why the order of the matrices is reversed when taking the inverse of a product:

$$
\boxed{
(HS)^{-1}=S^{-1}H^{-1}
}
$$

**Conclusion**

Both methods give the same inverse matrix:

$$
\boxed{
T^{-1}=
\begin{pmatrix}
\frac12&-\frac12\\
0&1
\end{pmatrix}
}
$$

The incorrect order gives a different matrix and does not produce the identity when multiplied by $T$. This confirms that the order must be reversed when undoing a composition of transformations.