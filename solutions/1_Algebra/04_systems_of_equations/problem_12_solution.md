# Exercise 12. Homogeneous System

## Given System

We are given the following homogeneous system:

$$
\begin{cases}
x+2y-z=0\\
2x+4y-2z=0\\
x-y+2z=0
\end{cases}
$$

The task is to find all solutions in parametric form and explain why $(0,0,0)$ always satisfies a homogeneous system.

## Solution

### Step 1: Write the Augmented Matrix

First, I write the system as an augmented matrix:

$$
\left[
\begin{array}{ccc|c}
1&2&-1&0\\
2&4&-2&0\\
1&-1&2&0
\end{array}
\right]
$$

### Step 2: Apply Gaussian Elimination

I use the first row to eliminate $x$ from the second and third rows.

The row operations are:

$$
R_2\rightarrow R_2-2R_1
$$

$$
R_3\rightarrow R_3-R_1
$$

After these operations, I get:

$$
\left[
\begin{array}{ccc|c}
1&2&-1&0\\
0&0&0&0\\
0&-3&3&0
\end{array}
\right]
$$

Now I swap the second and third rows:

$$
R_2\leftrightarrow R_3
$$

The matrix becomes:

$$
\left[
\begin{array}{ccc|c}
1&2&-1&0\\
0&-3&3&0\\
0&0&0&0
\end{array}
\right]
$$

### Step 3: Find the Variables

From the second row:

$$
-3y+3z=0
$$

Dividing by 3:

$$
y=z
$$

I choose $z=t$ as a free variable. Therefore:

$$
y=t
$$

Now I use the first row:

$$
x+2y-z=0
$$

Substituting $y=t$ and $z=t$:

$$
x+2t-t=0
$$

$$
x=-t
$$

### Step 4: Write the Parametric Solution

The complete solution is:

$$
\boxed{
\begin{aligned}
x&=-t\\
y&=t\\
z&=t
\end{aligned}
\quad t\in\mathbb{R}
}
$$

Or, in vector form:

$$
\boxed{
(x,y,z)=t(-1,1,1)
}
$$

### Step 5: Check the Zero Solution

If I choose $t=0$, I get:

$$
x=0,\qquad y=0,\qquad z=0
$$

Substituting these values into the original equations:

$$
0+2(0)-0=0
$$

$$
2(0)+4(0)-2(0)=0
$$

$$
0-0+2(0)=0
$$

All three equations are satisfied.

A homogeneous system always has the zero solution because all variables can be zero and the right-hand side is also zero.

## Conclusion

The system has infinitely many solutions because there is one free variable.

The parametric solution is:

$$
\boxed{(x,y,z)=(-t,t,t),\quad t\in\mathbb{R}}
$$

The zero solution $(0,0,0)$ is included when $t=0$.