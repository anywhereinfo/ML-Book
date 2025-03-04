## Length of a Vector (Norm) Using the Euclidean Inner Product

The **Euclidean inner product** (also called the **dot product**) in $\mathbb{R}^n$ is defined as:

$$\langle x, x \rangle = x^T x = \sum_{i=1}^{n} x_i^2$$

The **Euclidean norm** (length of a vector $ x $) is then:

$$\|x\| = \sqrt{x^T x}$$

### Example:

For $x = [3, 4]$:

$$\|x\| = \sqrt{3^2 + 4^2} = \sqrt{9 + 16} = \sqrt{25} = 5$$

---

## 2. Length of a Vector Using a Matrix-Defined Inner Product

In a **generalized inner product space**, the inner product is defined by a **positive definite matrix** $A$:

$$\langle x, x \rangle_A = x^T A x$$

The corresponding **norm** (or length) of $x$ is:

$$\|x\|_A = \sqrt{x^T A x}$$

### Example:

Let $x = [1, -1, 3]$ and the inner product matrix:

$$A = \begin{bmatrix} 2 & 1 & 0 \\ 1 & 2 & -1 \\ 0 & -1 & 2 \end{bmatrix}$$

Then, the length is:

$$\|x\|_A = \sqrt{x^T A x}$$

---

## Comparison of Euclidean vs. Matrix-Induced Norms

| Method                  | Formula            | When to Use                                                               |
| ----------------------- | ------------------ | ------------------------------------------------------------------------- |
| **Euclidean Norm**      | $$\sqrt{x^T x}$$   | Standard distance in $\mathbb{R}^n$                                       |
| **Matrix-Induced Norm** | $$\sqrt{x^T A x}$$ | Weighted distance based on matrix $A$ (e.g., in **Mahalanobis distance**) |

---

## Key Takeaways

- The **Euclidean norm** is a special case of the **matrix-induced norm** where $A$ is the identity matrix.
- The **matrix-induced norm** allows for distance calculations in **weighted spaces** or **non-Euclidean geometries**.

## Related to
[[Distance between Vectors]]