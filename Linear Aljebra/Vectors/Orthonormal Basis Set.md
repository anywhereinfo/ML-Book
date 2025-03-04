# Orthonormal Basis Set

An **orthonormal basis set** is a special type of basis for a vector space where all basis vectors satisfy two conditions:

## 1. Orthogonality
Each pair of distinct basis vectors is **perpendicular**, meaning their inner product (dot product) is zero:

$$\mathbf{b}_i \cdot \mathbf{b}_j = 0, \quad \text{for } i \neq j$$

## 2. Normalization
Each basis vector has **unit length**, meaning its norm (magnitude) is 1:

$$\|\mathbf{b}_i\| = 1 \quad \Rightarrow \quad \mathbf{b}_i \cdot \mathbf{b}_i = 1$$

## Example in $\mathbb{R}^3$
The standard basis for $\mathbb{R}^3$ is an **orthonormal basis**:

$$B = \left\{
\begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix},
\begin{bmatrix} 0 \\ 1 \\ 0 \end{bmatrix},
\begin{bmatrix} 0 \\ 0 \\ 1 \end{bmatrix}
\right\}$$

- Each vector is **orthogonal** to the others.
- Each vector has **unit length**.

## Why is an Orthonormal Basis Useful?
- **Simplifies calculations** (dot products, projections, transformations).
- **Preserves lengths and angles** when changing coordinate systems.
- **Useful in Gram-Schmidt Process** to construct an orthonormal basis from a general basis.

---
**Related Topics**:  
[[Linear Algebra]] | [[Gram-Schmidt Process]] | [[Orthogonal Vectors]]

