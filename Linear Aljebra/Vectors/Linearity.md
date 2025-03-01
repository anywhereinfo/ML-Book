---
tags: linear-algebra, linearity, vector-spaces, transformations
category: Mathematics
created: 2025-02-26
related: ["Vector Spaces.md", "Linear Transformations.md", "Inner Product.md"]
---

# What It Means to Be Linear

> **Definition:**  
> A function, transformation, or system is **linear** if it satisfies the properties of **additivity** and **homogeneity**. These properties ensure that the operation preserves vector space structure.

## **📌 Properties of Linearity**
A function $f: V \to W$ is **linear** if for all vectors $u, v \in V$ and scalars $\alpha, \beta$, it satisfies:

> **1️⃣ Additivity (Distributes Over Addition)**  
> $$
 f(u + v) = f(u) + f(v)
 $$
> - The function preserves **vector addition**.
> - The output of the sum of two inputs is the sum of their individual outputs.

> **2️⃣ Homogeneity (Scales Properly)**  
> $$
 f(\alpha u) = \alpha f(u)
 $$
> - Scaling the input scales the output by the same factor.
> - Ensures proportionality in transformations.

✅ **A function is linear if and only if it satisfies both conditions!**

---

## **📌 Examples of Linear and Non-Linear Functions**
### **✅ Linear Examples**
1. **Linear Transformations (Matrix Multiplication)**  
   If \( A \) is an $m \times n$  matrix, then the function:
   $$
   f(x) = Ax
   $$
   is **linear**, because matrix multiplication **preserves addition and scaling**.

2. **Derivative as a Linear Operator**  
   The derivative operator \( D \) is linear because:
   $$
   D(f + g) = Df + Dg, \quad D(\alpha f) = \alpha Df
   $$

3. **Inner Product as a Linear Map**  
   The inner product $\langle u, v \rangle$ is **linear in each argument**:
   $$
   \langle \alpha u + \beta v, w \rangle = \alpha \langle u, w \rangle + \beta \langle v, w \rangle
   $$

---

### **❌ Non-Linear Examples**
1. **Quadratic Functions**  
   $$
   f(x) = x^2
   $$
   **Fails additivity:**  
   $$
   f(x + y) = (x + y)^2 \neq f(x) + f(y)
   $$

2. **Trigonometric Functions (e.g., Sine and Cosine)**  
   $$
   f(x) = \sin(x)
   $$
   **Fails scaling:**  
   $$
   \sin(2x) \neq 2\sin(x)
   $$

3. **Absolute Value Function**  
   $$
   f(x) = |x|
   $$
   **Fails both properties.**

---

## **📌 Why Linearity Matters**
- **Linear Systems** are easier to solve and analyze.
- **Linear Algebra** is built on **vector spaces and transformations**.
- **Machine Learning Models** often assume **linear relationships**.
- **Physics & Engineering** rely on **linear approximations**.

---

## **🔗 Related Topics**
- [[Inner Product]]
- [[Bilinearity]]


---

## **🚀 Summary**
✅ **A function is linear if it satisfies additivity and homogeneity.**  
✅ **Common examples include matrix multiplication, derivatives, and inner products.**  
✅ **Quadratic, trigonometric, and absolute value functions are NOT linear.**  

---

