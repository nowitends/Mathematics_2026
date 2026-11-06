# Exercise 8 – Row Operations and Their Reversibility

## Question

Given:

\[
A=\begin{pmatrix}
1&2&-1\\
2&4&1\\
-1&1&3
\end{pmatrix}
\]

Perform the following operations in order:
1. \(R_2\leftarrow R_2-2R_1\)
2. \(R_3\leftarrow R_3+R_1\)
3. Interchange \(R_2\) and \(R_3\).

Write the matrix after each step and give the inverse operation for each step.

## Solution

**Step 1:**

\[
R_2\leftarrow R_2-2R_1
\]

\[
\begin{pmatrix}
1&2&-1\\
0&0&3\\
-1&1&3
\end{pmatrix}
\]

Inverse: \(R_2\leftarrow R_2+2R_1\).

**Step 2:**

\[
R_3\leftarrow R_3+R_1
\]

\[
\begin{pmatrix}
1&2&-1\\
0&0&3\\
0&3&2
\end{pmatrix}
\]

Inverse: \(R_3\leftarrow R_3-R_1\).

**Step 3:**

Interchange \(R_2\) and \(R_3\).

\[
\begin{pmatrix}
1&2&-1\\
0&3&2\\
0&0&3
\end{pmatrix}
\]

Inverse: Interchange \(R_2\) and \(R_3\) again.

All three row operations are reversible because each has an inverse operation.