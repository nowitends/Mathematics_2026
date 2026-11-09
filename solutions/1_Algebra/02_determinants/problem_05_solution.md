# Exercise 5 - Row Operations

## Question

Given:

\[
A=\begin{pmatrix}
1&2&3\\
2&1&0\\
-1&4&2
\end{pmatrix}
\]

Find det A by simplifying the matrix with row operations. Indicate how the determinant changes at each step.

## Solution

Start with:

\[
A=\begin{pmatrix}
1&2&3\\
2&1&0\\
-1&4&2
\end{pmatrix}
\]

Apply the row operations:

\[
R_2\rightarrow R_2-2R_1
\] 

\[
R_3\rightarrow R_3+R_1
\]

These operations do not change the determinant.

\[
\begin{pmatrix}
1&2&3\\
0&-3&-6\\
0&6&5
\end{pmatrix}
\]

Next:

\[
R_3\rightarrow R_3+2R_2
\]

The determinant remains unchanged.

\[
\begin{pmatrix}
1&2&3\\
0&-3&-6\\
0&0&-7
\end{pmatrix}
\]

Now multiply the diagonal entries:

\[
\det(A)=1\cdot(-3)\cdot(-7)=21
\]

Therefore, det A = 21.