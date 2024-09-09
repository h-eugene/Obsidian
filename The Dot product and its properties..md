# Material: 
- [Аналитическая Геометрия и Линейная Алгебра](Analiticheskaya_geometria_i_lineynaya_algebra_2020_Umnov.pdf)
- [Slides](2024_AGLA1_Lecture_1.pdf)
# Geometric view (int $\mathbb{R}^{2} \  and \ \mathbb{R}^{3}$):
>[!abstract] Scalar / dot product: 
>$a*b = |a||b|\cos\theta$, where $\theta$ is the angle between $a$ and $b$.
  ![Photo|500](Pasted%20image%2020240903223757.png)
> **Explanation:**
> It's just areas of parallelogramm that appears when we move each vector

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

> [!todo] ff
# Triangle Inequality:
