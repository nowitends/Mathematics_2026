# Exercise 11. A Parameter in a System of Three Equations

## Given System

We are given the following system:

$$
\begin{cases}
x+y+z=1\\
x+ty+z=2\\
x+y+tz=3
\end{cases}
$$

The task is to analyze the number of solutions depending on the parameter $t$. I will use elimination and check the value for which a calculation step is not valid.

## Solution

### Step 1: Write the Augmented Matrix

First, I write the system as an augmented matrix:

$$
\left[
\begin{array}{ccc|c}
1&1&1&1\\
1&t&1&2\\
1&1&t&3
\end{array}
\right]
$$

### Step 2: Apply Elimination

I use the first row to eliminate $x$ from the second and third rows.

The row operations are:

$$
R_2\rightarrow R_2-R_1
$$

$$
R_3\rightarrow R_3-R_1
$$

After these operations, I get:

$$
\left[
\begin{array}{ccc|c}
1&1&1&1\\
0&t-1&0&1\\
0&0&t-1&2
\end{array}
\right]
$$

Now the last two rows give:

$$
(t-1)y=1
$$

$$
(t-1)z=2
$$

### Step 3: Analyze the Case $t\neq1$

If $t$ is not equal to 1, I can divide both equations by $t-1$.

From the second row:

$$
y=\frac{1}{t-1}
$$

From the third row:

$$
z=\frac{2}{t-1}
$$

Now I use the first equation:

$$
x+y+z=1
$$

Substituting the values of $y$ and $z$:

$$
x+\frac{1}{t-1}+\frac{2}{t-1}=1
$$

$$
x+\frac{3}{t-1}=1
$$

Therefore:

$$
x=1-\frac{3}{t-1}
$$

So:

$$
x=\frac{t-4}{t-1}
$$

The solution is:

$$
\boxed{
\begin{aligned}
x&=\frac{t-4}{t-1}\\
y&=\frac{1}{t-1}\\
z&=\frac{2}{t-1}
\end{aligned}
}
$$

For every $t\neq1$, the system has exactly one solution.

### Step 4: Analyze the Case $t=1$

Now I check what happens when $t=1$.

The system becomes:

$$
\begin{cases}
x+y+z=1\\
x+y+z=2\\
x+y+z=3
\end{cases}
$$

All three equations have the same left-hand side, but their right-hand sides are different.

Using the matrix obtained after elimination, I get:

$$
\left[
\begin{array}{ccc|c}
1&1&1&1\\
0&0&0&1\\
0&0&0&2
\end{array}
\right]
$$

The second row gives:

$$
0=1
$$

This is impossible.

Therefore, the system has no solution when $t=1$.

### Step 5: Determine the Number of Solutions

There are two possible cases:

- If $t\neq1$, the system has exactly one solution.
- If $t=1$, the system has no solution.

There is no value of $t$ that gives infinitely many solutions.

## Conclusion

The number of solutions depends on the value of $t$:

$$
\boxed{
\begin{cases}
\text{Exactly one solution},&t\neq1\\
\text{No solution},&t=1
\end{cases}
}
$$

The important point is that when $t=1$, I cannot divide by $t-1$. This value must be checked separately because the elimination process gives a contradiction.