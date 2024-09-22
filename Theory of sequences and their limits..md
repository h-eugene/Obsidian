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

- Each converging sequence has unique limit and is bounded.
   
**Proof for unique limit:**

- Let $y$ and $z$ be limits(s) of a sequence $(x_{n})_n\in\mathbb{N}$
- Let $\epsilon>0$ be any positive real number and $m_{y}\in \mathbb{N}$ and $m_{z}\in \mathbb{N}$ be numbers such that
- $|x_{n}-y|\leq \epsilon$ for all $n\geq m_{y}$,
- $|x_{n}-z|\leq \epsilon$ for all $n\geq m_{z}$,
- and let $m=max\{m_{y},m_{z}\}$.   [^1].
- Then $$\displaylines{|y-z|=|(y-x_{m})+(x_{m}-z)|\leq\\ |y-x_{m}|+|x_{m}-z|\leq 2\epsilon}.$$![Trianle inequality|200](The%20Dot%20product%20and%20its%20properties..md#^73428c)
- Hence $y=z$ because the distance between $y$ and $z$ is less than any positive number. $\blacksquare$
 
  >[!check]+ Proof for bounded
  >- Let $(x_{n})_n\in\mathbb{N}$ be a sequence and $x$ be its limit.
  >- Let $m\in\mathbb{N}$ be a number such that for all $n\geq m$ holds $|x_{n}-x|\leq 1$.
  >- Let $c=max\{|x_{0}|,...|x_{m}|, |x-1|,|x+1|\}$.     [^2].
  >- Then for all $n\in\mathbb{N}$ holds $-c\leq x_{n}\leq +c,$ i.e., 
  >  $(x_{n})_n\in\mathbb{N}$ is bounded. $\blacksquare$
  
- (Bolzano – Weierstrass theorem) Each bounded sequence has a converging subsequence (but not vice versa)


[^1]: m is a number at which both of the above equalities work. The equalities will work if we take their intersection, in this case it is the maximum of these values
[^2]: c is a value that is larger or equal to the max element of sequence.  