# Exercise 13. Does Every Equation Add New Information?

## Given System

We are given the following system:

$$
\begin{cases}
x_1+x_2=10\\
x_2+x_3=8\\
x_1-x_3=2
\end{cases}
$$

The task is to solve the system and check whether all three equations are independently necessary. If one equation follows from the others, I need to show this by calculation.

## Solution

### Step 1: Start with the First Two Equations

First, I write the first two equations:

$$
x_1+x_2=10
$$

$$
x_2+x_3=8
$$

I subtract the second equation from the first:

$$
(x_1+x_2)-(x_2+x_3)=10-8
$$

After simplifying:

$$
x_1-x_3=2
$$

This is exactly the third equation.

Therefore, the third equation follows from the first two equations and does not give any new information.

### Step 2: Find the Variables

Now I use the first two equations to find the solution.

I choose $x_3=t$ as a free variable.

From the second equation:

$$
x_2+x_3=8
$$

Substituting $x_3=t$:

$$
x_2+t=8
$$

Therefore:

$$
x_2=8-t
$$

Now I use the first equation:

$$
x_1+x_2=10
$$

Substituting $x_2=8-t$:

$$
x_1+8-t=10
$$

$$
x_1=2+t
$$

### Step 3: Write the Parametric Solution

The complete solution is:

$$
\boxed{
\begin{aligned}
x_1&=2+t\\
x_2&=8-t\\
x_3&=t
\end{aligned}
\quad t\in\mathbb{R}
}
$$

### Step 4: Check the Third Equation

I substitute the values into the third equation:

$$
x_1-x_3=2
$$

$$
(2+t)-t=2
$$

$$
2=2
$$

The third equation is always satisfied.

This confirms that it follows from the first two equations.

### Step 5: Check One Particular Solution

I choose $t=0$.

Then:

$$
x_1=2,\qquad x_2=8,\qquad x_3=0
$$

Checking the original equations:

**First equation:**

$$
2+8=10
$$

**Second equation:**

$$
8+0=8
$$

**Third equation:**

$$
2-0=2
$$

All three equations are satisfied.

## Conclusion

The system has infinitely many solutions because $x_3$ is a free variable.

The parametric solution is:

$$
\boxed{
(x_1,x_2,x_3)=(2+t,8-t,t),
\quad t\in\mathbb{R}
}
$$

The third equation is not independent because it can be obtained by subtracting the second equation from the first.