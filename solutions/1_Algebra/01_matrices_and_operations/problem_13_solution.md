# Exercise 13 – A Recurrence Written in Matrix Form

## Question

Given:

\[
F=\begin{pmatrix}1&1\\1&0\end{pmatrix}
\]

Calculate \(F^2\), \(F^3\), \(F^4\) and \(F^5\). Compare the results with the Fibonacci sequence. Also calculate \(F\begin{pmatrix}a\\b\end{pmatrix}\).

## Solution

Calculate the powers:

\[
F^2=\begin{pmatrix}2&1\\1&1\end{pmatrix}
\]

\[
F^3=\begin{pmatrix}3&2\\2&1\end{pmatrix}
\]

\[
F^4=\begin{pmatrix}5&3\\3&2\end{pmatrix}
\]

\[
F^5=\begin{pmatrix}8&5\\5&3\end{pmatrix}
\]

The numbers follow the Fibonacci sequence:

\[
0,1,1,2,3,5,8,\ldots
\]

Each number is the sum of the two previous numbers. The entries of the matrix powers follow the same pattern.

Now calculate:

\[
F\begin{pmatrix}a\\b\end{pmatrix}
=
\begin{pmatrix}1&1\\1&0\end{pmatrix}
\begin{pmatrix}a\\b\end{pmatrix}
\]

\[
=\begin{pmatrix}a+b\\a\end{pmatrix}
\]

The new first term is \(a+b\), and the second term is a. This performs one Fibonacci recurrence step.