# Exercise 14. A Small Change in the Right-Hand Side

## Given Systems

We need to compare the following two systems.

**First system:**

$$
\begin{cases}
x+y=2\\
2x-y=1\\
3x=3
\end{cases}
$$

**Second system:**

$$
\begin{cases}
x+y=2\\
2x-y=1\\
3x=3.1
\end{cases}
$$

The task is to check if each system is consistent and explain how a small change in one number can change the type of the system.

## Solution

### Step 1: Solve the First System

I start with the third equation:

$$
3x=3
$$

Dividing both sides by 3:

$$
x=1
$$

Now I substitute this value into the first equation:

$$
x+y=2
$$

$$
1+y=2
$$

$$
y=1
$$

I check these values in the second equation:

$$
2x-y=1
$$

$$
2(1)-1=1
$$

$$
1=1
$$

All three equations are satisfied.

Therefore, the first system is consistent and has exactly one solution:

$$
\boxed{(x,y)=(1,1)}
$$

### Step 2: Solve the Second System

Now I use the third equation of the second system:

$$
3x=3.1
$$

Dividing both sides by 3:

$$
x=\frac{3.1}{3}=\frac{31}{30}
$$

I substitute this value into the first equation:

$$
x+y=2
$$

$$
\frac{31}{30}+y=2
$$

$$
y=2-\frac{31}{30}
$$

$$
y=\frac{29}{30}
$$

Now I check the second equation:

$$
2x-y=1
$$

Substituting the values:

$$
2\left(\frac{31}{30}\right)-\frac{29}{30}=1
$$

$$
\frac{62-29}{30}=1
$$

$$
\frac{33}{30}=1
$$

But:

$$
1.1\neq1
$$

This is a contradiction, so the second system has no solution.

### Step 3: Compare the Results

The first system has one solution because all three equations are satisfied by the same values.

The second system has no solution because the values found from the first and third equations do not satisfy the second equation.

## Conclusion

The results are:

- First system: consistent, with exactly one solution.
- Second system: inconsistent, with no solution.

A small change from 3 to 3.1 in the last equation changes the system from consistent to inconsistent. This shows that even a small change in the right-hand side can affect the existence of a solution.