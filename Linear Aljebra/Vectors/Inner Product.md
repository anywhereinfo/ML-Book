---
tags:
  - linear-aljebra
  - inner-product
  - dot-product
---

# Inner Product

> **Definition:**  
> The inner product is an operation that takes two vectors and returns a scalar, serving as the foundation for computing **length, angles, projections, and similarity**.
> 
> $$
 \langle u, v \rangle = u^T v = \sum_{i=1}^{n} u_i v_i
 $$

## Applications
- [[Vector Norms (Length)]]
- [[Orthogonality]]
- [[Angle Between Vectors]]
- [[Projection]]
- [[Cosine Similarity]]
- [[Gram-Schmidt Process]]

---

## **Properties**
> **1️⃣ Linearity:**  
> $$\langle au + bv, w \rangle = a \langle u, w \rangle + b \langle v, w \rangle$$
>
> **2️⃣ Symmetry:**  
> $$\langle u, v \rangle = \langle v, u \rangle$$
>
> **3️⃣ Positive Definiteness:**  
> $$\langle v, v \rangle \geq 0, \quad \text{and } \langle v, v \rangle = 0 \text{ iff } v = 0$$

---
## 📌 Generalized Inner Product with a Matrix
> When using a **positive definite matrix** \( A \), we define a **generalized inner product**:
> 
> $$
 \langle u, v \rangle_A = u^T A v
 $$
> 
> Where:
> - \( A \) is a **symmetric ($A = A^T$ ) , positive definite matrix ($x^TAx >0$)**.
> - This inner product is commonly used in **quadratic forms
> - Mahalanobis distance, and machine learning kernels**.

## 📌 Special Cases
> **1️⃣ Standard Inner Product** → When \( A = I \) (Identity matrix), we recover the **dot product**:
> 
> $$
> \langle u, v \rangle_I = u^T I v = u^T v
> $$
> 
> **2️⃣ Weighted Inner Product** → If \( A \) scales different components differently:
> 
> $$
> \langle u, v \rangle_A = u^T A v
> $$
> 
> Used in **quadratic forms and optimization**.




