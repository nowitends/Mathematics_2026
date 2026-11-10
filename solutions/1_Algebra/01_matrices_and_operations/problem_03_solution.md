## Exercise 3. When Can Matrices Be Multiplied?

### Question

The matrix sizes are given as:
$$A_{2 \times 3}, \quad B_{3 \times 4}, \quad C_{4 \times 2}, \quad D_{2 \times 2}$$

For the products:
$$AB, \quad BA, \quad BC, \quad CB, \quad AC, \quad CA, \quad AD, \quad DA$$

Determine whether they are defined. If so, state the size of the result. Justify each decision using the dimension compatibility condition.

*Why this exercise:* forces an understanding of dimension compatibility before carrying out any calculation.

---

### Solution

To check if we can multiply two matrices $XY$, the inner dimensions must be equal. Specifically, if $X$ is $m \times n$ and $Y$ is $p \times q$, the product exists only when $n = p$, and the resulting matrix will have dimensions $m \times q$.

#### 1. Product $AB$
* **Sizes:** $A_{2 \times 3}$ and $B_{3 \times 4}$
* **Check:** Inner numbers match ($3 = 3$).
* **Conclusion:** **Defined**, size is **$2 \times 4$**.

#### 2. Product $BA$
* **Sizes:** $B_{3 \times 4}$ and $A_{2 \times 3}$
* **Check:** Inner numbers do not match ($4 \neq 2$).
* **Conclusion:** **Undefined**.

#### 3. Product $BC$
* **Sizes:** $B_{3 \times 4}$ and $C_{4 \times 2}$
* **Check:** Inner numbers match ($4 = 4$).
* **Conclusion:** **Defined**, size is **$3 \times 2$**.

#### 4. Product $CB$
* **Sizes:** $C_{4 \times 2}$ and $B_{3 \times 4}$
* **Check:** Inner numbers do not match ($2 \neq 3$).
* **Conclusion:** **Undefined**.

#### 5. Product $AC$
* **Sizes:** $A_{2 \times 3}$ and $C_{4 \times 2}$
* **Check:** Inner numbers do not match ($3 \neq 4$).
* **Conclusion:** **Undefined**.

#### 6. Product $CA$
* **Sizes:** $C_{4 \times 2}$ and $A_{2 \times 3}$
* **Check:** Inner numbers match ($2 = 2$).
* **Conclusion:** **Defined**, size is **$4 \times 3$**.

#### 7. Product $AD$
* **Sizes:** $A_{2 \times 3}$ and $D_{2 \times 2}$
* **Check:** Inner numbers do not match ($3 \neq 2$).
* **Conclusion:** **Undefined**.

#### 8. Product $DA$
* **Sizes:** $D_{2 \times 2}$ and $A_{2 \times 3}$
* **Check:** Inner numbers match ($2 = 2$).
* **Conclusion:** **Defined**, size is **$2 \times 3$**.