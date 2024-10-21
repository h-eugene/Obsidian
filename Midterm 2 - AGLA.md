# Theory:

## 1. Definition, simple proofs:

### Let $V = \{v_{1},v_{2},...,v_{n}\}$ be a set of vectors. Give a definition of a span $S(V)$:

The **span** of a set of vectors $S = \{v_{1},v_{2},...,v_{n}\} \subseteq V$ is the set of all possible linear combinations of the vectors in $S$:
$$\text{span}(S) = \left\{w \in V:w=\sum^{n}_{k=1}c_{k},v_{k},\ \forall c_{k} \in \mathbb{R}\right\}.$$
In this context, any vector $w \in \text{span}(S)$ can ve expressed as a linear combination of the vectors $v_{1},v_{2},...,v_{n}$, where the coefficients $c_{k}$ are real numbers.

---
### What is the geometrical interpretation of the magnitude of $a \times b$?

The magnitude of the cross product $|a \times b|$ represents two things geometrically:

1. The area of the parallelogramm spanned by vectors $a$ and $b$: $|a||b||\sin \theta|$
2. The length of the vector that is perpendicular to both $a$ and $b$, as $a \times b$ itself is a vector that is orthogonal to both $a$ and $b$.

So, $|a \times b|$ gives the length of the vector normal to the plane defined by $a$ and $b$, and this length corresponds to the area of the parallelogram.

---
### Given that $BC$ and $CB$ are valid, prove that $Tr(BC) = Tr(CB)$:

1.  **Definition of Trace:** The trace of a matrix is the sum of its diagonal elements. For any $n \times n$ matrix $A$, we have:$$Tr(A) = \sum^{n}_{i=1}A_{ii}$$where $A_{ii}$ represents the $i$-th diagonal element of matrix $A$.
2. **Trace of a Product:** Let $B$ and $C$ be two $n \times n$ matrices such that both $BC$ and $CB$ are valid matrix multiplication.
   
   The $(i,i)$-th element of the matrix $BC$ is: $$(BC)_{ii} = \sum^{n}_{j=1}B_{ij}C_{ji}$$Therefore, the trace of $BC$ is:$$Tr(BC) = \sum^{n}_{i=1}(BC)_{ii} = \sum^{n}_{i=1}\sum^{n}_{j=1}B_{ij}C_{ji}$$
3. **Symmetry:** Now, consider the matrix $CB$. The $(i,i)$-th element of the matrix $CB$ is:$$(CB)_{ii} = \sum^{n}_{j=1}C_{ij}B_{ji}$$So the trace of $CB$ is:$$Tr(CB) = \sum^{n}_{i=1}(CB)_{ii} = \sum^{n}_{i=1}\sum^{n}_{j=1}C_{ij}B_{ji}$$
4. **Interchanging the Summation Using Commutativity:** Notice that in both expression $\sum^{n}_{i=1}\sum^{n}_{j=1}B_{ij}C_{ji}$ and $\sum^{n}_{i=1}\sum^{n}_{j=1}C_{ij}B_{ji}$, we are multiplying two scalars: $B_{ij}$ and $C_{ji}$ in one case, and $C_{ij}$ and $B_{ji}$ in the other. Since scalar multiplication is **commutative**, we have:$$B_{ij}C_{ji} = C_{ji}B_{ij}$$Therefore, the terms in both summations are identical, meaning:$$\sum^{n}_{i=1}\sum^{n}_{j=1}B_{ij}C_{ji}=\sum^{n}_{i=1}\sum^{n}_{j=1}C_{ji}B_{ij}=\sum^{n}_{i=1}\sum^{n}_{j=1}C_{ij}B_{ji}$$
5. **Conclusion:** Since the two summations are equal, it follows that:$$Tr(BC) = Tr(CB).$$
---
# Practice:

## 1. Vector operations / Matrices:

### Find the determinant of matrix:$\begin{bmatrix}1&-2&2\\2&1&-1\\4&-3&5\end{bmatrix}$

$$\begin{vmatrix}1&-2&2\\2&1&-1\\4&-3&5\end{vmatrix} = 2 + 2*14 -2*10 = 10$$
---
### Find a vector that is orthogonal to both $v_{1} = (1,-1,1)$ and $v_{2} = (6,-3,0)$ and which dot product with a vector $v_{3}= (3,2,3)$ equals to 10:

**First Solution:**

Find the orthogonal vector $q$ to both $v_1$ and $v_{2}$ using cross product:
$$v_{1}\times v_{2} = \begin{vmatrix}
i & j&k \\ 1&-1&1 \\ 6&-3&0
\end{vmatrix} = 3i+6j+3k = \begin{bmatrix}
3 \\ 6 \\ 3
\end{bmatrix}$$
We know that dot product of collinear vector to $q$ and $v_{3}$ is 10:
$$\lambda q \cdot v_{3} = 10$$
Let us define $\lambda$:
$$3\lambda *3 + 6\lambda*2 +3\lambda * 3 = 10$$
$$\lambda = \frac{1}{3} \Rightarrow \text{Answer:} \begin{bmatrix}
1 \\ 2 \\ 3
\end{bmatrix}$$
**Second Solution:**

Let the vector that we want to find be $q = (x,y,z)$, then, since it is orthogonal to both $v_{1}$ and $v_{2}$, we can conclude: $q \cdot v_{1} = 0$ and $q \cdot v_{2} = 0$

Also, we know that $q \cdot v_{3} = 10$, so we have the system of equations:
$$\begin{cases}
q \cdot v_{1}= x - y + z =0 \\

\end{cases}$$