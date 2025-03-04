# Distance Between Vectors in Inner Product Spaces

## 1. Distance Using the Euclidean Inner Product
The **Euclidean inner product** (dot product) in $\mathbb{R}^n$ is defined as:

$$\langle x, y \rangle = x^T y = \sum_{i=1}^{n} x_i y_i$$

The **Euclidean distance** between two vectors $ x $ and $ y $ is given by:

$$\|x - y\| = \sqrt{(x - y)^T (x - y)}$$

### Example:
For $x = [3, 4]$ and $y = [0, 0]$:

$$\|x - y\| = \sqrt{(3-0)^2 + (4-0)^2} = \sqrt{9 + 16} = \sqrt{25} = 5$$

---

## 2. Distance Using a Matrix-Defined Inner Product
In a **generalized inner product space**, the inner product is defined by a **positive definite matrix** $A$:

$$\langle x, y \rangle_A = x^T A y$$

The corresponding **distance** is given by:

$$\|x - y\|_A = \sqrt{(x - y)^T A (x - y)}$$

### Example:
Let $x = [1, -1, 3]$ and $y = [0, 1, 0]$, and define the inner product matrix:

$$A =
\begin{bmatrix}
2 & 1 & 0 \\
1 & 2 & -1 \\
0 & -1 & 2
\end{bmatrix}$$

Then, the squared distance is:

$$\|x - y\|_A^2 = (x - y)^T A (x - y)$$

Taking the square root gives the final distance.

---

## Comparison of Euclidean vs. Matrix-Induced Distance
| Method                      | Formula                        | When to Use                                                               |
| --------------------------- | ------------------------------ | ------------------------------------------------------------------------- |
| **Euclidean Distance**      | $$\sqrt{(x - y)^T (x - y)}$$   | Standard distance in $\mathbb{R}^n$                                       |
| **Matrix-Induced Distance** | $$\sqrt{(x - y)^T A (x - y)}$$ | Weighted distance based on matrix $A$ (e.g., in **Mahalanobis distance**) |

---

## Key Takeaways
- The **Euclidean distance** is a special case of the **matrix-induced distance** where $A$ is the identity matrix.
- The **matrix-induced distance** allows for distance calculations in **weighted spaces** or **non-Euclidean geometries**.
