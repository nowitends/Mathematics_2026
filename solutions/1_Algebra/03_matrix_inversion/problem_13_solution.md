# Exercise 13 – Undoing a Composite Transformation

## Question

The matrices are:

$$
S=
\begin{pmatrix}
2 & 0\\
0 & 1
\end{pmatrix}
$$

$$
H=
\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
$$

Given:

$$
T=HS
$$

Find the inverse of T in two ways and compare the results.

## Solution

### 1. Calculate T

Using:

$$
T=HS
$$

Substituting the matrices:

$$
T=
\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0\\
0 & 1
\end{pmatrix}
$$

Multiplying:

$$
T=
\begin{pmatrix}
2 & 1\\
0 & 1
\end{pmatrix}
$$

### 2. Calculate the Inverse of T

For a 2x2 matrix:

$$
A^{-1}=
\frac{1}{ad-bc}
\begin{pmatrix}
d & -b\\
-c & a
\end{pmatrix}
$$

The determinant of T is:

$$
\det(T)=(2)(1)-(1)(0)=2
$$

Since the determinant is not zero, the inverse exists.

Substituting:

$$
T^{-1}=
\frac{1}{2}
\begin{pmatrix}
1 & -1\\
0 & 2
\end{pmatrix}
$$

Therefore:

$$
\boxed{
T^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2}\\
0 & 1
\end{pmatrix}
}
$$

### 3. Calculate the Inverse Using the Product Rule

The inverse of a product is:

$$
(HS)^{-1}=S^{-1}H^{-1}
$$

First, calculate the inverses:

$$
S^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0\\
0 & 1
\end{pmatrix}
$$

$$
H^{-1}=
\begin{pmatrix}
1 & -1\\
0 & 1
\end{pmatrix}
$$

Now multiply:

$$
T^{-1}=S^{-1}H^{-1}
$$

$$
=
\begin{pmatrix}
\frac{1}{2} & 0\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & -1\\
0 & 1
\end{pmatrix}
$$

Therefore:

$$
\boxed{
T^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2}\\
0 & 1
\end{pmatrix}
}
$$

Both methods give the same result.

### 4. Check the Incorrect Order

Now calculate:

$$
H^{-1}S^{-1}
$$

$$
=
\begin{pmatrix}
1 & -1\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & 0\\
0 & 1
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
\frac{1}{2} & -1\\
0 & 1
\end{pmatrix}
$$

This is different from the correct inverse.

Therefore:

$$
H^{-1}S^{-1}\neq T^{-1}
$$

### 5. Verify the Result

Multiply T by its inverse:

$$
TT^{-1}=
\begin{pmatrix}
2 & 1\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2}\\
0 & 1
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
1 & -1+1\\
0 & 1
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
1 & 0\\
0 & 1
\end{pmatrix}
$$

Thus:

$$
\boxed{TT^{-1}=I}
$$

### 6. Conclusion

Both correct methods give the same inverse.

When undoing a product of matrices, we must reverse the order.

The correct rule is:

$$
\boxed{(HS)^{-1}=S^{-1}H^{-1}}
$$

Therefore, the inverse of a product reverses the order of the operations.