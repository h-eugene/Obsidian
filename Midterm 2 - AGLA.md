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
   
   The $(i,i)$-th element of the matrix $BC$ is:   $$(BC)_{ii} = \sum^{n}_{j=1}B_{ij}C_{ji}$$Therefore, the trace of $BC$ is:$$Tr(BC) = $$

