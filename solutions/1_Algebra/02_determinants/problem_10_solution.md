# Exercise 10 - Detecting Dependence

## Question

Without carrying out a full determinant calculation, explain why

$$
\det\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 5
\end{pmatrix} = 0.
$$

Identify a specific dependence between the rows and connect it with noninvertibility of the matrix.

## Solution

The second row is twice the first row:

$$
R_2 = 2R_1
$$

This means that the rows are linearly dependent.

A matrix with linearly dependent rows has a determinant equal to zero.

Therefore:

$$
\det(A) = 0
$$

Since the determinant is zero, the matrix is not invertible.

This shows that linearly dependent rows make a matrix singular.