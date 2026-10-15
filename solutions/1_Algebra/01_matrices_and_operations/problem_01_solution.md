
# Matrices and Basic Operations

## Solutions

---

## Basic Exercises

### Exercise 1. Matrix Size and Entries

Given

$$
A=\begin{pmatrix}2&-1&3\\0&4&5\end{pmatrix},
\qquad
B=\begin{pmatrix}1&0\\-2&3\\4&1\end{pmatrix}.
$$

**1. Matrix sizes:**

$$
\boxed{A:2\times3,\qquad B:3\times2}
$$

**2. Matrix entries:**

$$
\boxed{a_{12}=-1,\quad a_{23}=5,\quad b_{21}=-2,\quad b_{32}=1}
$$

**3. Row and column vectors:**

Second row of $A$:

$$
\boxed{\begin{pmatrix}0&4&5\end{pmatrix}}
$$

First column of $B$:

$$
\boxed{\begin{pmatrix}1\\-2\\4\end{pmatrix}}
$$

**Explanation:** The entry $a_{ij}$ is located in row $i$ and column $j$.

---

### Exercise 2. Addition and Scalar Multiplication

Given

$$
A=\begin{pmatrix}1&2\\-1&3\end{pmatrix},
\qquad
B=\begin{pmatrix}4&-2\\0&5\end{pmatrix}.
$$

**1. Addition:**

$$
A+B=
\begin{pmatrix}
1+4&2+(-2)\\
-1+0&3+5
\end{pmatrix}
$$

$$
\boxed{A+B=\begin{pmatrix}5&0\\-1&8\end{pmatrix}}
$$

**2. Subtraction:**

$$
A-B=
\begin{pmatrix}
1-4&2-(-2)\\
-1-0&3-5
\end{pmatrix}
$$

$$
\boxed{A-B=\begin{pmatrix}-3&4\\-1&-2\end{pmatrix}}
$$

**3. Scalar multiplication:**

$$
3A=\begin{pmatrix}3&6\\-3&9\end{pmatrix}
$$

$$
2B=\begin{pmatrix}8&-4\\0&10\end{pmatrix}
$$

Therefore,

$$
\boxed{3A-2B=\begin{pmatrix}-5&10\\-3&-1\end{pmatrix}}
$$

**Explanation:** Matrix addition and subtraction are performed entry by entry. They are defined only when both matrices have the same dimensions.

---

### Exercise 3. When Can Matrices Be Multiplied?

Given matrix dimensions:

$$
A_{2\times3},\quad B_{3\times4},\quad
C_{4\times2},\quad D_{2\times2}.
$$

**Multiplication rule:**

$$
(m\times n)(n\times p)=m\times p
$$

The number of columns of the first matrix must equal the number of rows of the second matrix.

| Product | Defined? | Result Size |
|---|---|---|
| $AB$ | Yes | $2\times4$ |
| $BA$ | No | $4\neq2$ |
| $BC$ | Yes | $3\times2$ |
| $CB$ | No | $2\neq3$ |
| $AC$ | No | $3\neq4$ |
| $CA$ | Yes | $4\times3$ |
| $AD$ | No | $3\neq2$ |
| $DA$ | Yes | $2\times3$ |

**Verification example:**

$$
AB=(2\times3)(3\times4)
$$

The inner dimensions are equal, so the product is defined and has size $2\times4$.

---

### Exercise 4. Matrix Multiplication and Noncommutativity

Given

$$
A=\begin{pmatrix}1&2\\0&1\end{pmatrix},
\qquad
B=\begin{pmatrix}2&0\\3&1\end{pmatrix}.
$$

**1. Calculate $AB$:**

$$
AB=
\begin{pmatrix}
1(2)+2(3)&1(0)+2(1)\\
0(2)+1(3)&0(0)+1(1)
\end{pmatrix}
$$

$$
\boxed{AB=\begin{pmatrix}8&2\\3&1\end{pmatrix}}
$$

**2. Calculate $BA$:**

$$
BA=
\begin{pmatrix}
2(1)+0(0)&2(2)+0(1)\\
3(1)+1(0)&3(2)+1(1)
\end{pmatrix}
$$

$$
\boxed{BA=\begin{pmatrix}2&4\\3&7\end{pmatrix}}
$$

**Conclusion:**

$$
\boxed{AB\neq BA}
$$

**Explanation:** Matrix multiplication is generally not commutative. Changing the order of multiplication can change the result.

---

### Exercise 5. Matrix Times Vector

Given

$$
A=\begin{pmatrix}2&-1\\1&3\end{pmatrix},
\qquad
x=\begin{pmatrix}4\\2\end{pmatrix}.
$$

**Matrix-vector multiplication:**

$$
Ax=
\begin{pmatrix}
2(4)+(-1)(2)\\
1(4)+3(2)
\end{pmatrix}
$$

$$
\boxed{Ax=\begin{pmatrix}6\\10\end{pmatrix}}
$$

**Linear combination of columns:**

$$
Ax=
4\begin{pmatrix}2\\1\end{pmatrix}
+
2\begin{pmatrix}-1\\3\end{pmatrix}
$$

$$
=
\begin{pmatrix}8\\4\end{pmatrix}
+
\begin{pmatrix}-2\\6\end{pmatrix}
=
\boxed{\begin{pmatrix}6\\10\end{pmatrix}}
$$

**Explanation:** Matrix-vector multiplication is a linear combination of the columns of the matrix, using the entries of the vector as coefficients.

---

### Exercise 6. Transpose

Given

$$
A=\begin{pmatrix}1&2&3\\4&5&6\end{pmatrix},
\qquad
B=\begin{pmatrix}1&0\\2&1\\-1&3\end{pmatrix}.
$$

**1. Calculate $A^T$:**

$$
\boxed{
A^T=
\begin{pmatrix}
1&4\\
2&5\\
3&6
\end{pmatrix}
}
$$

**2. Calculate $B^T$:**

$$
\boxed{
B^T=
\begin{pmatrix}
1&2&-1\\
0&1&3
\end{pmatrix}
}
$$

**3. Calculate $AB$:**

$$
AB=
\begin{pmatrix}
1+4-3&0+2+9\\
4+10-6&0+5+18
\end{pmatrix}
$$

$$
\boxed{
AB=\begin{pmatrix}2&11\\8&23\end{pmatrix}
}
$$

**4. Verify $(AB)^T=B^TA^T$:**

$$
(AB)^T=\begin{pmatrix}2&8\\11&23\end{pmatrix}
$$

Also,

$$
B^TA^T=
\begin{pmatrix}1&2&-1\\0&1&3\end{pmatrix}
\begin{pmatrix}1&4\\2&5\\3&6\end{pmatrix}
$$

$$
=\begin{pmatrix}2&8\\11&23\end{pmatrix}
$$

Therefore,

$$
\boxed{(AB)^T=B^TA^T}
$$

**Explanation:** Transposition exchanges rows and columns. The transpose of a product reverses the order of its factors.

---

### Exercise 7. Identity Matrix, Zero Matrix, and Powers

Given

$$
A=\begin{pmatrix}2&1\\0&2\end{pmatrix}.
$$

Identity and zero matrices:

$$
I=\begin{pmatrix}1&0\\0&1\end{pmatrix},
\qquad
0=\begin{pmatrix}0&0\\0&0\end{pmatrix}.
$$

**1. Identity multiplication:**

$$
\boxed{AI=IA=\begin{pmatrix}2&1\\0&2\end{pmatrix}}
$$

**2. Addition with zero matrix:**

$$
\boxed{A+0=\begin{pmatrix}2&1\\0&2\end{pmatrix}}
$$

**3. Calculate $A^2$:**

$$
A^2=
\begin{pmatrix}2&1\\0&2\end{pmatrix}
\begin{pmatrix}2&1\\0&2\end{pmatrix}
$$

$$
\boxed{A^2=\begin{pmatrix}4&4\\0&4\end{pmatrix}}
$$

**4. Calculate $A^3$:**

$$
A^3=A^2A
$$

$$
=\begin{pmatrix}4&4\\0&4\end{pmatrix}
\begin{pmatrix}2&1\\0&2\end{pmatrix}
$$

$$
\boxed{A^3=\begin{pmatrix}8&12\\0&8\end{pmatrix}}
$$

**Pattern:**

$$
\boxed{
A^n=
\begin{pmatrix}
2^n&n2^{n-1}\\
0&2^n
\end{pmatrix}
}
$$

**Explanation:** The identity matrix is the multiplicative neutral element, while the zero matrix is the additive neutral element. The diagonal entries double with each power.

---

### Exercise 8. Row Operations and Their Reversibility

Given

$$
A=
\begin{pmatrix}
1&2&-1\\
2&4&1\\
-1&1&3
\end{pmatrix}.
$$

**Step 1: $R_2\leftarrow R_2-2R_1$**

$$
R_2=(2,4,1)-2(1,2,-1)=(0,0,3)
$$

$$
\boxed{
A_1=
\begin{pmatrix}
1&2&-1\\
0&0&3\\
-1&1&3
\end{pmatrix}
}
$$

**Step 2: $R_3\leftarrow R_3+R_1$**

$$
R_3=(-1,1,3)+(1,2,-1)=(0,3,2)
$$

$$
\boxed{
A_2=
\begin{pmatrix}
1&2&-1\\
0&0&3\\
0&3&2
\end{pmatrix}
}
$$

**Step 3: Interchange $R_2$ and $R_3$**

$$
\boxed{
A_3=
\begin{pmatrix}
1&2&-1\\
0&3&2\\
0&0&3
\end{pmatrix}
}
$$

**Inverse operations:**

1. $R_2\leftarrow R_2+2R_1$
2. $R_3\leftarrow R_3-R_1$
3. Interchange $R_2$ and $R_3$ again.

**Verification:** Applying the inverse operations in reverse order to $A_3$ restores the original matrix $A$.

**Explanation:** Elementary row operations are reversible. Each operation can be undone by a corresponding inverse operation.

---

### Exercise 9. Composing Transformations

Given

$$
S=\begin{pmatrix}2&0\\0&1\end{pmatrix},
\qquad
R=\begin{pmatrix}0&-1\\1&0\end{pmatrix},
\qquad
x=\begin{pmatrix}1\\2\end{pmatrix}.
$$

**1. Calculate $RSx$:**

First apply scaling:

$$
Sx=
\begin{pmatrix}2&0\\0&1\end{pmatrix}
\begin{pmatrix}1\\2\end{pmatrix}
=
\begin{pmatrix}2\\2\end{pmatrix}
$$

Then rotate:

$$
RSx=
\begin{pmatrix}0&-1\\1&0\end{pmatrix}
\begin{pmatrix}2\\2\end{pmatrix}
$$

$$
\boxed{RSx=\begin{pmatrix}-2\\2\end{pmatrix}}
$$

**2. Calculate $SRx$:**

First rotate:

$$
Rx=
\begin{pmatrix}0&-1\\1&0\end{pmatrix}
\begin{pmatrix}1\\2\end{pmatrix}
=
\begin{pmatrix}-2\\1\end{pmatrix}
$$

Then scale:

$$
SRx=
\begin{pmatrix}2&0\\0&1\end{pmatrix}
\begin{pmatrix}-2\\1\end{pmatrix}
$$

$$
\boxed{SRx=\begin{pmatrix}-4\\1\end{pmatrix}}
$$

**Conclusion:**

$$
\boxed{RSx\neq SRx}
$$

**Explanation:** Scaling before rotation gives a different result from rotation before scaling. The scaling matrix stretches the horizontal coordinate, while rotation changes the direction of the vector.

---

### Exercise 10. Columns of a Matrix Product

Given

$$
A=\begin{pmatrix}1&2&0\\0&1&1\end{pmatrix},
\qquad
B=\begin{pmatrix}1&2\\-1&0\\3&1\end{pmatrix}.
$$

The columns of $B$ are

$$
b_1=\begin{pmatrix}1\\-1\\3\end{pmatrix},
\qquad
b_2=\begin{pmatrix}2\\0\\1\end{pmatrix}.
$$

**1. Calculate $Ab_1$:**

$$
Ab_1=
\begin{pmatrix}
1(1)+2(-1)+0(3)\\
0(1)+1(-1)+1(3)
\end{pmatrix}
$$

$$
\boxed{Ab_1=\begin{pmatrix}-1\\2\end{pmatrix}}
$$

**2. Calculate $Ab_2$:**

$$
Ab_2=
\begin{pmatrix}
1(2)+2(0)+0(1)\\
0(2)+1(0)+1(1)
\end{pmatrix}
$$

$$
\boxed{Ab_2=\begin{pmatrix}2\\1\end{pmatrix}}
$$

**3. Calculate $AB$:**

$$
AB=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
\begin{pmatrix}
1&2\\
-1&0\\
3&1
\end{pmatrix}
$$

$$
\boxed{
AB=\begin{pmatrix}-1&2\\2&1\end{pmatrix}
}
$$

**Verification:**

$$
\boxed{AB=\begin{pmatrix}Ab_1&Ab_2\end{pmatrix}}
$$

**Explanation:** Each column of the product $AB$ is obtained by multiplying $A$ by the corresponding column of $B$.

---

## More Challenging Exercises

### Exercise 11. When Do Matrices Commute?

Given

$$
A=\begin{pmatrix}1&1\\0&1\end{pmatrix},
\qquad
B=\begin{pmatrix}a&b\\c&d\end{pmatrix}.
$$

We want to find when

$$
AB=BA.
$$

**1. Calculate $AB$:**

$$
AB=
\begin{pmatrix}
a+c&b+d\\
c&d
\end{pmatrix}
$$

**2. Calculate $BA$:**

$$
BA=
\begin{pmatrix}
a&a+b\\
c&c+d
\end{pmatrix}
$$

**3. Compare corresponding entries:**

$$
a+c=a\Rightarrow c=0
$$

$$
b+d=a+b\Rightarrow d=a
$$

The remaining equations are then automatically satisfied.

**Final answer:**

$$
\boxed{c=0,\qquad d=a}
$$

Thus,

$$
\boxed{
B=\begin{pmatrix}a&b\\0&a\end{pmatrix}
}
$$

where $a,b$ are arbitrary real numbers.

**Verification:**

For this form of $B$,

$$
AB=BA=
\begin{pmatrix}
a&a+b\\
0&a
\end{pmatrix}.
$$

**Explanation:** These are exactly the matrices that commute with $A$.

---

### Exercise 12. Formula for a Matrix Power

Given

$$
A=\begin{pmatrix}1&1\\0&1\end{pmatrix}.
$$

**1. Calculate powers:**

$$
A^2=
\begin{pmatrix}1&2\\0&1\end{pmatrix}
$$

$$
A^3=
\begin{pmatrix}1&3\\0&1\end{pmatrix}
$$

$$
A^4=
\begin{pmatrix}1&4\\0&1\end{pmatrix}
$$

**2. General formula:**

$$
\boxed{
A^n=\begin{pmatrix}1&n\\0&1\end{pmatrix}
}
$$

**3. Proof by mathematical induction:**

Base case $n=1$:

$$
A^1=\begin{pmatrix}1&1\\0&1\end{pmatrix}
$$

The formula is true.

Assume it is true for $n$:

$$
A^n=\begin{pmatrix}1&n\\0&1\end{pmatrix}.
$$

Then

$$
A^{n+1}=A^nA
$$

$$
=
\begin{pmatrix}1&n\\0&1\end{pmatrix}
\begin{pmatrix}1&1\\0&1\end{pmatrix}
$$

$$
=
\begin{pmatrix}1&n+1\\0&1\end{pmatrix}.
$$

Therefore,

$$
\boxed{
A^n=\begin{pmatrix}1&n\\0&1\end{pmatrix}
}
$$

for every positive integer $n$.

**Explanation:** Since the base case and induction step are true, the formula follows by mathematical induction.

---

### Exercise 13. A Recurrence Written in Matrix Form

Given

$$
F=\begin{pmatrix}1&1\\1&0\end{pmatrix}.
$$

**1. Calculate $F^2$:**

$$
F^2=
\begin{pmatrix}1&1\\1&0\end{pmatrix}
\begin{pmatrix}1&1\\1&0\end{pmatrix}
$$

$$
\boxed{F^2=\begin{pmatrix}2&1\\1&1\end{pmatrix}}
$$

**2. Calculate $F^3$:**

$$
\boxed{F^3=\begin{pmatrix}3&2\\2&1\end{pmatrix}}
$$

**3. Calculate $F^4$:**

$$
\boxed{F^4=\begin{pmatrix}5&3\\3&2\end{pmatrix}}
$$

**4. Calculate $F^5$:**

$$
\boxed{F^5=\begin{pmatrix}8&5\\5&3\end{pmatrix}}
$$

**Fibonacci relationship:**

The sequence is

$$
0,1,1,2,3,5,8,\ldots
$$

Each term is the sum of the two previous terms:

$$
f_{n+1}=f_n+f_{n-1}.
$$

The general matrix formula is

$$
\boxed{
F^n=
\begin{pmatrix}
f_{n+1}&f_n\\
f_n&f_{n-1}
\end{pmatrix}
}
$$

for $n\geq1$, where $f_0=0$ and $f_1=1$.

**5. Matrix-vector multiplication:**

$$
F\begin{pmatrix}a\\b\end{pmatrix}
=
\begin{pmatrix}1&1\\1&0\end{pmatrix}
\begin{pmatrix}a\\b\end{pmatrix}
$$

$$
\boxed{
F\begin{pmatrix}a\\b\end{pmatrix}
=
\begin{pmatrix}a+b\\a\end{pmatrix}
}
$$

**Explanation:** The multiplication creates the sum $a+b$ and preserves $a$. This performs one step of the Fibonacci recurrence.

---

### Exercise 14. Rotation Matrices

Given

$$
R(\theta)=
\begin{pmatrix}
\cos\theta&-\sin\theta\\
\sin\theta&\cos\theta
\end{pmatrix}.
$$

We want to prove

$$
R(\alpha)R(\beta)=R(\alpha+\beta).
$$

**1. Multiply the matrices:**

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha&-\sin\alpha\\
\sin\alpha&\cos\alpha
\end{pmatrix}
\begin{pmatrix}
\cos\beta&-\sin\beta\\
\sin\beta&\cos\beta
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
\cos\alpha\cos\beta-\sin\alpha\sin\beta&
-\cos\alpha\sin\beta-\sin\alpha\cos\beta\\
\sin\alpha\cos\beta+\cos\alpha\sin\beta&
-\sin\alpha\sin\beta+\cos\alpha\cos\beta
\end{pmatrix}
$$

**2. Use trigonometric identities:**

$$
\cos(\alpha+\beta)
=\cos\alpha\cos\beta-\sin\alpha\sin\beta
$$

$$
\sin(\alpha+\beta)
=\sin\alpha\cos\beta+\cos\alpha\sin\beta
$$

Therefore,

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos(\alpha+\beta)&-\sin(\alpha+\beta)\\
\sin(\alpha+\beta)&\cos(\alpha+\beta)
\end{pmatrix}
$$

**Final result:**

$$
\boxed{R(\alpha)R(\beta)=R(\alpha+\beta)}
$$

**Geometric explanation:** Rotating a vector by $\beta$ and then by $\alpha$ is equivalent to rotating it once by the total angle $\alpha+\beta$.

---

### Exercise 15. Associativity of Multiplication and Different Calculation Paths

Given

$$
A=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix},
\quad
B=
\begin{pmatrix}
1&0\\
2&1\\
-1&3
\end{pmatrix},
\quad
C=
\begin{pmatrix}
2&1\\
0&-1
\end{pmatrix}.
$$

**1. Calculate $(AB)C$:**

First calculate $AB$:

$$
AB=
\begin{pmatrix}
1+4+0&0+2+0\\
0+2-1&0+1+3
\end{pmatrix}
$$

$$
AB=\begin{pmatrix}5&2\\1&4\end{pmatrix}
$$

Now multiply by $C$:

$$
(AB)C=
\begin{pmatrix}5&2\\1&4\end{pmatrix}
\begin{pmatrix}2&1\\0&-1\end{pmatrix}
$$

$$
\boxed{
(AB)C=\begin{pmatrix}10&3\\2&-3\end{pmatrix}
}
$$

**2. Calculate $A(BC)$:**

First calculate $BC$:

$$
BC=
\begin{pmatrix}
1&0\\
2&1\\
-1&3
\end{pmatrix}
\begin{pmatrix}
2&1\\
0&-1
\end{pmatrix}
$$

$$
BC=
\begin{pmatrix}
2&1\\
4&1\\
-2&-4
\end{pmatrix}
$$

Now multiply by $A$:

$$
A(BC)=
\begin{pmatrix}
1&2&0\\
0&1&1
\end{pmatrix}
\begin{pmatrix}
2&1\\
4&1\\
-2&-4
\end{pmatrix}
$$

$$
\boxed{
A(BC)=\begin{pmatrix}10&3\\2&-3\end{pmatrix}
}
$$

**3. Compare results:**

$$
\boxed{
(AB)C=A(BC)=
\begin{pmatrix}10&3\\2&-3\end{pmatrix}
}
$$

**4. Compare computational costs:**

Counting scalar multiplications:

For $(AB)C$:

- $AB$: $2\cdot2\cdot3=12$
- $(AB)C$: $2\cdot2\cdot2=8$
- Total: $20$ scalar multiplications.

For $A(BC)$:

- $BC$: $3\cdot2\cdot2=12$
- $A(BC)$: $2\cdot2\cdot3=12$
- Total: $24$ scalar multiplications.

**Conclusion:**

$$
\boxed{20<24}
$$

The first calculation path requires fewer scalar multiplications.

**Explanation:** Matrix multiplication is associative, meaning that changing the grouping of factors does not change the result. However, the grouping can affect the number of operations required.

---

## Conclusion

These exercises demonstrate the fundamental properties of matrices:

- Matrix dimensions determine which operations are possible.
- Addition and subtraction are performed entry by entry.
- Matrix multiplication is generally noncommutative.
- Matrix-vector multiplication represents a linear combination of columns.
- Transposition reverses the order of multiplication.
- Matrix powers can follow predictable patterns.
- Row operations are reversible.
- Matrices can represent geometric transformations.
- Matrix multiplication is associative.
- Matrix powers can describe recurrence relations such as the Fibonacci sequence.
