# Exercise 8 – Inverse of a Transformation

## Question

The matrix is:

$$
S=
\begin{pmatrix}
2&0\\
0&\frac12
\end{pmatrix}
$$

Find S⁻¹ and explain the inverse transformation. Check the result using a simple vector.

## Solution

### 1. Calculate the Determinant

$$
\det(S)=(2)\left(\frac12\right)-(0)(0)
$$

$$
\boxed{\det(S)=1}
$$

Since the determinant is not zero, the inverse exists.

### 2. Calculate the Inverse

Using the inverse formula:

$$
S^{-1}=
\frac{1}{1}
\begin{pmatrix}
\frac12&0\\
0&2
\end{pmatrix}
$$

Therefore:

$$
\boxed{
S^{-1}=
\begin{pmatrix}
\frac12&0\\
0&2
\end{pmatrix}
}
$$

### 3. Geometric Meaning

The original transformation:

- Doubles the x-coordinate.
- Halves the y-coordinate.

The inverse transformation does the opposite:

- Halves the x-coordinate.
- Doubles the y-coordinate.

It returns the point to its original position.

### 4. Check Using a Vector

Choose:

$$
v=\begin{pmatrix}2\\4\end{pmatrix}
$$

First, apply S:

$$
Sv=
\begin{pmatrix}
2&0\\
0&\frac12
\end{pmatrix}
\begin{pmatrix}2\\4\end{pmatrix}
$$

$$
Sv=
\begin{pmatrix}4\\2\end{pmatrix}
$$

Now apply the inverse:

$$
S^{-1}(Sv)=
\begin{pmatrix}
\frac12&0\\
0&2
\end{pmatrix}
\begin{pmatrix}4\\2\end{pmatrix}
$$

$$
S^{-1}(Sv)=
\begin{pmatrix}2\\4\end{pmatrix}
$$

Therefore:

$$
\boxed{S^{-1}Sv=v}
$$

### 5. Conclusion

The inverse transformation returns the vector to its original position.

Therefore, the inverse is correct.