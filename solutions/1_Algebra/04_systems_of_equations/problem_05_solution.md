# Exercise 5. Row Echelon Form and Number of Solutions

## Given Matrix

We are given the following augmented matrix:

$$
\left[
\begin{array}{ccc|c}
1&2&-1&3\\
0&1&2&1\\
0&0&0&0
\end{array}
\right]
$$

The task is to determine the number of solutions, write them in parametric form, and explain how many variables can be chosen freely.

## Solution

First, I write the equations represented by the matrix:

$$
\begin{cases}
x+2y-z=3\\
y+2z=1\\
0=0
\end{cases}
$$

### Step 1: Identify the Pivot Variables

Looking at the matrix, I can see that there are two pivot positions:

- The first pivot is in the $x$ column.
- The second pivot is in the $y$ column.

There is no pivot in the $z$ column, so $z$ is a free variable.

### Step 2: Find the Variables

Since $z$ is free, I choose:

$$
z=t
$$

From the second equation:

$$
y+2z=1
$$

Substituting $z=t$:

$$
y+2t=1
$$

Therefore:

$$
y=1-2t
$$

Now I use the first equation:

$$
x+2y-z=3
$$

Substituting the values of $y$ and $z$:

$$
x+2(1-2t)-t=3
$$

$$
x+2-4t-t=3
$$

$$
x=1+5t
$$

### Step 3: Write the Parametric Solution

The solution is:

$$
\boxed{
\begin{aligned}
x&=1+5t\\
y&=1-2t\\
z&=t
\end{aligned}
\quad t\in\mathbb{R}
}
$$

### Step 4: Determine the Number of Solutions

There are three variables and two pivot columns. This means there is one free variable.

Since $t$ can be any real number, there are infinitely many solutions.

The last row gives $0=0$, so it does not create a contradiction.

## Conclusion

The system has infinitely many solutions because there is one free variable.

The parametric form is:

$$
\boxed{(x,y,z)=(1+5t,1-2t,t)}
$$

There is one free variable, which is $z$.