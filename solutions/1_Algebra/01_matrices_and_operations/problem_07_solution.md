# Exercise 7 – Identity Matrix, Zero Matrix and Powers

## Question

Given:

\[
A=\begin{pmatrix}2&1\\0&2\end{pmatrix}
\]

Calculate \(AI\), \(IA\), \(A+0\), \(A^2\) and \(A^3\). Explain the roles of the identity matrix I and zero matrix 0. Find the pattern in the powers of A.

## Solution

The identity matrix and zero matrix are:

\[
I=\begin{pmatrix}1&0\\0&1\end{pmatrix},
\quad
0=\begin{pmatrix}0&0\\0&0\end{pmatrix}
\]

Multiplying by the identity matrix does not change A:

\[
AI=IA=A=\begin{pmatrix}2&1\\0&2\end{pmatrix}
\]

Adding the zero matrix also does not change A:

\[
A+0=\begin{pmatrix}2&1\\0&2\end{pmatrix}
\]

Now calculate the powers:
\[
A^2=A\cdot A=
\begin{pmatrix}4&4\\0&4\end{pmatrix}
\]

\[
A^3=A^2\cdot A=
\begin{pmatrix}8&12\\0&8\end{pmatrix}
\]
The diagonal elements follow the pattern \(2^n\), and the upper-right element follows \(n\cdot2^{n-1}\).

Therefore, for \(n\geq1\): 
\[
A^n=\begin{pmatrix}
2^n&n\cdot2^{n-1}\\
0&2^n
\end{pmatrix}
\]

The identity matrix keeps a matrix unchanged during multiplication, while the zero matrix does not change it during addition.