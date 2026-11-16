# Exercise 14 – A Matrix That Is Its Own Inverse

## Question

Assume that a square matrix A satisfies:

$$
A^2=I
$$

Show that:

$$
A^{-1}=A
$$

Give an example of a 2x2 matrix different from I and -I that satisfies this condition. Verify it by multiplication.

## Solution

### 1. Show That A Is Its Own Inverse

We know that:

$$
A^2=I
$$

This means:

$$
A\cdot A=I
$$

The definition of an inverse matrix is:

$$
A\cdot A^{-1}=I
$$

Comparing these two equations:

$$
A\cdot A= A\cdot A^{-1}
$$

Therefore:

$$
\boxed{A^{-1}=A}
$$

### 2. Give an Example

Choose the following matrix:

$$
A=
\begin{pmatrix}
0 & 1\\
1 & 0
\end{pmatrix}
$$

This matrix is different from I and -I.

### 3. Verify the Result

Multiply A by itself:

$$
A^2=A\cdot A
$$

$$
=
\begin{pmatrix}
0 & 1\\
1 & 0
\end{pmatrix}
\begin{pmatrix}
0 & 1\\
1 & 0
\end{pmatrix}
$$

Multiplying:

$$
=
\begin{pmatrix}
0+1 & 0+0\\
0+0 & 1+0
\end{pmatrix}
$$

Therefore:

$$
\boxed{
A^2=
\begin{pmatrix}
1 & 0\\
0 & 1
\end{pmatrix}
=I
}
$$

### 4. Conclusion

The matrix satisfies the condition A² = I.

Therefore, the matrix is its own inverse.

$$
\boxed{A^{-1}=A}
$$

The result is correct.