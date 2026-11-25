# Exercise 4. Infinitely Many Solutions

## Given System

We are given the following system:

$$
\begin{cases}
x+y+z=2\\
2x+2y+2z=4\\
x-y+z=0
\end{cases}
$$

The task is to solve the system in parametric form, identify a free variable, and check one chosen parameter value in the original equations.

## Solution

First, I write the system as an augmented matrix:

$$
\left[
\begin{array}{ccc|c}
1&1&1&2\\
2&2&2&4\\
1&-1&1&0
\end{array}
\right]
$$

### Step 1: Apply Gaussian Elimination

I use the first row to eliminate $x$ from the second and third rows.

The row operations are:

$$
R_2\rightarrow R_2-2R_1
$$

$$
R_3\rightarrow R_3-R_1
$$

After these operations, the matrix becomes:

$$
\left[
\begin{array}{ccc|c}
1&1&1&2\\
0&0&0&0\\
0&-2&0&-2
\end{array}
\right]
$$

Now I swap the second and third rows:

$$
R_2\leftrightarrow R_3
$$

The matrix is now:

$$
\left[
\begin{array}{ccc|c}
1&1&1&2\\
0&-2&0&-2\\
0&0&0&0
\end{array}
\right]
$$

### Step 2: Find the Unknowns

From the second row:

$$
-2y=-2
$$

Therefore:

$$
y=1
$$

From the first row:

$$
x+y+z=2
$$

Substituting $y=1$:

$$
x+1+z=2
$$

So:

$$
x+z=1
$$

There is no equation that determines $z$ separately. Therefore, $z$ is a free variable.

### Step 3: Write the Parametric Solution

I choose:

$$
z=t
$$

Then:

$$
x=1-t
$$

And:

$$
y=1
$$

The solution in parametric form is:

$$
\boxed{
\begin{aligned}
x&=1-t\\
y&=1\\
z&=t
\end{aligned}
\qquad t\in\mathbb{R}
}
$$

Since $t$ can be any real number, the system has infinitely many solutions.

### Step 4: Check One Parameter Value

I choose $t=0$.

Then the solution becomes:

$$
x=1,\qquad y=1,\qquad z=0
$$

Now I substitute these values into the original equations.

**First equation:**

$$
x+y+z=2
$$

$$
1+1+0=2
$$

**Second equation:**

$$
2x+2y+2z=4
$$

$$
2(1)+2(1)+2(0)=4
$$

$$
4=4
$$

**Third equation:**

$$
x-y+z=0
$$

$$
1-1+0=0
$$

All three equations are satisfied.

## Conclusion

The system has infinitely many solutions because $z$ is a free variable.

The complete parametric solution is:

$$
\boxed{(x,y,z)=(1-t,1,t),\quad t\in\mathbb{R}}
$$

The chosen value $t=0$ also satisfies all three original equations.