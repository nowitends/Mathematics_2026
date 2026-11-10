## Exercise 4. Matrix Multiplication and Noncommutativity

### Question

For the matrices:
$$
A = \begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}, \quad
B = \begin{pmatrix}
2 & 0 \\
3 & 1
\end{pmatrix}
$$

Compute $AB$ and $BA$. Is $AB = BA$? Use this example to explain what noncommutativity of matrix multiplication means.

*Why this exercise:* shows one of the most important differences between matrix multiplication and multiplication of numbers.

---

### Solution

#### 1. Calculating $AB$
We multiply the rows of $A$ by the columns of $B$:
* Top-left: $(1)(2) + (2)(3) = 2 + 6 = 8$
* Top-right: $(1)(0) + (2)(1) = 0 + 2 = 2$
* Bottom-left: $(0)(2) + (1)(3) = 0 + 3 = 3$
* Bottom-right: $(0)(0) + (1)(1) = 0 + 1 = 1$

Putting it together:
$$
AB = \begin{pmatrix}
8 & 2 \\
3 & 1
\end{pmatrix}
$$

#### 2. Calculating $BA$
Now we multiply the rows of $B$ by the columns of $A$:
* Top-left: $(2)(1) + (0)(0) = 2 + 0 = 2$
* Top-right: $(2)(2) + (0)(1) = 4 + 0 = 4$
* Bottom-left: $(3)(1) + (1)(0) = 3 + 0 = 3$
* Bottom-right: $(3)(2) + (1)(1) = 6 + 1 = 7$

Putting it together:
$$
BA = \begin{pmatrix}
2 & 4 \\
3 & 7
\end{pmatrix}
$$

#### 3. Why $AB \neq BA$ (Noncommutativity)
Looking at our results:
$$
AB = \begin{pmatrix} 8 & 2 \\ 3 & 1 \end{pmatrix} \neq \begin{pmatrix} 2 & 4 \\ 3 & 7 \end{pmatrix} = BA
$$
Since $AB \neq BA$, matrix multiplication is **noncommutative**. In regular arithmetic, order doesn't change the product (like $2 \times 3 = 3 \times 2$), but with matrices, switching the order generally gives a completely different result.