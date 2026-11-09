# Exercise 7 - Using Properties Instead of Recomputing

## Question

Suppose that for a 3x3 matrix:

\[
\det(A)=-4
\]

Compute:

\[
\det(2A),\quad \det(A^T),\quad
\det(A^2),\quad \det(-A)
\]

Justify each answer using the appropriate property.

## Solution

Since A is a 3x3 matrix:

1. Using \(\det(kA)=k^3\det(A)\):

\[
\det(2A)=2^3(-4)=-32
\]

2. The determinant of a transpose is unchanged:

\[
\det(A^T)=\det(A)=-4
\]

3. Using \(\det(A^2)=\det(A)\det(A)\):

\[
\det(A^2)=(-4)^2=16
\]

4. Using \(\det(-A)=(-1)^3\det(A)\):

\[
\det(-A)=-1(-4)=4
\]

Therefore:

\[
\boxed{-32,\ -4,\ 16,\ 4}
\]