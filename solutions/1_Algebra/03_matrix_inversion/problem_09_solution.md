# Exercise 9 – Matrix Equation

## Question

Given:

$$
A=\begin{pmatrix}1&2\\0&1\end{pmatrix}
$$

$$
B=\begin{pmatrix}3&1\\2&4\end{pmatrix}
$$

Solve the equation AX = B for X.

## Solution

### 1. Determine Which Side to Use

The original equation is:

$$
AX=B
$$

Multiply both sides by A⁻¹ on the left:

$$
A^{-1}AX=A^{-1}B
$$

Since:

$$
A^{-1}A=I
$$

Therefore:

$$
\boxed{X=A^{-1}B}
$$

### 2. Calculate the Determinant

$$
\det(A)=(1)(1)-(2)(0)
$$

$$
\boxed{\det(A)=1}
$$

Since the determinant is not zero, the inverse exists.

### 3. Calculate the Inverse of A

Using the inverse formula:

$$
A^{-1}=
\begin{pmatrix}
1&-2\\
0&1
\end{pmatrix}
$$

### 4. Calculate X

Using:

$$
X=A^{-1}B
$$

Substitute the values:

$$
X=
\begin{pmatrix}
1&-2\\
0&1
\end{pmatrix}
\begin{pmatrix}
3&1\\
2&4
\end{pmatrix}
$$

$$
X=
\begin{pmatrix}
3-4&1-8\\
2&4
\end{pmatrix}
$$

$$
\boxed{
X=
\begin{pmatrix}
-1&-7\\
2&4
\end{pmatrix}
}
$$

### 5. Verify the Result

Substitute X into the original equation:

$$
AX=
\begin{pmatrix}
1&2\\
0&1
\end{pmatrix}
\begin{pmatrix}
-1&-7\\
2&4
\end{pmatrix}
$$

$$
AX=
\begin{pmatrix}
-1+4&-7+8\\
2&4
\end{pmatrix}
$$

$$
AX=
\begin{pmatrix}
3&1\\
2&4
\end{pmatrix}
$$

This is equal to B.

Therefore:

$$
\boxed{AX=B}
$$

### 6. Conclusion

The solution is:

$$
\boxed{
X=
\begin{pmatrix}
-1&-7\\
2&4
\end{pmatrix}
}
$$

The result is correct because multiplying A by X gives B.