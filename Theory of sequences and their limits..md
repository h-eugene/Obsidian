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

# Sequences and their limits

- A sequence converges to a real number $x\in \mathbb{R}$, if the sequences has $x$ as a limit.
- A sequences converges (or has a limit), if it has a limit (i.e, there exists $x$ such that ..).
- A sequences $(x_{n})_{x\in \mathbb{N}}$ is bounded, if for some interval $[a,b]\subseteq\mathbb{R}$ and each (all) $n \in \mathbb{N}$ holds $x_{n}\in [a,b]$. 
>[!hint] Examples and exercises
>- Sequences $(1- \frac{1}{n+1})_{n\in\mathbb{N}}$ and $((-1)^{n} - \frac{1}{n+1})$ are bounded.

# Subsequences:

- A sequence $(y_{n})_{n\in \mathbb{N}}$ is said to be a subsequence of a sequence $(x_{n})_{x\in \mathbb{N}}$, if there exists a strictly monotone (strictly increasing / growing) total ("sub-indexing") function $m: \mathbb{N}\to\righ\mathbb{N}$ 