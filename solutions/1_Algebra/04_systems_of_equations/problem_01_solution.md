# Exercise 1. From a System to a Matrix

## Given System

We are given the following system of equations:

$$
\begin{cases}
2x-y+z=4\\
x+3y-2z=1\\
3x+y+z=7
\end{cases}
$$

The task is to write the system in the form $Ax=b$, identify the coefficient matrix, the vector of unknowns, and the right-hand side vector. I also need to explain how each row corresponds to one equation.

## Solution

First, I write the coefficients of each equation in the order $x$, $y$, and $z$.

### Coefficient Matrix

The coefficients from the three equations give the following matrix:

$$
A=
\begin{pmatrix}
2&-1&1\\
1&3&-2\\
3&1&1
\end{pmatrix}
$$

### Vector of Unknowns

The unknown variables are written as a column vector:

$$
x=
\begin{pmatrix}
x\\
y\\
z
\end{pmatrix}
$$

### Right-Hand Side Vector

The numbers on the right side of the equations form this vector:

$$
b=
\begin{pmatrix}
4\\
1\\
7
\end{pmatrix}
$$

### Matrix Form

Now I put everything together:

$$
\begin{pmatrix}
2&-1&1\\
1&3&-2\\
3&1&1
\end{pmatrix}
\begin{pmatrix}
x\\
y\\
z
\end{pmatrix}
=
\begin{pmatrix}
4\\
1\\
7
\end{pmatrix}
$$

### Explanation

Each row of the coefficient matrix represents one equation:

- The first row represents $2x-y+z=4$.
- The second row represents $x+3y-2z=1$.
- The third row represents $3x+y+z=7$.

The coefficients show how the variables are used in each equation, while the right-hand side vector contains the corresponding constants.

## Conclusion

The system is now written in the form $Ax=b$, where $A$ is the coefficient matrix, $x$ is the vector of unknowns, and $b$ is the right-hand side vector.