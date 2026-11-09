# Exercise 14 - A System of Equations and the Determinant

## Question

Consider the system Ax = b, where

\[
A=\begin{pmatrix}
1&2\\
k&4
\end{pmatrix}
\]

Find the values of k for which the system has exactly one solution for every b. For the remaining value, give examples of infinitely many solutions and no solution.

## Solution

Calculate the determinant:

\[
\det(A)=4-2k
\]

The system has exactly one solution for every b when the determinant is not zero.

\[
4-2k\neq0
\]

\[
k\neq2
\]

For k = 2, the second row is twice the first row.

For infinitely many solutions, choose:

\[
b=\begin{pmatrix}1\\2\end{pmatrix}
\]

The equations are dependent, so there are infinitely many solutions.

For no solution, choose:

\[
b=\begin{pmatrix}1\\0\end{pmatrix}
\]

The equations are inconsistent.

Therefore, the system has a unique solution for every b when k is not equal to 2.