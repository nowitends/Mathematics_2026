# Exercise 3 - Swapping Two Rows

## Question

Given:

\[
A=\begin{pmatrix}
1&2&0\\
0&3&1\\
2&1&1
\end{pmatrix}
\]

Calculate det A. Then form matrix B by swapping the first and second rows of A. Predict det B and verify your answer.

## Solution

First, calculate det A:

\[
\det(A)=1(3-1)-2(0-2)=2+4=6
\]

After swapping the first and second rows:

\[
B=\begin{pmatrix}
0&3&1\\
1&2&0\\
2&1&1
\end{pmatrix}
\]

Swapping two rows changes the sign of the determinant.

\[
\det(B)=-\det(A)=-6
\]

Checking by calculation:

\[
\det(B)=-3(1)+1(1-4)
\]

\[
=-3-3=-6
\]

Therefore, det A = 6 and det B = -6.