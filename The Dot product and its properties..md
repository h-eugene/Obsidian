# Material: 
- [Аналитическая Геометрия и Линейная Алгебра](Analiticheskaya_geometria_i_lineynaya_algebra_2020_Umnov.pdf)
- [Slides](2024_AGLA1_Lecture_1.pdf)
# Geometric view (int $\mathbb{R}^{2} \  and \ \mathbb{R}^{3}$):
>[!abstract] Scalar / dot product: 
>$a*b = |a||b|\cos\theta$, where $\theta$ is the angle between $a$ and $b$.
  ![Photo|500](Pasted%20image%2020240903223757.png)
>[!Abstract] Scalar projection of vector $a$ on vector $b$  
>**A scalar:** $a_{b}=\|a\|\cos \theta$ 

>[!abstract] Orthogonal projection of vector $a$ on vector $b$ 
> **A vector:** $a_{b}= \hat{b}\|a\|\cos\theta$ 
  $\hat{b}$ is the *unit vector* in the direction on $b$
  >
  >**Explanation:**
  ![](Introduction.%20Vector%20Spaces.%20Linear%20Independence.%20Basis..md#^cdc541)
  > Orthogonal projection is a Scalar projection but we also add a direction to it using the unit vector of vector $\hat{b}$ 
# Algebraic view:
>[!abstract] Dot product
>Let $V$ be a vector space over $\mathbb{R}$.
>By a *dot product* on $V$ we mean a real valued function $u \cdot v$ on $V \times V \rightarrow \mathbb{R}$ which satisfies the following axioms:
>- $u\cdot v = v \cdot u,\ \forall u, v \in V$
>- $u\cdot (w + v) = u\cdot w + u\cdot v,\ \forall u,v,w\in V$
>- $(\lambda u) \cdot v = \lambda(u\cdot v),\ \forall u,v\in V, \lambda\in\mathbb{R}$
>- $u\cdot u \geq 0,\ \forall u \in V$
>- $u\cdot u = 0 \Leftrightarrow u=0$
>$$u\cdot v = a_{1}b_{1}+...+a_{n}b_{n}=\sum^{N}_{n=1}a_{n}b_{n}$$
>Where $u =\{a_{1},...,a_{n}\}$ and $v=\{b_{1},...,b_{n}\}$

> [!attention] Notation
> $u\cdot = (u,v) = u\ v = \langle u,v \rangle$
# Norm (or a length) of a vector:
> [!abstract] Definition
> We say $\| u \|$ is a norm on a vector space $V$ if $\forall u, v \in V$ and $\alpha\in\mathbb{R}:$
> - $\| \alpha u \| = |\alpha| \|u\|$
> - $\|u\| \geq 0$
> - $\| u \| = 0 \Leftrightarrow u = 0$
> - $\| u+v \| \leq\|u\| + \| v\|$

>[!check] Check
>$u\cdot v = \sum^{n}_{i=1}u_{i}v_{i} = \|u\|\|v\|\cos\theta$
# Cauchy-Schwarz inequality:
> [!abstract] Cauchy-Schwarz inequality
> For all $x,y \in \mathbb{R^{n}},$$$|x\cdot y| \leq \|x\|\|y\|.$$

> [!check] Proof
> Consider the expression $\| x- \lambda y \|^{2}.$ We must have $$\displaylines{\|x-\lambda y\|^{2}\geq 0\\
> (x-\lambda y)\cdot(x - \lambda y)\geq 0\\ 
> \lambda^{2}\|y\|^{2} - \lambda (2x \cdot y) + \|x\|^{2}\geq 0.}$$
> Viewing this as a quadratic in $\lambda$, we see that the quadratic is non-negative. It's possible if the discriminant $\Delta\leq0$, so quadratic cannot have 2 different real roots. $$\displaylines{\Delta = b^{2}-4ac\leq0 \\
> 4(x\cdot y)^{2}\leq 4\|y\|^{2}\|x\|^{2}\\
> (x\cdot y)^{2}\leq \|x\|^{2}\|y\|^{2}\\
> |x\cdot y|\leq\|x\|\|y\|}$$
# Triangle Inequality:
> [!abstract] Triangle inequality
> $\|x+y\|\leq\|x\|+\|y\|.$

>[!check] Proof
>$$\|x+y\|^{2}= (x+y)\cdot(x+y)=\|x\|^{2}+2x\cdot y + \|y\|^{2}$$ $$\leq \|x\|^{2}+2\|x\|\|y\| + \|y\|^{2} = (\|x\|+\|y\|)^{2}$$ 

# Orthogonality
> [!abstract] Definition
> Let $V$ be vector space with a dot product.
> Vectors $u,v\in V$ are said to be **orthogonal** if $$u\cdot v =0$$
# Homework
- Show that the difference between a vector $a$ and its orthogonal projection ($a_{b}$) on a vector $b$ is orthogonal to the vector $b$.
  If $$p=a-a_{b}$$then $$p\cdot b=0$$
  **Solution:**
  $$p = a - a_{b} = a - \hat{b}\|a\|\cos\theta$$
  Substitute the $p$ in another equation: $$\displaylines{
  (a-\hat{b}\|a\|\cos\theta)\cdot b=0 \\
  a\cdot b - b\cdot \hat{b}\|a\|\cos\theta =0 \\
  \|a\|\|b\|\cos \theta - b\cdot \hat{b}\|a\| \cos\theta = 0
  }$$We know that $\hat{b} = \frac{b}{\|b\|} \Leftrightarrow b\cdot \hat{b}=\frac{b\cdot b}{\|b\|}=\frac{\|b\|^{2}}{\|b\|}= \|b\|$, if we substitude it into expression: $$\|a\|\|b\|\cos \theta-\|b\|\|a\|\cos\theta=0$$$\blacksquare$  
- In the triangle ABC the median AD is divided into three equal segments: AE, EF and FD. $$\displaylines{\overline{BA} \cdot \overline{CA}=4\\
   \overline{BF}\cdot\overline{CF}=-1}$$
   Find $\overline{BE}\cdot \overline{CE}$. 
   **Solution:**
   ![Drawing 2024-09-09 23.41.39.excalidraw](Drawing%202024-09-09%2023.41.39.excalidraw.md)
   $$\displaylines{ =\|\overline{FC}\|\|\overline{FB}\|\cos\theta\\
   \overline{AC}-\overline{AB}=\overline{FC}-\overline{FB}\\
   \overline{AC}-\overline{AD}=\overline{AD}-\overline{AB} \Rightarrow \overline{AC}+\overline{AB}=2\overline{AD}\\
   \overline{FC}+\overline{FB}=2\overline{FD}=2\cdot \frac{1}{3}\overline{AD} = \frac{1}{3}(\overline{AC}+\overline{AB})\\
   }$$ $$\displaylines{\begin{cases}3\overline{FC}+3\overline{FB}=\overline{AC}+\overline{AB} \\
\overline{AC}-\overline{AB}=\overline{FC}-\overline{FB}
\end{cases}\Rightarrow \begin{cases}2\overline{AC}=4\overline{FC}+2\overline{FB} \\
2\overline{AB}=2\overline{FC}+4\overline{FB}\end{cases}\Rightarrow\\ \begin{cases}
\overline{AC}=2\overline{FC}+\overline{FB} \\
\overline{AB}=\overline{FC}+2\overline{FB}
\end{cases}}$$
   $$\displaylines{\overline{AC}\cdot \overline{AB} = 4\\}$$