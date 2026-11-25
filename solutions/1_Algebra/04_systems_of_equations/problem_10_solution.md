# Exercise 10. A Polynomial Through Three Points

## Given Points

We need to find a polynomial of the form:

$$
p(x)=ax^2+bx+c
$$

Its graph must pass through the following three points:

$$
(0,1),\quad (1,3),\quad (2,9)
$$

The task is to turn this problem into a system of equations, find the unknown coefficients, and check the result using all three points.

## Solution

### Step 1: Use the First Point

The first point is $(0,1)$.

I substitute $x=0$ and $p(x)=1$ into the polynomial:

$$
a(0)^2+b(0)+c=1
$$

Therefore:

$$
c=1
$$

### Step 2: Use the Second Point

The second point is $(1,3)$.

I substitute $x=1$ and $p(x)=3$:

$$
a(1)^2+b(1)+c=3
$$

$$
a+b+c=3
$$

Since $c=1$:

$$
a+b=2
$$

### Step 3: Use the Third Point

The third point is $(2,9)$.

I substitute $x=2$ and $p(x)=9$:

$$
a(2)^2+b(2)+c=9
$$

$$
4a+2b+c=9
$$

Since $c=1$:

$$
4a+2b=8
$$

Dividing both sides by 2:

$$
2a+b=4
$$

### Step 4: Solve the System

Now I have two equations:

$$
\begin{cases}
a+b=2\\
2a+b=4
\end{cases}
$$

I subtract the first equation from the second:

$$
(2a+b)-(a+b)=4-2
$$

$$
a=2
$$

Now I substitute $a=2$ into the first equation:

$$
2+b=2
$$

$$
b=0
$$

I already found that:

$$
c=1
$$

Therefore, the coefficients are:

$$
\boxed{a=2,\quad b=0,\quad c=1}
$$

### Step 5: Write the Polynomial

I put the coefficients into the original polynomial:

$$
p(x)=ax^2+bx+c
$$

The final polynomial is:

$$
\boxed{p(x)=2x^2+1}
$$

### Step 6: Check All Three Points

I substitute each $x$ value into the polynomial.

**First point: $(0,1)$**

$$
p(0)=2(0)^2+1=1
$$

**Second point: $(1,3)$**

$$
p(1)=2(1)^2+1=3
$$

**Third point: $(2,9)$**

$$
p(2)=2(2)^2+1=9
$$

All three points satisfy the polynomial.

## Conclusion

The polynomial that passes through all three given points is:

$$
\boxed{p(x)=2x^2+1}
$$

The result is correct because all three points give the required values when substituted into the polynomial.