# Exercise 11 – When Do Matrices Commute?

## Question

Given:

\[
A=\begin{pmatrix}1&1\\0&1\end{pmatrix},
\quad
B=\begin{pmatrix}a&b\\c&d\end{pmatrix}
\]

Find the conditions on a, b, c and d for which \(AB=BA\). Describe the general form of B.

## Solution

First, calculate AB:

\[
AB=\begin{pmatrix}a+c&b+d\\c&d\end{pmatrix}
\]

Now calculate BA:

\[
BA=\begin{pmatrix}a&a+b\\c&c+d\end{pmatrix}
\]

For \(AB=BA\), corresponding entries must be equal:

\[
a+c=a \Rightarrow c=0
\]

\[
b+d=a+b \Rightarrow d=a
\]

The remaining equations give the same condition.

Therefore:

\[
c=0,\quad d=a
\]

The general form of B is:

\[
B=\begin{pmatrix}a&b\\0&a\end{pmatrix}
\]

where a and b can be any real numbers.

Thus, \(AB=BA\) when B has this form.