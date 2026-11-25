# Exercise 6. A System with a Parameter — Which Cases Actually Occur?

## Given System

We are given the system:

$$
\begin{cases}
x+y=2\\
ax+ay=4
\end{cases}
$$

The task is to analyze the system depending on the parameter $a$.

I need to determine when the system has exactly one solution, infinitely many solutions, or no solution. I also need to explain if one of these cases cannot occur.

## Solution

First, I notice that the second equation can be written as:

$$
a(x+y)=4
$$

From the first equation, we know that:

$$
x+y=2
$$

I substitute this into the second equation:

$$
a\cdot 2=4
$$

Therefore:

$$
2a=4
$$

$$
a=2
$$

### Case 1: When a = 2

If $a=2$, the system becomes:

$$
\begin{cases}
x+y=2\\
2x+2y=4
\end{cases}
$$

The second equation is just two times the first equation.

Both equations represent the same line, so there are infinitely many solutions.

I can write the solution as:

$$
y=2-x
$$

If I choose $x=t$, then:

$$
\boxed{(x,y)=(t,2-t),\quad t\in\mathbb{R}}
$$

### Case 2: When a ≠ 2

If $a$ is not equal to 2, the two equations contradict each other.

From the first equation:

$$
x+y=2
$$

Multiplying both sides by $a$ gives:

$$
ax+ay=2a
$$

But the second equation says:

$$
ax+ay=4
$$

For both equations to be true, we would need:

$$
2a=4
$$

which means $a=2$.

Since we are considering $a\neq 2$, this is impossible.

Therefore, the system has no solution.

### Step 3: Can the System Have Exactly One Solution?

The two equations have proportional coefficients:

$$
\begin{pmatrix}
1&1\\
a&a
\end{pmatrix}
$$

The determinant is:

$$
\det(A)=1\cdot a-1\cdot a=0
$$

The determinant is always zero, so the coefficient matrix is never invertible.

This means the system cannot have exactly one solution.

## Conclusion

The possible cases are:

- If $a=2$, the system has infinitely many solutions.
- If $a\neq 2$, the system has no solution.
- Exactly one solution is not possible for any value of $a$.

Therefore, the system has only two possible cases: infinitely many solutions or no solution.