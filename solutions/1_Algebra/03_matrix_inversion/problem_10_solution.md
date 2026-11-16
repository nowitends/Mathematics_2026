# Exercise 10 – Inverse of a Diagonal Matrix

## Question

Given:

$$
D=\begin{pmatrix}
2&0&0\\
0&-3&0\\
0&0&5
\end{pmatrix}
$$

$$
E=\begin{pmatrix}
2&0&0\\
0&0&0\\
0&0&5
\end{pmatrix}
$$

Decide which matrix is invertible. Find the inverse of the invertible matrix and check the result by multiplication.

## Solution

### 1. Check Matrix D

A diagonal matrix is invertible if all diagonal elements are nonzero.

For matrix D:

$$
D=\begin{pmatrix}
2&0&0\\
0&-3&0\\
0&0&5
\end{pmatrix}
$$

All diagonal elements are nonzero.

Therefore, D is invertible.

### 2. Calculate the Inverse of D

To find the inverse, take the reciprocal of each diagonal element.

$$
D^{-1}=
\begin{pmatrix}
\frac{1}{2}&0&0\\
0&-\frac{1}{3}&0\\
0&0&\frac{1}{5}
\end{pmatrix}
$$

Therefore:

$$
\boxed{
D^{-1}=
\begin{pmatrix}
\frac12&0&0\\
0&-\frac13&0\\
0&0&\frac15
\end{pmatrix}
}
$$

### 3. Check the Result

Multiply D by its inverse:

$$
DD^{-1}=
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
=
\begin{pmatrix}
1&0&0\\
0&1&0\\
0&0&1
\end{pmatrix}
$$

Therefore:

$$
\boxed{DD^{-1}=I}
$$

### 4. Check Matrix E

For matrix E:

$$
E=\begin{pmatrix}
2&0&0\\
0&0&0\\
0&0&5
\end{pmatrix}
$$

One diagonal element is zero.

Its determinant is:

$$
\det(E)=(2)(0)(5)=0
$$

Since the determinant is zero, the inverse does not exist.

Therefore:

$$
\boxed{E^{-1}\text{ does not exist}}
$$

### 5. Conclusion

Matrix D is invertible because all diagonal elements are nonzero.

Matrix E is not invertible because one diagonal element is zero.

The inverse of D is correct because their product gives the identity matrix.