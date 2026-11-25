# Exercise 5 – A 3x3 Matrix

## Question

Use Gauss–Jordan elimination to find the inverse of:

$$
A=
\begin{pmatrix}
1&1&0\\
0&1&1\\
1&0&1
\end{pmatrix}
$$

Check the result by multiplication.

## Solution

### 1. Set Up the Augmented Matrix

Start with:

$$
[A|I]=
\left[
\begin{array}{ccc|ccc}
1&1&0&1&0&0\\
0&1&1&0&1&0\\
1&0&1&0&0&1
\end{array}
\right]
$$

### 2. Apply Row Operations

Subtract Row 1 from Row 3:

$$
R_3\rightarrow R_3-R_1
$$

$$
\left[
\begin{array}{ccc|ccc}
1&1&0&1&0&0\\
0&1&1&0&1&0\\
0&-1&1&-1&0&1
\end{array}
\right]
$$

Add Row 2 to Row 3:

$$
R_3\rightarrow R_3+R_2
$$

$$
\left[
\begin{array}{ccc|ccc}
1&1&0&1&0&0\\
0&1&1&0&1&0\\
0&0&2&-1&1&1
\end{array}
\right]
$$

Divide Row 3 by 2:

$$
R_3\rightarrow \frac{1}{2}R_3
$$

$$
\left[
\begin{array}{ccc|ccc}
1&1&0&1&0&0\\
0&1&1&0&1&0\\
0&0&1&-\frac12&\frac12&\frac12
\end{array}
\right]
$$

Subtract Row 3 from Row 2:

$$
R_2\rightarrow R_2-R_3
$$

$$
\left[
\begin{array}{ccc|ccc}
1&1&0&1&0&0\\
0&1&0&\frac12&\frac12&-\frac12\\
0&0&1&-\frac12&\frac12&\frac12
\end{array}
\right]
$$

Subtract Row 2 from Row 1:

$$
R_1\rightarrow R_1-R_2
$$

$$
\left[
\begin{array}{ccc|ccc}
1&0&0&\frac12&-\frac12&\frac12\\
0&1&0&\frac12&\frac12&-\frac12\\
0&0&1&-\frac12&\frac12&\frac12
\end{array}
\right]
$$

### 3. Find the Inverse

The left side is now the identity matrix.

Therefore:

$$
\boxed{
A^{-1}=
\begin{pmatrix}
\frac12&-\frac12&\frac12\\
\frac12&\frac12&-\frac12\\
-\frac12&\frac12&\frac12
\end{pmatrix}
}
$$

### 4. Verify the Result

Multiply A by its inverse:

$$
AA^{-1}=
\begin{pmatrix}
1&1&0\\
0&1&1\\
1&0&1
\end{pmatrix}
\begin{pmatrix}
\frac12&-\frac12&\frac12\\
\frac12&\frac12&-\frac12\\
-\frac12&\frac12&\frac12
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

Thus:

$$
\boxed{AA^{-1}=I}
$$

### 5. Conclusion

The multiplication gives the identity matrix.

Therefore, the inverse is correct.

$$
\boxed{
A^{-1}=
\frac12
\begin{pmatrix}
1&-1&1\\
1&1&-1\\
-1&1&1
\end{pmatrix}
}
$$