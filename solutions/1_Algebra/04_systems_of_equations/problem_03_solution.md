# Exercise 3. Inconsistent System

## Given System

We are given the following system:

$$
\begin{cases}
x+2y=3\\
2x+4y=7
\end{cases}
$$

The task is to show that the system is inconsistent. I need to use elimination to find the contradiction in the matrix and explain what it means.

## Solution

First, I write the system as an augmented matrix:

$$
\left[
\begin{array}{cc|c}
1&2&3\\
2&4&7
\end{array}
\right]
$$

### Step 1: Elimination

I want to eliminate $x$ from the second row.

For this, I use the row operation:

$$
R_2\rightarrow R_2-2R_1
$$

After the operation, I get:

$$
\left[
\begin{array}{cc|c}
1&2&3\\
0&0&1
\end{array}
\right]
$$

### Step 2: Find the Contradiction

The second row represents the equation:

$$
0x+0y=1
$$

This means:

$$
0=1
$$

This is impossible because zero cannot be equal to one.

### Step 3: Interpret the Result

I can also see the same problem directly from the original equations.

If I multiply the first equation by 2, I get:

$$
2x+4y=6
$$

But the second equation says:

$$
2x+4y=7
$$

The left sides are the same, but the right sides are different. Therefore, both equations cannot be true at the same time.

## Conclusion

The system is inconsistent because elimination gives the impossible equation $0=1$.

$$
\boxed{\text{No solution}}
$$

Therefore, there is no pair of values for $x$ and $y$ that satisfies both equations.