One important condition for a matrix to be **positive definite** is that all of its **leading principal minors** (determinants of its upper-left submatrices) must be **strictly positive**. 

--- 
## Determinant Condition 
For an $n \times n$ **symmetric** matrix: $$ A = \begin{bmatrix} a_{11} & a_{12} & \dots & a_{1n} \\ a_{12} & a_{22} & \dots & a_{2n} \\ \vdots & \vdots & \ddots & \vdots \\ a_{1n} & a_{2n} & \dots & a_{nn} \end{bmatrix} $$ The **leading principal minors** are the determinants of the **top-left** $k \times k$ submatrices: 
1. **First minor**: $$ D_1 = \det(A_1) = \det \begin{bmatrix} a_{11} \end{bmatrix} > 0 $$ 2. **Second minor**: $$ D_2 = \det(A_2) = \det \begin{bmatrix} a_{11} & a_{12} \\ a_{12} & a_{22} \end{bmatrix} > 0 $$ 3. **Third minor**: $$ D_3 = \det(A_3) = \det \begin{bmatrix} a_{11} & a_{12} & a_{13} \\ a_{12} & a_{22} & a_{23} \\ a_{13} & a_{23} & a_{33} \end{bmatrix} > 0 $$ 4. **Continue up to**: $$ D_n = \det(A) > 0 $$ 
### **Determinant Condition for Positive Definiteness**
A symmetric matrix  A  is **positive definite** if and only if **all leading principal minors are strictly positive**: $$ D_k = \det(A_k) > 0, \quad \forall k = 1, 2, ..., n $$

--- 

## Example: Checking Positive Definiteness Using Determinants 
Consider the matrix: $$ A = \begin{bmatrix} 2 & -1 \\ -1 & 2 \end{bmatrix} $$ 1. **First principal minor**: $$ D_1 = \det \begin{bmatrix} 2 \end{bmatrix} = 2 > 0 $$ 2. **Second principal minor**: $$ D_2 = \det \begin{bmatrix} 2 & -1 \\ -1 & 2 \end{bmatrix} = (2 \times 2) - (-1 \times -1) = 4 - 1 = 3 > 0 $$ Since both determinants are **positive**, \( A \) is **positive definite**. 


--- 
## Python Code to Check Positive Definiteness 
Using Determinants You can check the **determinant condition** using **NumPy**:
```python 

import numpy as np 
def is_positive_definite(A): 
	"""Check if a matrix is positive definite using determinant condition.""" 
	n = A.shape[0] 
	for k in range(1, n + 1): 
		if np.linalg.det(A[:k, :k]) <= 0: 
			return False 
	return True 
	
A = np.array([[2, -1], [-1, 2]]) 
print("Is A positive definite?", is_positive_definite(A))