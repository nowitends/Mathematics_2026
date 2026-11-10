## Exercise 15. Combining Determinant Properties

### Question

Let $A$ and $B$ be invertible $2 \times 2$ matrices with

$$
\det A = -2, \quad \det B = 3
$$

Without finding the entries of the matrices, compute

$$
\det \left( B^{-1} A^T B \right)
$$

State the determinant properties you use in order and explain why the factors involving $B$ eventually cancel.

---

### Solution

To compute $\det \left( B^{-1} A^T B \right)$ without explicitly knowing the entries of matrices $A$ and $B$, we apply fundamental properties of determinants step by step:

#### 1. Multiplicative Property of Determinants
The determinant of a product of square matrices is equal to the product of their individual determinants:
$$
\det(XY) = \det(X) \det(Y)
$$

Applying this to our expression with three matrix factors ($B^{-1}$, $A^T$, and $B$):
$$
\det \left( B^{-1} A^T B \right) = \det(B^{-1}) \cdot \det(A^T) \cdot \det(B)
$$

#### 2. Determinant of an Inverse Matrix
For any invertible matrix $B$, the determinant of its inverse is the reciprocal of its determinant:
$$
\det(B^{-1}) = \frac{1}{\det(B)}
$$

#### 3. Determinant of a Transpose Matrix
The determinant of a matrix's transpose is equal to the determinant of the original matrix:
$$
\det(A^T) = \det(A)
$$

---

#### 4. Combining and Simplifying (Why Factors Involving $B$ Cancel)
Substitute the properties from steps 2 and 3 back into our product:

$$
\det \left( B^{-1} A^T B \right) = \left( \frac{1}{\det(B)} \right) \cdot \det(A) \cdot \det(B)
$$

Rearranging the terms using commutativity of multiplication shows why the factors involving $B$ cancel out:

$$
= \left( \frac{\det(B)}{\det(B)} \right) \cdot \det(A)
$$

Since $\det(B) = 3 \neq 0$ (as $B$ is invertible), the term $\frac{\det(B)}{\det(B)} = 1$. Thus, the factors involving $B$ cancel each other out because the inverse matrix $B^{-1}$ and the matrix $B$ neutralize their scaling effects on the volume/determinant scale.

---

#### 5. Final Calculation
Substitute the given numerical values ($\det A = -2$ and $\det B = 3$):

$$
\det \left( B^{-1} A^T B \right) = \left( \frac{1}{3} \right) \cdot (-2) \cdot (3) = -2
$$

Therefore:

$$
\boxed{\det \left( B^{-1} A^T B \right) = -2}
$$

---

### Conclusion
* The determinant properties used in order are: the **multiplicative property** ($\det(XYZ) = \det(X)\det(Y)\det(Z)$), the **inverse property** ($\det(B^{-1}) = \frac{1}{\det(B)}$), and the **transpose property** ($\det(A^T) = \det(A)$).
* The factors involving $B$ cancel because $\det(B^{-1})\det(B) = \frac{1}{\det(B)}\det(B) = 1$, meaning similarity transformations preserve the determinant of the core matrix.