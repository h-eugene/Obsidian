# Sequences and their limits:
- A (real) sequences is a total function $(x_{n})_{n\in N}:\ \mathbb{N}\rightarrow\mathbb{R}$ usually presented as $x_{0}, x_{1},x_{2},...$
- A real number $x\in \mathbb{R}$ is said to be a limit of a sequences $(x_{n})_{n\in N}$, (notation $x=\lim_{x\to\infty} x_{n}$) if
	- for each (any) real $\epsilon>0$ 
		- for some (i.e., there exists) $m\in \mathbb{N}$ such that 
			- for all $n\geq m$ holds $|x_{m}-x_{n}|\leq \epsilon$.

> [!hint] Examples and exercises
> - Examples:
> 	- Sequence $(1- \frac{1}{n+1})_{n\in \mathbb{N}}$ has a limit $1$.
> 	- Sequence $((-1)^{n} - \frac{1}{n+1})_{n\in\mathbb{N}}$ has no any limit.

- A sequence converges to a real number $x\in \mathbb{R}$, if the sequences has $x$ as a limit.
- A sequences converges (or has a limit), if it has a limit (i.e, there exists $x$ such that ..).
- A sequences $(x_{n})_{x\in \mathbb{N}}$ is bounded, if for some interval $[a,b]\subseteq\mathbb{R}$ and each (all) $n \in \mathbb{N}$ holds $x_{n}\in [a,b]$. 

>[!hint] Examples and exercises
>- Sequences $(1- \frac{1}{n+1})_{n\in\mathbb{N}}$ and $((-1)^{n} - \frac{1}{n+1})$ are bounded.

# Subsequences:

- A sequence $(y_{n})_{n\in \mathbb{N}}$ is said to be a subsequence of a sequence $(x_{n})_{x\in \mathbb{N}}$, if there exists a strictly monotone (strictly increasing / growing) total ("sub-indexing") function $m: \mathbb{N}\to\mathbb{N}$ such that for all $n\in\mathbb{N}$ holds $y_{n}=x_{m(n)}$.
- Example: Sequence $0,2,4,...$ of even numbers is a subsequence of all natural numbers $0,1,2,...$ but not vice-versa, a sub-indexing function is $m=\lambda m \in \mathbb{N}.(2n)$.
- Subsequence of a converging sequence does converge to the same limit as the sequence itself.

# Main properties: convergence and boundness:

- Each converging sequence (a) has unique limit and (b) is bounded.
  
  >[!check] Proof a
  >- Let $y$ and $z$ be limits(s) of a sequence $(x_{n})_n\in\mathbb{N}$.
  >- Let $\epsilon>0$ be any positive real number and $m_{y}\in \mathbb{N}$ and $m_{z}\in \mathbb{N}$ be numbers such that
  >	- $|x_{n}-y|\leq \epsilon$ for all $n\geq m_{z}$,
  >	- $|$
- (Bolzano – Weierstrass theorem) Each bounded sequence has a converging subsequence (but not vice versa)