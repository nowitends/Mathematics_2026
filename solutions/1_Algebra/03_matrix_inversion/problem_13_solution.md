# Exercise 13. Undoing a Composite Transformation

## Given Matrices

The matrices

$$
S=\begin{pmatrix}
2&0\\
0&1
\end{pmatrix},
\qquad
H=\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
$$

describe nonuniform scaling and shear.

For $T=HS$, find $T^{-1}$ in two ways:

1. First calculate $T$, then find its inverse.
2. Use the property $(HS)^{-1}=S^{-1}H^{-1}$.

Compare the results. Also calculate $H^{-1}S^{-1}$ and verify that the incorrect order gives a different matrix.

## Solution

First, I calculate $T=HS$:

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
=
\begin{pmatrix}
2&1\\
0&1
\end{pmatrix}
$$

### Method 1: Finding the Inverse of T

For a $2\times2$ matrix, I use the inverse formula:

$$
T^{-1}=
\begin{pmatrix}
2&1\\
0&1
\end{pmatrix}^{-1}
$$

$$
T^{-1}=
\begin{pmatrix}
1/2&-1/2\\
0&1
\end{pmatrix}
$$

### Method 2: Using the Inverse Property

The inverse of a product reverses the order of the matrices:

$$
(HS)^{-1}=S^{-1}H^{-1}
$$

First, I calculate the inverse of each matrix:

$$
S^{-1}=
\begin{pmatrix}
1/2&0\\
0&1
\end{pmatrix}
$$

$$
H^{-1}=
\begin{pmatrix}
1&-1\\
0&1
\end{pmatrix}
$$

Now I multiply them in the correct order:

$$
S^{-1}H^{-1}
=
\begin{pmatrix}
1/2&0\\
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
1/2&-1/2\\
0&1
\end{pmatrix}
$$

Both methods give the same result.

## Checking the Incorrect Order

Now I multiply the inverse matrices in the opposite order:

$$
H^{-1}S^{-1}
=
\begin{pmatrix}
1&-1\\
0&1
\end{pmatrix}
\begin{pmatrix}
1/2&0\\
0&1
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
1/2&-1\\
0&1
\end{pmatrix}
$$

To check this result, I multiply it by $T$:

$$
T(H^{-1}S^{-1})
=
\begin{pmatrix}
2&1\\
0&1
\end{pmatrix}
\begin{pmatrix}
1/2&-1\\
0&1
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
1&-1\\
0&1
\end{pmatrix}
$$

This is not the identity matrix. Therefore, the opposite order does not give the inverse of $T$.

## Conclusion

Both methods give the same inverse:

$$
\boxed{
T^{-1}=
\begin{pmatrix}
1/2&-1/2\\
0&1
\end{pmatrix}
}
$$

This exercise shows that when finding the inverse of a product, the order of the matrices must be reversed. Multiplying them in the wrong order gives a different result.s