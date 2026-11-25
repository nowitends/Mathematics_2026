# Exercise 15. Classifying Three Systems

## Given Systems

We are given three different systems:

**System 1**

$$
\begin{cases}
x+y=2\\
x-y=0
\end{cases}
$$

**System 2**

$$
\begin{cases}
x+y=2\\
2x+2y=4
\end{cases}
$$

**System 3**

$$
\begin{cases}
x+y=2\\
2x+2y=5
\end{cases}
$$

The task is to classify each system as having one solution, infinitely many solutions, or no solution. I will use elimination to check each case.

## Solution

### System 1: One Solution

The system is:

$$
\begin{cases}
x+y=2\\
x-y=0
\end{cases}
$$

I subtract the second equation from the first:

$$
(x+y)-(x-y)=2-0
$$

$$
2y=2
$$

$$
y=1
$$

Now I substitute this value into the first equation:

$$
x+1=2
$$

$$
x=1
$$

The solution is:

$$
\boxed{(x,y)=(1,1)}
$$

This system has exactly one solution because both variables have fixed values.

### System 2: Infinitely Many Solutions

The system is:

$$
\begin{cases}
x+y=2\\
2x+2y=4
\end{cases}
$$

I multiply the first equation by 2:

$$
2x+2y=4
$$

This is exactly the second equation.

If I subtract the first equation multiplied by 2 from the second equation, I get:

$$
0=0
$$

This means both equations describe the same line.

Therefore, there are infinitely many solutions.

I can write them as:

$$
y=2-x
$$

So the solutions are:

$$
\boxed{(x,y)=(t,2-t),\quad t\in\mathbb{R}}
$$

### System 3: No Solution

The system is:

$$
\begin{cases}
x+y=2\\
2x+2y=5
\end{cases}
$$

I multiply the first equation by 2:

$$
2x+2y=4
$$

Now I subtract this equation from the second equation:

$$
(2x+2y)-(2x+2y)=5-4
$$

$$
0=1
$$

This is impossible because zero cannot be equal to one.

Therefore, the system has no solution.

## Conclusion

The three systems represent the three possible cases:

**System 1:**

$$
\boxed{\text{One solution}}
$$

**System 2:**

$$
\boxed{\text{Infinitely many solutions}}
$$

**System 3:**

$$
\boxed{\text{No solution}}
$$

The difference becomes clear after elimination:

- If we get fixed values for the variables, there is one solution.
- If we get $0=0$, there are infinitely many solutions.
- If we get a contradiction such as $0=1$, there is no solution.