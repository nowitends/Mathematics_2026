# Exercise 12 – Formula for a Matrix Power

## Question

Given:

\[
A=\begin{pmatrix}1&1\\0&1\end{pmatrix}
\]

Calculate \(A^2\), \(A^3\) and \(A^4\). Find a formula for \(A^n\) and verify it for \(n+1\).

## Solution

First, calculate the powers:

\[
A^2=A\cdot A=
\begin{pmatrix}1&2\\0&1\end{pmatrix}
\]

\[
A^3=A^2\cdot A=
\begin{pmatrix}1&3\\0&1\end{pmatrix}
\]

\[
A^4=A^3\cdot A=
\begin{pmatrix}1&4\\0&1\end{pmatrix}
\]

The pattern is:

\[
A^n=\begin{pmatrix}1&n\\0&1\end{pmatrix}
\]

To verify the formula, assume it is true for n:

\[
A^{n+1}=A^nA
\]

\[
=\begin{pmatrix}1&n\\0&1\end{pmatrix}
\begin{pmatrix}1&1\\0&1\end{pmatrix}
\]

\[
=\begin{pmatrix}1&n+1\\0&1\end{pmatrix}
\]

This is the same formula for \(n+1\). Therefore, the formula is valid for all non-negative integers n.