# Exercise 15 – Two Methods for Solving the Same System

## Question

Given:

$$
A=\begin{pmatrix}
2&1\\
1&3
\end{pmatrix}
$$

$$
b=\begin{pmatrix}
7\\
8
\end{pmatrix}
$$

Solve the system $Ax=b$ in two ways:

1. Using the inverse matrix.
2. Using Gaussian elimination.

Compare both solutions.

## Solution

### 1. Calculate the Determinant

For a 2x2 matrix:

$$
\det(A)=ad-bc
$$

Substituting the values:

$$
\det(A)=(2)(3)-(1)(1)
$$

$$
=6-1=5
$$

Therefore:

$$
\boxed{\det(A)=5}
$$

Since the determinant is not zero, the inverse exists.

### 2. Solve Using the Inverse Matrix

The inverse formula is:

$$
A^{-1}=\frac{1}{ad-bc}
\begin{pmatrix}
d&-b\\
-c&a
\end{pmatrix}
$$

Substituting the values:

$$
A^{-1}=\frac{1}{5}
\begin{pmatrix}
3&-1\\
-1&2
\end{pmatrix}
$$

Using:

$$
x=A^{-1}b
$$

Substituting:

$$
x=\frac{1}{5}
\begin{pmatrix}
3&-1\\
-1&2
\end{pmatrix}
\begin{pmatrix}
7\\
8
\end{pmatrix}
$$

Multiplying:

$$
x=\frac{1}{5}
\begin{pmatrix}
21-8\\
-7+16
\end{pmatrix}
$$

$$
x=\frac{1}{5}
\begin{pmatrix}
13\\
9
\end{pmatrix}
$$

Therefore:

$$
\boxed{
x=
\begin{pmatrix}
13/5\\
9/5
\end{pmatrix}
}
$$

### 3. Solve Using Gaussian Elimination

Start with the augmented matrix:

$$
\left[
\begin{array}{cc|c}
2&1&7\\
1&3&8
\end{array}
\right]
$$

Swap Row 1 and Row 2:

$$
R_1\leftrightarrow R_2
$$

$$
\left[
\begin{array}{cc|c}
1&3&8\\
2&1&7
\end{array}
\right]
$$

Subtract 2 times Row 1 from Row 2:

$$
R_2\rightarrow R_2-2R_1
$$

$$
\left[
\begin{array}{cc|c}
1&3&8\\
0&-5&-9
\end{array}
\right]
$$

Divide Row 2 by -5:

$$
R_2\rightarrow-\frac{1}{5}R_2
$$

$$
\left[
\begin{array}{cc|c}
1&3&8\\
0&1&9/5
\end{array}
\right]
$$

Subtract 3 times Row 2 from Row 1:

$$
R_1\rightarrow R_1-3R_2
$$

$$
\left[
\begin{array}{cc|c}
1&0&13/5\\
0&1&9/5
\end{array}
\right]
$$

Therefore:

$$
\boxed{
x=
\begin{pmatrix}
13/5\\
9/5
\end{pmatrix}
}
$$

### 4. Verify the Result

Substitute the solution into the original equation:

$$
Ax=b
$$

$$
\begin{pmatrix}
2&1\\
1&3
\end{pmatrix}
\begin{pmatrix}
13/5\\
9/5
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
26/5+9/5\\
13/5+27/5
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
35/5\\
40/5
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
7\\
8
\end{pmatrix}
=b
$$

Thus:

$$
\boxed{Ax=b}
$$

The solution is correct.

### 5. Compare the Methods

Both methods give the same solution.

- The inverse matrix method requires calculating the determinant and the inverse.
- Gaussian elimination uses row operations directly.

In this example, Gaussian elimination is simpler because it does not require calculating the inverse separately.

### 6. Conclusion

Both methods give the same result:

$$
\boxed{
x=
\begin{pmatrix}
13/5\\
9/5
\end{pmatrix}
}
$$

Therefore, both methods are correct.