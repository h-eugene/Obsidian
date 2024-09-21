# Bases, orientations. Matrices and determinants.

- **Right hand rule for cross product:**
  ![|360](Pasted%20image%2020240921105221.png) ^3f1278
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

  
# Vector Cross Product:

>[!info] 
$$a\times b= \hat{n}\|a\|\|b\|\sin\theta \ | \ a,b\in \mathbb{R}^3,\ \hat{n}\perp a,b$$
>- A $\hat{n}$ is directed by a [right-hand rule](Matrix%20Operations%20and%20Vector%20Cross%20Product..md#^3f1278).
>- Vector cross product defined only for 3-dimensional vectors!!!
>**Geometric view:**
>![|300](Pasted%20image%2020240921113341.png)

## Properties:

- $a\times b = -b \times a$.
- $a\times a = 0$.
- $a\times b = 0 \Rightarrow a=\lambda b$ for some $\lambda\in\mathbb{R}$ (or $b=0$).
- $a\times (\lambda b) = \lambda(a\times b)$.
- $a\times (b+c)=a\times b + a\times c$.

## Calculating:
$$\displaylines{a\begin{pmatrix}a_1\\ a_2\\ a_3 \end{pmatrix}\times b\begin{pmatrix}b_1\\ b_2\\ b_3 \end{pmatrix}=\\
=(a_2b_3-a_3b_2)\hat{i}-(a_1b_3-a_3b_1)\hat{j}+(a_1b_2-a_2b_1)\hat{k}\\
=(a_2b_3-a_3b_2)\hat{i}+(a_3b_1-a_1b_3)\hat{j}+(a_1b_2-a_2b_1)\hat{k}}$$
There are more convenient ways to calculate vector cross products.

**Interpretation:** 
$-a\times b = b\times a$
![|200](Pasted%20image%2020240921115145.png)

# Scalar Triple Product:

![|500](Pasted%20image%2020240921115510.png)
![|500](Pasted%20image%2020240921115532.png)

>[!abstract] Scalar Triple Product.
>$$a\cdot (b\times c)$$
>$$a\cdot(b\times c)=(a\times b)\cdot c$$
>**Meaning:** $V=\|a\times b\|(\|c\||\cos(\phi)|)$ = Area of base * Height 

# Matrix multiplication:
 ![](Pasted%20image%2020240921115853.png)

>[!abstract] Definition
>- Let 
  $A$ be $m\times n$ matrix;
  $B$ be $n\times p$ matrix
  Then exists $C=AB$,
  $C$ must be $m\times p$ matrix
  $$\displaylines{c_{ij} = a_{i1}b_{1j} + a_{i2}b_{2j}+...+a_{in}b_{nj} = \sum_{k=1}^{n} a_{ik}b{kj},\\\texttt{for $i=1,..,m$ and $j=1,..,p$}}$$
  >![multiplication of matrices|1000](multiplication%20of%20matrices.md)
  >- Commit into your memory: **matrix multiplication is not commutative.**
  >  $$AB\neq BA$$
  >- **Check sizes of the two matrices:**
  >  if you multiply $AB\ (m\times n)(k\times p)$, then check that $n=k$
  >- **Calculate the size** of the result:
  >  if you multiply $AB\ (m\times n)(k\times p)$, then the result is a $m\times p$ matrix.

- **Order of operations after transposition:**
  $(ABDC)^\top = D^\top C^\top B^\top A^\top$

- **Matrix vector multiplication:**
  $x$ is a **column** vector
  $Ax = (m\times n)(n\times 1)\to (m\times 1)$ is a **column** vector
  $x^{\top}A = (1\times m)(m\times n)\to (1\times n)$ is a **row** vector
# Homework:

## Task 1: $det(A) = det(A^{\top})$

Let 
$A=\begin{bmatrix}a_{11}&a_{12}&...&a_{1n}\\a_{21}&a_{22}&...&a_{2n}\\...&...&...&...\\ a_{m1}&a_{m2}&...&a_{mn}\end{bmatrix},$ then 
$A^{\top} = \begin{bmatrix}a_{11}&a_{21}&...&a_{m1}\\a_{12}&a_{22}&...&a_{m2}\\...\end{bmatrix}$ 
$$\displaylines{det(A)=}$$




