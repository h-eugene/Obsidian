# Variant 1:
---
## Theory:

1. Vectors $v_{1}, v_{2},...,v_{n}$ are linearly independent if for $\lambda_{1},\ \lambda_{2},...,\ \lambda_{n}\in\mathbb{R},\ \lambda_{1}v_{1} + \lambda_{2}v_{2} +\ ...\ + \lambda_{n}v_{n} = 0$ if and only if $\lambda_{1}=\lambda_2=...=\lambda_{n}=0.$  
2. Condition of coplanarity of three vectors:
   Three vectors are complanar if their scalar triple product is equal to $0$:
   $$\displaylines{a \cdot (b \times c) = 0}$$
3. Trace of a matrix is the sum of all elements on the main diagonal:
   $$Tr(A) = \sum^{m}_{i=1}a_{ii}$$
   
   Trace is linear if it satisfies the following properties:
   
   - **Additivity:** $Tr(A + B) = Tr(A) + Tr(B)$
   - **Homogeneity:** $Tr(c \cdot A) = c \cdot Tr(A)$

   **Additivity:**
   $$Tr(A+B) = \sum^{m}_{i=1}(a_{ii} + b_{ii}) = \sum^{m}_{i=1}a_{ii} + \sum^{m}_{i=1}b_{ii} = Tr(A) + Tr(B)$$
   
   **Homogeneity:**
   $$Tr(c \cdot A) = \sum^{m}_{i=1}(c \cdot a_{ii}) = c \cdot \sum^{m}_{i=1}a_{ii} = c \cdot Tr(A)$$$$Tr(c\cdot A) = \sum^{m}_{i=1}(c \cdot a_{ii}) = c \cdot \sum^{m}_{i=1}a_{ii}$$


## Practice:

### 1. Vector operations / Matrices:

#### Find the determinant of the $3 \times 3$ matrix:
$\begin{bmatrix}2&5&-3 \\ 1& 4 & -2 \\ -7 & 3 & 0\end{bmatrix}$

**Solution:**

$$\displaylines{\Delta = (2*4*0 + 5*(-2)*(-7) + (-3)* 1 * 3) - \\(-7*4*(-3) + (3*(-2)*5))}$$