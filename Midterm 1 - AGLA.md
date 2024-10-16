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
$$\displaylines{\Delta = (2*4*0 + 5*(-2)*(-7) + (-3)* 1 * 3) - \\(-7*4*(-3) + (3*(-2)*2) + 0 * 1 * 5) = \\ (0 + 70 -9) - (84 - 12 + 0) = 61 - 72 = -11}$$
---
#### Find  a vector that is orthogonal to both $v_{1} = (1,0,1)$ and $v_{2}=(1,3,0)$ and which dot product with vector $v_{3} = (1,1,0)$ equals to $8$:

$$\displaylines{\lambda(v_{1}\times v_{2})\cdot v_{3} = 8\\
v_{1}\times v_{2}=\begin{bmatrix}
1 \\ 0 \\ 1
\end{bmatrix} \times \begin{bmatrix}
1 \\ 3 \\0
\end{bmatrix} = det \begin{bmatrix}
i & 1 & 1 \\ j & 0 & 3  \\ k & 1 & 0
\end{bmatrix} = \\
i \begin{bmatrix}
0 & 3  \\  1 & 0
\end{bmatrix} + j \begin{bmatrix}
1&1 \\ 1&0
\end{bmatrix} + k\begin{bmatrix}
1&1 \\ 0&3
\end{bmatrix} = -3i + j + 3k=
\begin{bmatrix}
-3 \\ 1 \\ 3
\end{bmatrix}\\
\lambda(v_{1} \times v_{2})\cdot v_{3} = \lambda\begin{bmatrix}
-3 \\ 1 \\ 3
\end{bmatrix}\cdot \begin{bmatrix}
1 \\ 1 \\ 0 
\end{bmatrix} = \lambda(-3+1+0)=8}$$
$$-2\lambda = 8 \Rightarrow \lambda = -4$$
**Answer:** $\lambda\begin{bmatrix}-3 \\ 1 \\ 3\end{bmatrix} = \begin{bmatrix}12 \\ -4 \\ -12\end{bmatrix}$

### 2. Lines / Planes:

#### Find the angle between the planes $2x - y + z = 6$, $x+y+2z =3$:

We can consider the planes $2x - y +z = 6$ and $x+y+2z = 3$ through a plane that is perpendicular to both of them. From the equations of these planes, we can directly determine the normal vectors.

Each plane can be written in the general form $Ax+By+Cz =D$, where the coefficient $A,\ B$ and $C$ are the components of the normal vector to the plane. These coefficient represents the direction in which the plane is perpendicular to all vectors lying on it.
- For the first plane, the normal vector is $\overline{n}_{1} = \begin{bmatrix}2 \\ -1 \\ 1\end{bmatrix}$
- For the second plane, the normal vector is $\overline{n}_{2} = \begin{bmatrix}1 \\ 1 \\ 2 \end{bmatrix}$
![](Pasted%20image%2020241016210817.png)
In the diagram, the angle between these planes is represented by the angle between their normal vectors. Using the dot product of the normal vectors, we can calculate this angle:
$$cos \theta = \frac{\overline{n}_{1} \cdot \overline{n}_{2}}{|\overline{n}_{1}||\overline{n}_{2}|} = \frac{3}{\sqrt{6}\sqrt{6}} = \frac{1}{2} \Rightarrow \theta = 60^\circ$$

#### What is the general equation of the plane which contains the following two parallel lines: $\frac{x+1}{6} = \frac{y-2}{7} =z$ and $\frac{x-3}{6} = \frac{y-4}{7} = z-1$:

To find the equation of a plane that contains two parallel lines, we need to determine the **normal vector** to the plane. This vector will be **perpendicular** to both parallel vectors. To find this normal vector, we can use the **cross product** of two **linearly independent vectors** that lie in the plane.

1. **Guiding vector:**
   To **guiding vector** of a line, denoted as $\overline{q}$, is the vector that defines the direction of the line in space. According to the canonical representation of a line in space:
   $$\frac{x-x_{0}}{q_{x}} = \frac{y-y_0}{q_{y}} = \frac{z-z_{0}}{q_{z}}$$
   the components of the guiding vector $(q_{x},q_{y},q_{z}$) are the denominators in this equation. In our case, we have the line $\frac{x+1}{6} = \frac{y-2}{7} =z$, and the guiding vector is $\overline{q} = (6,7,1)$.

2. **Choosing a second vector:**
   To find 