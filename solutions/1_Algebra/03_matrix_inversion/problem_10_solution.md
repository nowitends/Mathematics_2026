# Exercise 10 – Inverse of a Diagonal Matrix

## Question

Given:

$$
D=
\begin{pmatrix}
2&0&0\\
0&-3&0\\
0&0&5
\end{pmatrix},
\qquad
E=
\begin{pmatrix}
2&0&0\\
0&0&0\\
0&0&5
\end{pmatrix}
$$

Without using Gauss-Jordan elimination, decide which matrix is invertible. For the invertible matrix, give the inverse and check the result by multiplication.

## Solution

### 1. Check Whether D Is Invertible

A diagonal matrix is invertible if all its diagonal entries are non-zero.

For matrix $D$, the diagonal entries are $2$, $-3$, and $5$.

All diagonal entries are non-zero, so $D$ is invertible.

### 2. Calculate the Inverse of D

For a diagonal matrix, the inverse is found by taking the reciprocal of each diagonal entry.

Therefore:

$$
D^{-1}=
\begin{pmatrix}
\frac12&0&0\\
0&-\frac13&0\\
0&0&\frac15
\end{pmatrix}
$$

### 3. Verify the Inverse of D

Multiply $D$ by $D^{-1}$:

$$
DD^{-1}
=
\begin{pmatrix}
2&0&0\\
0&-3&0\\
0&0&5
\end{pmatrix}
\begin{pmatrix}
\frac12&0&0\\
0&-\frac13&0\\
0&0&\frac15
\end{pmatrix}
$$

$$
DD^{-1}
=
\begin{pmatrix}
1&0&0\\
0&1&0\\
0&0&1
\end{pmatrix}
=I
$$

The reverse multiplication also gives the identity matrix:

$$
D^{-1}D=I
$$

Therefore, the calculated inverse is correct.

### 4. Check Whether E Is Invertible

The diagonal entries of $E$ are $2$, $0$, and $5$.

Since one diagonal entry is zero, $E$ is not invertible.

Its determinant is:

$$
\det(E)=(2)(0)(5)=0
$$

A matrix with a zero determinant has no inverse.

### 5. Final Comparison

- Matrix $D$ is invertible because all its diagonal entries are non-zero.
- Matrix $E$ is not invertible because one of its diagonal entries is zero.

**Conclusion**

Only matrix $D$ has an inverse. Its inverse is obtained by taking the reciprocal of each diagonal entry. Multiplication confirms that the result is the identity matrix. No Gauss-Jordan elimination is needed.