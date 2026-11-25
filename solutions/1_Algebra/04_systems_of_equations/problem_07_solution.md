# Exercise 7. Choosing a Method Deliberately

## Given Systems

We are asked to choose the most suitable method for three different situations.

### Case 1

A system with a triangular coefficient matrix:

$$
\begin{cases}
2x-y=3\\
4y=8
\end{cases}
$$

### Case 2

Three systems of the form:

$$
Ax=b_i
$$

They have the same invertible matrix $A$, and $A^{-1}$ is already known.

### Case 3

A $3\times3$ system where the inverse matrix is not given, and the goal is to find only one solution vector.

## Solution

### Case 1: Triangular System

For this system, I choose back substitution because the second equation contains only one unknown.

First, I solve the second equation:

$$
4y=8
$$

$$
y=2
$$

Now I substitute this value into the first equation:

$$
2x-y=3
$$

$$
2x-2=3
$$

$$
2x=5
$$

$$
x=\frac{5}{2}
$$

Therefore, the solution is:

$$
\boxed{x=\frac{5}{2},\quad y=2}
$$

Back substitution is a good choice here because the system is already in triangular form. There is no need for extra elimination steps.

### Case 2: Three Systems with the Same Matrix

In this case, I would use the inverse matrix that is already given.

For each system, the solution is:

$$
x_i=A^{-1}b_i
$$

Since the matrix $A$ is the same for all three systems, I only need to calculate or use $A^{-1}$ once.

Then I multiply it by each right-hand side vector:

$$
x_1=A^{-1}b_1
$$

$$
x_2=A^{-1}b_2
$$

$$
x_3=A^{-1}b_3
$$

This saves time because I do not need to find the inverse again for every system.

### Case 3: One 3×3 System

For this case, I would choose Gaussian elimination.

The inverse matrix is not given, and I only need one solution vector. Finding the whole inverse matrix would require extra calculations that are not necessary.

I would write the system as an augmented matrix:

$$
[A\mid b]
$$

Then I would use row operations to get an upper triangular form and find the unknowns using back substitution.

This method is more direct because I only need one solution.

## Conclusion

The best method depends on the structure of the problem:

- For Case 1, back substitution is the easiest method.
- For Case 2, I reuse the known inverse matrix for all three systems.
- For Case 3, Gaussian elimination is more useful than calculating the full inverse.

Each method is chosen to avoid unnecessary calculations.