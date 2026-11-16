# Exercise 7 – Identity Matrix, Zero Matrix, and Powers

## Question

Given:

$$
A=\begin{pmatrix}2&1\\0&2\end{pmatrix}
$$

Compute \(AI\), \(IA\), \(A+0\), \(A^2\), and \(A^3\). Explain the roles of the matrices I and 0, and describe the pattern you observe in successive powers of A.

## Solution

The identity matrix and zero matrix are:

$$
I=\begin{pmatrix}1&0\\0&1\end{pmatrix},
\quad
0=\begin{pmatrix}0&0\\0&0\end{pmatrix}
$$

$$
AI=IA=A+0=
\begin{pmatrix}2&1\\0&2\end{pmatrix}
$$

Calculate the powers:

$$
A^2=
\begin{pmatrix}2&1\\0&2\end{pmatrix}
\begin{pmatrix}2&1\\0&2\end{pmatrix}
=
\begin{pmatrix}4&4\\0&4\end{pmatrix}
$$

$$
A^3=A^2A=
\begin{pmatrix}4&4\\0&4\end{pmatrix}
\begin{pmatrix}2&1\\0&2\end{pmatrix}
=
\begin{pmatrix}8&12\\0&8\end{pmatrix}
$$

The pattern is:

$$
A=\begin{pmatrix}2^1&1\cdot2^0\\0&2^1\end{pmatrix}
$$

$$
A^2=\begin{pmatrix}2^2&2\cdot2^1\\0&2^2\end{pmatrix}
$$

$$
A^3=\begin{pmatrix}2^3&3\cdot2^2\\0&2^3\end{pmatrix}
$$

Therefore, the general formula is:

$$
\boxed{
A^n=\begin{pmatrix}
2^n&n2^{n-1}\\
0&2^n
\end{pmatrix}
}
$$

The identity matrix leaves A unchanged when multiplied by it. Adding the zero matrix also leaves A unchanged.