# Exercise 4 – Gauss–Jordan

## Question

Find $A^{-1}$ using the Gauss–Jordan method for:

$$
A=\begin{pmatrix}
1&2\\
3&5
\end{pmatrix}
$$

Show the augmented matrix after each operation and explain why obtaining $I$ on the left gives the inverse on the right.

## Solution

### 1. Set Up the Augmented Matrix

Start with:

$$
[A|I]=
\left[
\begin{array}{cc|cc}
1&2&1&0\\
3&5&0&1
\end{array}
\right]
$$

### 2. Apply Row Operations

Subtract 3 times Row 1 from Row 2:

$$
R_2\rightarrow R_2-3R_1
$$

$$
\left[
\begin{array}{cc|cc}
1&2&1&0\\
0&-1&-3&1
\end{array}
\right]
$$

Multiply Row 2 by -1:

$$
R_2\rightarrow -R_2
$$

$$
\left[
\begin{array}{cc|cc}
1&2&1&0\\
0&1&3&-1
\end{array}
\right]
$$

Subtract 2 times Row 2 from Row 1:

$$
R_1\rightarrow R_1-2R_2
$$

$$
\left[
\begin{array}{cc|cc}
1&0&-5&2\\
0&1&3&-1
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
-5&2\\
3&-1
\end{pmatrix}
}
$$

### 4. Explanation

The same row operations are applied to both sides of the augmented matrix.

When the left side becomes the identity matrix, the right side becomes the inverse of A.

### 5. Conclusion

$$
\boxed{AA^{-1}=I}
$$

Therefore, the inverse matrix is:

$$
\boxed{
A^{-1}=
\begin{pmatrix}
-5&2\\
3&-1
\end{pmatrix}
}
$$