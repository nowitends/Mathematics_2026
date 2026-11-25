# Exercise 2. Gaussian Elimination — One Solution

## Given System

We are given the following system of equations:

$$
\begin{cases}
x+y+z=6\\
2x-y+z=3\\
x+2y-z=2
\end{cases}
$$

The task is to solve the system using Gaussian elimination. After finding the solution, I also need to substitute the values into all three original equations to check the result.

## Solution

First, I write the system as an augmented matrix:

$$
\left[
\begin{array}{ccc|c}
1&1&1&6\\
2&-1&1&3\\
1&2&-1&2
\end{array}
\right]
$$

### Step 1: Eliminate x

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
1&1&1&6\\
0&-3&-1&-9\\
0&1&-2&-4
\end{array}
\right]
$$

### Step 2: Continue Gaussian Elimination

To make the next calculation easier, I swap the second and third rows:

$$
R_2\leftrightarrow R_3
$$

Then I add three times the second row to the third row:

$$
R_3\rightarrow R_3+3R_2
$$

The matrix becomes:

$$
\left[
\begin{array}{ccc|c}
1&1&1&6\\
0&1&-2&-4\\
0&0&-7&-21
\end{array}
\right]
$$

Now the matrix is in upper triangular form.

### Step 3: Find the Unknowns

Starting from the last row:

$$
-7z=-21
$$

$$
z=3
$$

Now I use the second row:

$$
y-2z=-4
$$

Substituting $z=3$:

$$
y-2(3)=-4
$$

$$
y=2
$$

Finally, I use the first row:

$$
x+y+z=6
$$

Substituting $y=2$ and $z=3$:

$$
x+2+3=6
$$

$$
x=1
$$

Therefore, the solution is:

$$
\boxed{x=1,\quad y=2,\quad z=3}
$$

### Step 4: Check the Solution

I substitute the values into the original equations to make sure the result is correct.

**First equation:**

$$
x+y+z=6
$$

$$
1+2+3=6
$$

$$
6=6
$$

**Second equation:**

$$
2x-y+z=3
$$

$$
2(1)-2+3=3
$$

$$
3=3
$$

**Third equation:**

$$
x+2y-z=2
$$

$$
1+2(2)-3=2
$$

$$
2=2
$$

All three equations are satisfied.

## Conclusion

The system has exactly one solution:

$$
\boxed{(x,y,z)=(1,2,3)}
$$

After checking the values in all three original equations, I can confirm that the solution is correct.