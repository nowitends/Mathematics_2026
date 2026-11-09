# Exercise 13 - Determinant by Elimination

## Question

Calculate the determinant using elimination.

\[
A=\begin{pmatrix}
1&2&3\\
2&5&7\\
1&0&2
\end{pmatrix}
\]

## Solution

Apply the row operations:

\[
R_2\rightarrow R_2-2R_1
\]

\[
R_3\rightarrow R_3-R_1
\]

\[
\begin{pmatrix}
1&2&3\\
0&1&1\\
0&-2&-1
\end{pmatrix}
\]

Then:

\[
R_3\rightarrow R_3+2R_2
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