# Exercise 10 – Columns of a Matrix Product

## Question

Given:

\[
A=\begin{pmatrix}1&2&0\\0&1&1\end{pmatrix},
\quad
B=\begin{pmatrix}1&2\\-1&0\\3&1\end{pmatrix}
\]

Let \(b_1\) and \(b_2\) be the columns of B.

1. Calculate \(Ab_1\) and \(Ab_2\).
2. Calculate \(AB\).
3. Compare the results.

## Solution

The columns of B are:

\[
b_1=\begin{pmatrix}1\\-1\\3\end{pmatrix},
\quad
b_2=\begin{pmatrix}2\\0\\1\end{pmatrix}
\]

**1. Calculate \(Ab_1\) and \(Ab_2\):**

\[
Ab_1=
\begin{pmatrix}1&2&0\\0&1&1\end{pmatrix}
\begin{pmatrix}1\\-1\\3\end{pmatrix}
=\begin{pmatrix}-1\\2\end{pmatrix}
\]

\[
Ab_2=
\begin{pmatrix}1&2&0\\0&1&1\end{pmatrix}
\begin{pmatrix}2\\0\\1\end{pmatrix}
=\begin{pmatrix}2\\1\end{pmatrix}
\]

**2. Calculate AB:**

\[
AB=\begin{pmatrix}-1&2\\2&1\end{pmatrix}
\]

**3. Comparison:**

The columns of AB are exactly \(Ab_1\) and \(Ab_2\):

\[
AB=\begin{pmatrix}|&|\\Ab_1&Ab_2\\|&|\end{pmatrix}
\]

This shows that each column of a matrix product is obtained by multiplying A by the corresponding column of B.