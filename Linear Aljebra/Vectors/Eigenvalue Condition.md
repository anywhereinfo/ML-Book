## Definition
The **Eigenvalue Condition** states that all eigenvalues $\lambda_i$ of a square matrix A must be **strictly positive**:
$$\lambda_i > 0, \quad \forall i$$
## Importance

### **1️⃣ Positive Definiteness** 
A matrix \( A \) is **positive definite** if: $$ x^T A x > 0, \quad \forall x \neq 0$$ This property ensures: 
- The matrix represents a **valid inner product**. 
- It defines a meaningful **distance metric** in geometry and ML. 

### **2️⃣ Stability in Systems** 
In **dynamical systems**, if a system matrix has **only positive eigenvalues**, it implies **stability**. 
### **3️⃣ Optimization Applications** 
- The **Hessian matrix** in second-order optimization must be **positive definite** for a function to have a unique local minimum. 

- Used in **Newton's method** for optimization. 

### **4️⃣ Machine Learning & Statistics** 
- **Covariance matrices** in statistics and ML must be **positive semi-definite**. 
- **Gradient descent** methods behave better when the Hessian is positive definite. 

--- 
## Example: Eigenvalues and Positive Definiteness 
Consider the matrix: $$ A = \begin{bmatrix} 2 & -1 \\ -1 & 2 \end{bmatrix} $$ **Step 1: Compute Eigenvalues** 
Solve $\det(A - \lambda I) = 0$: $$ \begin{vmatrix} 2 - \lambda & -1 \\ -1 & 2 - \lambda \end{vmatrix} = 0 $$ Expanding: $$ (2-\lambda)(2-\lambda) - (-1)(-1) = 0 $$ $$ \lambda^2 - 4\lambda + 3 = 0 $$ $$ (\lambda - 3)(\lambda - 1) = 0 $$ So the eigenvalues are: $$ \lambda_1 = 3, \quad \lambda_2 = 1 $$ Since **both eigenvalues are strictly positive**, \( A \) is **positive definite**. 

--- 
## Checking Positive Definiteness in Python 
You can use **NumPy** to check if a matrix is positive definite:
```python 
import numpy as np 
A = np.array([[2, -1], [-1, 2]]) 

# Compute eigenvalues 
eigenvalues = np.linalg.eigvals(A) 

# Check if all eigenvalues are positive 
is_positive_definite = np.all(eigenvalues > 0) 

print("Eigenvalues:", eigenvalues) 
print("Is A positive definite?", is_positive_definite)
```


## Summary

✅ **If all eigenvalues $\lambda_i > 0$, then A is positive definite**.  
✅ **Used in stability analysis, optimization, and machine learning**.  
✅ **Eigenvalues can be computed using NumPy or algebraic methods**.