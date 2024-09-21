# Bases, orientations. Matrices and determinants.

- **Right hand rule for cross product:**
  ![|360](Pasted%20image%2020240921105221.png)
## Matrices:

- Matrix $A$ is a rectangular table of numbers with $m$ rows and $n$ columns.
  $$A = \begin{bmatrix}
a_{11} & a_{12} & a_{13} \\ 
a_{21} & a_{22} & a_{23} \\
a_{31} & a_{32} & a_{33}
\end{bmatrix} \ \texttt{Example of a 3$\times$3 matrix}$$
$$A = \begin{bmatrix}
a_{11}&a_{12}&a_{13}\\
a_{21}&a_{22}&a_{23}
\end{bmatrix}\ \texttt{Example of a 2$\times$3 matrix}$$

- Different kinds of matrices ($A$ is a $m\times n$ matrix):
	- Square ($m=n$)
	- Rectangular ($m\neq n$)
	- Symmetric matrix ($A^{\top} = A$)
	- (Upper) Triangular matrix ($\forall i,j$ such that $i>j:a_{ij}=0$)
	- Diagonal matrix ($\forall i,j$$\ such that $i\neq j: a_{ij} = 0$)
	- Identity matrix ($IA=AI = A$) $I=\begin{bsmallmatrix}1&0&0\\0&1&0\\0&0&1\end{bsmallmatrix}$ or $I=\begin{bsmallmatrix}1&0\\0&1\end{bsmallmatrix}$
	- Zero matrix ($0+A=A$)
- Operations. Transpose a matrix:
  >[!abstract] Transpose of matrix
  >If $A$ is an $m\times n$ matrix, the transpose $A^{\top}$ is and $n\times m$ matrix defined by $(A^{\top})_{ij}=A_{ji}$.
  >$$\begin{bmatrix}
  >1&4 \\ 2&5 \\ 3&6\end{bmatrix}^\top = \begin{bmatrix} 1&2&3 \\ 4&5&6 \end{bmatrix}$$
  >$$\forall A, (A^\top)^\top = A$$
  
  Vexot