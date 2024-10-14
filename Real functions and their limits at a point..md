# From sequences to functions and their limits in $\mathbb{R}_{\pm\infty}$:

>[!abstract] Sequence limit
>A point $x$ of $\mathbb{R}_{\pm\infty}$ is a limit of a real sequence $(x_{n})_{n\in \mathbb{N}}$ 
>if for any neighborhood $V$ of $x$ for some neighborhood $U$ of $+\infty$ holds $(x_{n})_{n\in \mathbb{N}}(U)\subseteq V$.

>[!abstract] Function limit
>A point $y$ of $\mathbb{R}_{\pm \infty}$ is a limit of a real function $f:D\to \mathbb{R}$ when $x$ tending to $d\in \mathbb{R}_{\pm \infty}$ (notation $\displaystyle y = \lim_{x\to d}f(x)$),
>if for any neighborhood $V$ of $y$ for some neighborhood $U$ of $d$ holds $f(U)\subseteq V$. 

---
# Function limit in reals at real points: from neighborhoods to $\varepsilon\&\delta$ and back:

> [!abstract] Function limit via neighborhoods
> A point $y$ of $\mathbb{R}_{\pm \infty}$ is a limit of a real function $f:D\to \mathbb{R}$ when $x$ tending to $d\in \mathbb{R}_{\pm \infty}$,
> if $D$ is a neighborhood of $d$ and for any neighborhood $V$ of $y$ for some neighborhood $U$ of $d$ holds $f(U)\subseteq V$.

>[!abstract] Function limit via $\varepsilon\&\delta$
>A point $y$ in $\mathbb{R}$ is a limit of a real function $f:D\to \mathbb{R}$ when $x$ tending to $d\in \mathbb{R}$, 
>if for any $\varepsilon>0$ for some $\delta>0$ for every $x$ in support of $f$ 
>	if $|x-d|\leq \delta$ then $|f(x)-y|\leq \varepsilon$. 

---
# Function limit in reals at infinities: from neighborhoods to $\varepsilon \& u$ and back:
---
- A point $y$ in $\mathbb{R}$ is a limit of a real function $f: D \to \mathbb{R}$ when $x$ tending to $\pm \infty$, if 
	- for any $\varepsilon >0$ 
		- for some $u>0$ 
			- for every $x$ in support of $f$ 
				- if $x \frac{\geq}{\leq}\pm u$ then 
				    - $|f(x)-y|\leq \varepsilon$.
- It means that if $f(x)$ approaches $y$ as $x \to+\infty$ or $x \to-\infty$, then for any arbitrary small $\varepsilon>0$ there exists a sufficiently large $u$ such that for all $x$ greater than $u$ (or less than   $-u$, if you're considering $-\infty$) holds the inequality $|f(x) - y|\leq \varepsilon$. 
---
- A point $y$ of $\mathbb{R}_{\pm \infty}$ is a limit of a real function $f:D \to \mathbb{R}$ when $x$ tending to $d \in \mathbb{R}_{\pm \infty}$,
	- if for any neighborhood $V$ of $y$ 
		- for some neighborhood $U$ of $d$ 
			- holds $f(U) \subseteq V$.
- $f(d) = y$  –  Notion.
---
# Function limits in infinities at infinities: from neighborhood to $\displaystyle v \& u$ and back:
---
Let $f: D \to \mathbb{R}$.
- $\displaystyle -\infty = \lim_{x\to \pm \infty}f(x),$
	- if for any $v \in \mathbb{R}$ 
		- for some $u>0$
			-  for every $x$ in support of $f$
				- if $x \frac{\geq}{\leq}\pm u$ then $f(x)\geq v$.
- $\displaystyle +\infty = \lim_{x\to \pm \infty}f(x)$,
	- if for any $v \in \mathbb{R}$
		- for some $u>0$ 
			- for every $x$ in support of $f$
				- if $x \frac{\geq}{\leq}\pm u$ then $f(x) \leq v$.
---
- $\pm \infty$ is a limit of a real function $f: D \to \mathbb{R}$ when $x$ tending to $d \in \mathbb{R}_{\pm \infty}$, 
	- if for any neighborhood $V$ of $\pm \infty$
		-  for some neighborhood $U$ of $d$
			- holds $f(U) \subseteq V$.
----
# Right-side limit in reals at real points: from neighborhood to $\varepsilon \& \delta$ and back:
---
- A point $y$ in $R$ is a right-side limit of a real function $f: D \to \mathbb{R}$ when $x$ tending (from right) to $d \in \mathbb{R}$ (notation $\displaystyle y = \lim_{x \to d+0}f(x)$) if:
	- for any $\varepsilon>0$
		- for some $\delta>0$
			- for every $x$ in support of $f$
				- if $d<x \leq d + \delta$
					- then $|f(x) - y| \leq \varepsilon$.
	- function $f$ with a restricted domain $D\ \cap \ ]d, +\infty[$ has $y$ as a limit when $x$ tending to $d$.
---
# Cardinal sine function $\text{sinc}(x)$:  
---
- Remark that function $\lambda x \in \mathbb{R}.$ $\left( \frac{\sin(x)}{x}\right)$ has a punctured point $x = 0$ where the function is not defined (out of its support) while the function is defined everywhere else.
<br>
- The cardinal sine function $\text{sinc}:\mathbb{R} \to \mathbb{R}$ at a real point $x \in \mathbb{R}$ is defined as 
  $$\text{sinc($x$)} = \begin{cases}1, \text{ if $x = 0$} \\
\frac{sin(x)}{x}, \text{ if $x \neq 0$}\end{cases}$$ 