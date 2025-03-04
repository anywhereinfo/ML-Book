# Basis Vectors and Spanning Sets

## 1. Spanning Set
A **spanning set** of a vector space $V$  is a set of vectors such that **any vector in $V$ can be expressed as a **linear combination** of these vectors.

### Definition:
Given a set of vectors $S = \{ v_1, v_2, \dots, v_k \}$  in $V$ , if every vector $v$  in $V$ can be written as:

$$
v = \lambda_1 v_1 + \lambda_2 v_2 + \dots + \lambda_k v_k, \quad \lambda_i \in \mathbb{R}
$$

then \( S \) is said to **span** \( V \), and we write:

$$
V = \text{span}(S)
$$

### Example:
In $\mathbb{R}^2$ , the set 

$$
S = \left\{
\begin{bmatrix} 1 \\ 0 \end{bmatrix}, 
\begin{bmatrix} 0 \\ 1 \end{bmatrix}
\right\}
$$

spans $\mathbb{R}^2$  because any vector $v = \begin{bmatrix} x \\ y \end{bmatrix}$  can be written as:

$$v = x \begin{bmatrix} 1 \\ 0 \end{bmatrix} + y \begin{bmatrix} 0 \\ 1 \end{bmatrix}$$

---

## 2. Basis Vectors
A **basis** of a vector space $V$  is a **minimal spanning set**—a set of vectors that both:
1. **Spans \( V \)** (i.e., any vector in \( V \) can be written as a linear combination of them).
2. **Is linearly independent** (no vector in the set can be written as a linear combination of the others).

### Definition:
A set of vectors $B = \{ b_1, b_2, ..., b_n \}$  is a **basis** for $V$  if:
- It spans $V$.
- The vectors are **linearly independent**, meaning:

$$
\sum_{i=1}^{n} \lambda_i b_i = 0 \quad \Rightarrow \quad \lambda_i = 0 \text{ for all } i
$$

### Example in $\mathbb{R}^3$:
The **standard basis** for $\mathbb{R}^3$ is:

$$B = \left\{
\begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix},
\begin{bmatrix} 0 \\ 1 \\ 0 \end{bmatrix},
\begin{bmatrix} 0 \\ 0 \\ 1 \end{bmatrix}
\right\}$$

Every vector in $\mathbb{R}^3$  can be uniquely expressed as a linear combination of these basis vectors.

---

## 3. Key Properties:
- **Every vector space has at least one basis.**
- **Bases are not unique**, but all bases of the same vector space have the same number of elements.
- The **dimension** of $V$ , written as $\dim(V)$, is the number of basis vectors.

### Relation Between Basis and Spanning Set:
- A **spanning set** can contain **redundant** vectors.
- A **basis** is a **minimal spanning set** (i.e., removing any vector makes it no longer span \( V \)).

---
**Related Topics**:  
[[Linear Algebra]] | [[Orthonormal Basis]] | [[Vector Spaces]]
