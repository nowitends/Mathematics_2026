# Exercise 15 – Two Methods for Solving the Same System

## Question

For

$$
A=
\begin{pmatrix}
2&1\\
1&3
\end{pmatrix},
\qquad
b=
\begin{pmatrix}
7\\
8
\end{pmatrix}
$$

solve $Ax=b$ in two ways:

1. Using $A^{-1}b$.
2. Using Gaussian elimination.

Compare both solutions, the number of essential steps, and state which method was simpler in this example.

## Solution

### 1. Method 1: Using the Inverse Matrix

We start with:

$$
Ax=b
$$

Multiplying both sides by $A^{-1}$ gives:

$$
x=A^{-1}b
$$

First, calculate the determinant of A:

$$
\det(A)=(2)(3)-(1)(1)=5
$$

Since the determinant is not zero, the inverse exists.

Calculate the inverse:

$$
A^{-1}
=
\frac{1}{5}
\begin{pmatrix}
3&-1\\
-1&2
\end{pmatrix}
$$

Now calculate $x=A^{-1}b$:

$$
x=
\frac{1}{5}
\begin{pmatrix}
3&-1\\
-1&2
\end{pmatrix}
\begin{pmatrix}
7\\
8
\end{pmatrix}
$$

$$
x=
\frac{1}{5}
\begin{pmatrix}
21-8\\
-7+16
\end{pmatrix}
$$

Therefore:

$$
\boxed{
x=
\begin{pmatrix}
\frac{13}{5}\\
\frac{9}{5}
\end{pmatrix}
}
$$

### 2. Method 2: Using Gaussian Elimination

Start with the augmented matrix:

$$
\left[
\begin{array}{cc|c}
2&1&7\\
1&3&8
\end{array}
\right]
$$

First, swap the two rows:

$$
\left[
\begin{array}{cc|c}
1&3&8\\
2&1&7
\end{array}
\right]
$$

Subtract twice the first row from the second row:

$$
R_2\rightarrow R_2-2R_1
$$

$$
\left[
\begin{array}{cc|c}
1&3&8\\
0&-5&-9
\end{array}
\right]
$$

Divide the second row by $-5$:

$$
R_2\rightarrow-\frac15R_2
$$

$$
\left[
\begin{array}{cc|c}
1&3&8\\
0&1&\frac95
\end{array}
\right]
$$

Subtract three times the second row from the first row:

$$
R_1\rightarrow R_1-3R_2
$$

$$
\left[
\begin{array}{cc|c}
1&0&\frac{13}{5}\\
0&1&\frac95
\end{array}
\right]
$$

Therefore:

$$
\boxed{
x=
\begin{pmatrix}
\frac{13}{5}\\
\frac95
\end{pmatrix}
}
$$

### 3. Verify the Solution

Both methods give the same solution:

$$
x=
\begin{pmatrix}
\frac{13}{5}\\
\frac95
\end{pmatrix}
$$

Substitute it into the original equation:

$$
Ax=
\begin{pmatrix}
2&1\\
1&3
\end{pmatrix}
\begin{pmatrix}
\frac{13}{5}\\
\frac95
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
\frac{26}{5}+\frac95\\
\frac{13}{5}+\frac{27}{5}
\end{pmatrix}
=
\begin{pmatrix}
7\\
8
\end{pmatrix}
=b
$$

The solution is correct.

### 4. Compare the Methods

Both methods give the same answer, but their essential steps are different.

**Inverse matrix method:**
1. Calculate the determinant.
2. Find the inverse matrix.
3. Multiply the inverse by the vector $b$.

This method requires three main calculation steps.

**Gaussian elimination method:**
1. Swap the rows.
2. Eliminate the first entry in the second row.
3. Make the second pivot equal to one.
4. Eliminate the second entry in the first row.

This method requires four main row operations.

For this example, the inverse matrix method is slightly simpler because it requires fewer essential calculation steps.

**Conclusion**

Both methods give the same solution:

$$
\boxed{
x=
\begin{pmatrix}
\frac{13}{5}\\
\frac95
\end{pmatrix}
}
$$

The inverse matrix method is simpler in this particular example because it requires fewer essential steps. Gaussian elimination is also correct, but it requires more row operations here.