# Exercise 10 - Detecting Dependence

## Question

Explain why the determinant of the following matrix is zero without a full calculation. Identify the dependence between the rows.

\[
A=\begin{pmatrix}
1&2&3\\
2&4&6\\
0&1&5
\end{pmatrix}
\]

## Solution

The second row is twice the first row:

\[
R_2=2R_1
\]

Therefore, the rows are linearly dependent.

A matrix with linearly dependent rows has a determinant equal to zero.

\[
\det(A)=0
\]

The matrix is not invertible because its determinant is zero.