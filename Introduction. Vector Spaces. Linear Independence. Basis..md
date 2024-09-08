# Material:
- [Lecture](2024_AGLA1_Lecture_1.pdf)
# Body:

**Notation:**
- **Points** are capital italic letter - *A, B...*
- **Scalars** are Greek letters - $\alpha,\beta$.., and sometimes
  Latin letters - a,b..
- **Vectors** are **bold** - **a,b..**, and also $\vec{a},\ \vec{b}$..
- $\mathbb{R}$ is the set of **real** numbers
- $\mathbb{C}$ is the set of **complex** numbers
## Points and Vectors.
- **Vector** is all directed line segments sharing the same direction and length.
- The length of a vector - $|\vec{a}|$ 
- *Unit vector* **u** = $\frac{\vec{V}}{|V|}$
- $\begin{bmatrix}3& 4\end{bmatrix}^{\top} = \begin{bmatrix}3\\4\end{bmatrix}$ 
## Vector Addition. Scalar Vector Multiplication.
## Properties of Vector Arithmetic.
## Vector spaces, Subspaces.
- Vector space $V$ over $\mathbb{R}\ (or \ \mathbb{C})$ is a collection of vectors, together with two operations:
	- $a+b$, addition of two vectors and
	- $\lambda a$, multiplication by scalar ($\lambda \in \mathbb{R}$)
	
- A scalar is a number from $\mathbb{R}\ or\ \mathbb{C}$, respectively.
  
- Addition and multiplication SHOULD satisfy following axioms:
	- Addition:
		1. $a + b = b + a$ (commutativity)
		2. $(a + b) + c = a + (b + c)$ (associativity)
		3. There is a vector $0$ (zero vector) such that $a + 0 = a.$ (identity)
		4. For each vector a, there exists a vector (-a) such that $a + (-a) = 0$ (inverse)
	- Multiplication:
		1. $\lambda(a + b) = \lambda a + \lambda b.$
		2. $(\lambda + \mu)a = \lambda a + \mu a.$
		3. $\lambda(\mu a) = (\lambda\mu)a = \mu(\lambda)a$
		4. $1a = a \ (here \ \lambda = 1).$
- $W$ is a subspace of $V$ if:
	1. $W \subset V$ (subset)
	2. $u,v \in W \Rightarrow u + v \in W$ (closure under addition)
	3. $u \in W,\ \lambda \in \mathbb{R} \Rightarrow \lambda u \in W$ (closure under scalar multiplication)
## Span, Linear Independence.
- Vector $w\in V$ is a linear combination of vectors $v_{1}, ... ,v_{n} \in V \ with \ coefficients\ c_{k}\in \mathbb{R};\ (k = 1..n)$ such that: $$w = c_{1}v_{1}+c_{2}v_{2} +\ ...\ + c_{n}v_{n} = \sum^{n}_{k=1}c_{k}v_{k} $$
- Let $S = \{v_{1},\ v_{2},...,\ v_{n}\}\subset V.$ $$span(S) = \{w\in V : w = \sum^{n}_{k=1}c_{k}v_{k}, \ \forall c_{k} \in \mathbb{R}\}$$
- **Linearly independent vectors** in $\mathbb{R}^{n}$, where $n\in\mathbb{N}$
	- Vectors $v_{1},\ v_{2},...,\ v_{n}$ are *linearly independent* if for $\lambda_{1},\ \lambda_{2},...,\ \lambda_{n}\in\mathbb{R},\ \lambda_{1}v_{1} + \lambda_{2}v_{2} +\ ...\ + \lambda_{n}v_{n} = 0$ if and only if $\lambda_{1}=\lambda_2=...=\lambda_{n}=0.$ 
## Vector Bases and Vector Coordinates in Basis.
- **Basis** of a vector space is a set of vectors that spans a vector space and that is *linearly independent*.
- Let $V$ be a vector space over $\mathbb{R}^{n}$ and let $\{e_{1},...,\ e_{n}\}$ be a basis.
  Then each vector $u$ can be identified with its coordinates $\{u_{1}, ...,\ u_{n}\}$ in the basis. $$u = \sum^{n}_{k=1}u_{k}e_{k}$$$$u = \begin{bmatrix}
  u_{1}\\ 
  u_{2}\\
  ...\\
  u_{n}
  \end{bmatrix}$$
# Assignments:
- Read the topics of lecture: [Аналитическая Геометрия и Линейная Алгебра](Analiticheskaya_geometria_i_lineynaya_algebra_2020_Umnov.pdf)
- Watch the topics of lecture: [Linear Algebra](https://www.3blue1brown.com/topics/linear-algebra)