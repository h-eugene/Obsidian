# Material: 

- [2024_AGLA1_Lecture_4](2024_AGLA1_Lecture_4.pdf)

# Change of basis and coordinates:
---
**Notations:**
- $(O, \overline{e}_{1},\overline{e}_{2},\overline{e}_{3})$ – is coordinates system ($\overline{e}_{1},\overline{e}_{2},\overline{e}_{3}$ - basis).
- $\overline{v} = x_{1}\overline{e}_{1}+x_{2}\overline{e}_{2}+x_{3}\overline{e}_{3} = \begin{bsmallmatrix}x_{1}\\ x_{2}\\ x_{3}\end{bsmallmatrix}$
---
Let $(O, \overline{e}_{1},\overline{e}_{2},\overline{e}_{3})$ is old coordinates system, and $(O', \overline{e'}_{1},\overline{e'}_{2},\overline{e'}_{3})$ is new coordinates system.
N – is arbitrary point in space.
Then,

![|600](Pasted%20image%2020240923093732.png)
$$\displaylines{ON = OO'+O'N \\
ON = x_{1}e_{1}+x_{2}e_{2}+x_{3}e_{3}\\
O'N = x_{1}'e_{1}'+x_{2}'e_{2}'+x_{3}'e_{3}'\\
OO' = b_{1}e_{1}+b_{2}e_{2}+b_{3}e_{3}
}$$
We can express the new basis through the old one.
$$\displaylines{
e_{1}' = \alpha_{11}e_{1} + \alpha_{21}e_{2}+\alpha_{31}e_{3}\\
e_{1}' = \alpha_{12}e_{1} + \alpha_{22}e_{2}+\alpha_{32}e_{3}\\
e_{1}' = \alpha_{13}e_{1} + \alpha_{23}e_{2}+\alpha_{33}e_{3}}$$
Hence, we will get the transition matrix [^1]
$$A=\begin{bmatrix}
\alpha_{11}&\alpha_{12}&\alpha_{13}\\ \alpha_{21}&\alpha_{22}&\alpha_{23}\\ 
\alpha_{31}&\alpha_{32}&\alpha_{33}\\
\end{bmatrix}$$
Next, we substitute all of we got to initial expression.
$$\displaylines{ON = OO'+O'N = \\b_{1}e_{1}+b_{2}e_{2}+b_{3}e_{3} + \\ x_{1}'(\alpha_{11}e_{1} + \alpha_{21}e_{2}+\alpha_{31}e_{3})+\\
x_{2}'(\alpha_{12}e_{1} + \alpha_{22}e_{2}+\alpha_{32}e_{3} + \\
x_{3}'(\alpha_{13}e_{1} + \alpha_{23}e_{2}+\alpha_{33}e_{3}) =\\
(b_{1}+ x_{1}' \alpha_{11}+x_{2}'\alpha_{12}+x_{3}'\alpha_{13})e_{1}+\\
(b_{2}+ x_{1}' \alpha_{21}+x_{2}'\alpha_{22}+x_{3}'\alpha_{23})e_{2}+\\
(b_{3}+ x_{1}' \alpha_{31}+x_{2}'\alpha_{32}+x_{3}'\alpha_{33})e_{3}
}$$
This expression can be represented by the transition matrix:
$$\displaylines{
\begin{bmatrix}
x_{1} \\ x_{2} \\ x_{3}
\end{bmatrix} = \begin{bmatrix}
b_{1} \\ b_{2}\\b_{3}
\end{bmatrix} + \begin{bmatrix}
\alpha_{11}&\alpha_{12}&\alpha_{13}\\ \alpha_{21}&\alpha_{22}&\alpha_{23}\\ 
\alpha_{31}&\alpha_{32}&\alpha_{33}\\
\end{bmatrix} \begin{bmatrix}
x_{1}' \\ x_{2}' \\ x_{3}'
\end{bmatrix} \\ x = b + Ax'
}$$
# Matrix rotating:

- Let $v$ be a vector with coordinates $\begin{bmatrix}x\\y\end{bmatrix}$.
- Let $v'$ be the vector with new coordinates $\begin{bmatrix}x'\\y'\end{bmatrix}$ obtained by rotating $v$ by angle an $\theta$.

![|400](Pasted%20image%2020240923102734.png)

-  The new coordinates $\begin{bmatrix}x'\\y'\end{bmatrix}$ can be found using the following matrix:
$$\displaylines{
\begin{bmatrix}
x' \\ y'
\end{bmatrix} = R(\theta)\begin{bmatrix}
x \\ y
\end{bmatrix} = \begin{bmatrix}
\cos\theta & -\sin\theta \\ \sin\theta & \cos\theta 
\end{bmatrix}\begin{bmatrix}
x \\ y
\end{bmatrix}
}$$
# Matrix Inverses:

> [!abstract] Definition
> Matrix $B$ is called inverse of a square matrix $A$ if
> $$AB = BA = I$$
> **Notation:** 
> - $B=A^{-1}$
> - $AA^{-1}= A^{-1}A = I$
> **Example:**
> ![](Pasted%20image%2020240923105422.png)

> [!abstract] Left inverse
> Consider an $m\times n$ matrix $A$ and $n\times m$ matrix $B$. 
> If $BA = I$, then we say $B$ is the **left inverse** of $A$.

>[!abstract] Right inverse 
>Consider an $m\times n$ matrix $A$ and $n\times m$ matrix $C$.
>If $AC = I$, then we say $C$ is the **right inverse** of $A$.

- If $A$ has an inverse, then $A$ is **invertible** (== nonsingular).
- If $A$ and $B$ are invertible and $AB$ is invertible, then
  $$(AB)^{-1}=B^{-1}A^{-1}$$
## Ways to find the inverse matrix:

> [!example]  Minor Method (using cofactors)
> 1. Find the determinant of matrix $A$.
> 2. Find the minors:
> 	- **Minor** is the determinant of the smaller matrix you get by deleting the row and column of that element.
> 	- For each element of the matrix, you find a **minor** and write it to another matrix in the appropriate position. 
> 3. Find cofactors:
>	- For each element of the obtained matrix we apply a sign pattern: $(-1)^{i+j}$, where $i$ and $j$ are the row and column numbers of the element.
>	- This gives you the cofactor matrix.
>4. Transpose[^2] the cofactor matrix.
>5. Find the inverse:
>	- $A^{-1} = \frac{1}{det(A)}\times \texttt{(Transposed cofactor matrix)}$.

> [!example] Gauss-Jordan Method
> 1. Set up an augmented matrix.
> 	- You take your matrix $A$ and put it next to identity matrix[^3] $I$



[^1]: Matrix that converts coordinates from one basis to another
[^2]: Transpose is flipping rows and columns.
[^3]: Matrix which has 1's on the diagonal and 0's everywhere else $\begin{bsmallmatrix}1&0\\\end{bsmallmatrix}$ 