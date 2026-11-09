# Exercise 12 - A Parameter Revealed by a Row Operation

## Question

Given:

\[
A(t)=\begin{pmatrix}
1&2&3\\
2&4&t\\
0&1&1
\end{pmatrix}
\]

Find the value of t for which the matrix is not invertible.

## Solution

Apply the given row operation:

\[
R_2\rightarrow R_2-2R_1
\]

\[
\begin{pmatrix}
1&2&3\\
0&0&t-6\\
0&1&1
\end{pmatrix}
\]

The matrix is not invertible when its determinant is zero.

Expanding along the second row:

\[
\det(A(t))=t-6
\]

\[
t-6=0
\]

\[
t=6
\]

At t = 6, the second row of the original matrix is twice the first row. Therefore, the rows are linearly dependent and the determinant is zero.