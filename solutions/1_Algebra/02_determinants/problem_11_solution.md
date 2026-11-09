# Exercise 11 - Shortening the Calculation with Row Operations

## Question

Calculate the determinant using row operations.

\[
A=\begin{pmatrix}
1&2&3\\
1&3&4\\
1&4&6
\end{pmatrix}
\]

## Solution

Apply the row operations:

\[
R_2\rightarrow R_2-R_1
\]

\[
R_3\rightarrow R_3-R_1
\]

\[
\begin{pmatrix}
1&2&3\\
0&1&1\\
0&2&3
\end{pmatrix}
\]

Then:

\[
R_3\rightarrow R_3-2R_2
\]

\[
\begin{pmatrix}
1&2&3\\
0&1&1\\
0&0&1
\end{pmatrix}
\]

These row operations do not change the determinant.

\[
\det(A)=1\cdot1\cdot1=1
\]

Therefore, det(A) = 1.

Adding a multiple of one row to another does not change the determinant.