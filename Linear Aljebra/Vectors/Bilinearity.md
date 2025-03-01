---
tags: linear-algebra, bilinearity, vector-spaces, transformations, inner-product
category: Mathematics
created: 2025-02-26
related: ["Vector Spaces.md", "Linear Transformations.md", "Inner Product.md", "Multilinear Algebra.md"]
---

# Bilinearity

> **Definition:**  
> A function $B: V \times W \to X$ is **bilinear** if it is **linear in each argument** separately.  
> This means that when we hold one argument fixed, the function behaves as a **linear transformation** in the other.

## **📌 Properties of a Bilinear Map**
A function $B(u, v)$ is **bilinear** if for all vectors $u, u', v, v'$ and scalars $\alpha, \beta$, it satisfies:

> **1️⃣ Linearity in the First Argument**  
> $$
 B(\alpha u + \beta u', v) = \alpha B(u, v) + \beta B(u', v)
 $$
> - The function distributes **over vector addition** in the first argument.
> - The function **scales linearly** in the first argument.

> **2️⃣ Linearity in the Second Argument**  
> $$
 B(u, \alpha v + \beta v') = \alpha B(u, v) + \beta B(u, v')
 $$
> - The function distributes **over vector addition** in the second argument.
> - The function **scales linearly** in the second argument.

✅ **A function is bilinear if and only if it is linear in each argument separately!**

---

## **📌 Examples of Bilinear Maps**
### **✅ 1. Inner Product as a Bilinear Form**
The inner product $\langle u, v \rangle$ is **bilinear in real vector spaces**:
$$
\langle \alpha u + \beta u', v \rangle = \alpha \langle u, v \rangle + \beta \langle u', v \rangle
$$
$$
\langle u, \alpha v + \beta v' \rangle = \alpha \langle u, v \rangle + \beta \langle u, v' \rangle
$$
However, in **complex vector spaces**, the inner product is **not bilinear** but rather **sesquilinear** due to the conjugate symmetry.

---

### **✅ 2. Matrix Multiplication as a Bilinear Map**
If $A$ is an $m \times n$ matrix and $B$ is an $n \times p$ matrix, then matrix multiplication defines a **bilinear operation**:
$$
C = AB
$$
where
$$
(A + A')B = AB + A'B, \quad A(B + B') = AB + AB'
$$
✅ **This shows matrix multiplication distributes over addition in both arguments, making it bilinear.**

---

### **✅ 3. Determinant as a Bilinear Function**
For a **$2 \times 2$ determinant**, the determinant function is **bilinear in rows (or columns)**:
$$
\det
\begin{bmatrix} 
a_1 + b_1 & a_2 + b_2 \\ 
c_1 & c_2
\end{bmatrix}
=
\det
\begin{bmatrix} 
a_1 & a_2 \\ 
c_1 & c_2
\end{bmatrix}
+
\det
\begin{bmatrix} 
b_1 & b_2 \\ 
c_1 & c_2
\end{bmatrix}
$$
✅ **This means determinants satisfy bilinearity in each row/column separately.**

---

## **📌 Bilinear Forms and Quadratic Forms**
A **bilinear form** is a bilinear function that maps two vectors to a scalar:
$$
B(u, v) = u^T A v
$$
- If **$A$ is symmetric**, then $B(u, v)$ defines a **quadratic form**:
  $$
  Q(u) = B(u, u) = u^T A u
  $$
- Quadratic forms appear in **machine learning, optimization, and physics**.

✅ **Examples:**
- **Energy in physics**: The quadratic form represents **potential energy**.
- **Variance in statistics**: Covariance matrices use **quadratic forms**.

---

## **📌 Why Bilinearity Matters**
- **Generalizes linearity** to functions of **two arguments**.
- **Appears in physics, computer science, and machine learning**.
- **Foundation for multilinear algebra and tensor analysis**.

---

## **🔗 Related Topics**
- [[Inner Product]]


---

## **🚀 Summary**
✅ **A function is bilinear if it is linear in each argument separately.**  
✅ **Common examples include inner products, matrix multiplication, and determinants.**  
✅ **Bilinear forms lead to important applications in machine learning, physics, and optimization.**  

---
