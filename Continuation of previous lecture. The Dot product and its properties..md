#AGLA 
# Material: 
- [Аналитическая Геометрия и Линейная Алгебра](Analiticheskaya_geometria_i_lineynaya_algebra_2020_Umnov.pdf)
- [Slides](2024_AGLA1_Lecture_1.pdf)
# Body:
## Linear dependency / independency. Basis.
### Lemma: 
- For the linear dependency of the vectors $\vec{a_1},\vec{a_2},...\vec{a_n}$ It's sufficient and necessary to have one of them as a linear combination of the others.
**Proof:**
1. **Necessity:** Let $\vec{a_{1}},...,\ \vec{a_{n}}$ - linearly dependent $\Rightarrow \exists$ the set of scalars $\lambda_{1},...,\lambda_{n}$ not equal to 0 simultaneously such that: $$\sum^{n}_{i=1}d_{i}\vec{a}_{i}=0\Leftrightarrow\lambda_{1}\vec{a}_{1}+\ ...\ + \lambda_{n}\vec{a}_{n}=0$$$$\vec{a}_{1}+\frac{\lambda_{2}}{\lambda_{1}} \vec{a}_{2}+\ ...\ +\frac{\lambda_{n}}{\lambda_{n}} \vec{a}_{n} = 0 \Rightarrow \vec{a}_{1}=\sum^{n}_{k=2}(-\frac{\lambda_{k}}{\lambda_{1}}\vec{a}_{k})\ \blacksquare$$
 >Есть ли один из векторов можно представить суммой остальных, то мы можем получить нулевой вектор без тривиального случая. Значит, эти вектора линейно зависимы.
2. **Sufficiency:** Let $\vec{a}_{1}= \sum^{n}_{i=2}\lambda_{i}\vec{a}_{i}$ then $(-1)\vec{a}_{1} + \lambda_{2}\vec{a}_{2} +\ ...\ + \lambda_{n}\vec{a}_{n}=0$, $|-1| + |\lambda_{2}| +\ ...\ + |\lambda_{n}|>0$ - This is a non-trivial case $\rightarrow$ $\vec{a}_{1}+\ ... \ \vec{a}_{n}$ is linearly dependent.
> Не все $\lambda$ равны 0, значит, это не *тривиальный случай*, а если есть другая комбинация для получения 0, то такие векторы линейно зависимы.
> $|\lambda_{1}|+\ ...\ + |\lambda_{n}| > 0$ is the triviality condition.
### Theorem 1:
- Given the basis {$\vec{g_{1}},\ \vec{g_{2}}, \ \vec{g_3}$}, then any vector $\vec{x}$ can be represented by $\vec{x} = \xi_1\vec{g_{1}} + \xi_2\vec{g_{2}}+\xi_3\vec{g_3}$ , where $\xi_{1}, \xi_{2}, \xi_3$ - scalars, moreover - uniquely.
**Proof:** 
  ! 
Let us first **prove the existence** of such numbers.
Let $\vec{x} = \vec{z}+\vec{y}$, then $\vec{z}||\vec{g}_{3}\Rightarrow\vec{z}=\xi_{3}\vec{g}_{3}$
$\vec{y}=\xi_{1}\vec{g}_{1}+\xi_2\vec{g}_{2}$
$\vec{z}+\vec{y}=\xi_{1}\vec{g}_{1}+\xi_2\vec{g}_{2}+\xi_{3}\vec{g}_{3}\ \blacksquare$ 
**Uniqueness:**
Let $\vec{x} = \xi_1\vec{g_1}+\xi_3\vec{g_3}+\xi_3\vec{g_3}$
Assume that there exist $\xi'_{1}\neq\xi_{1}\neq0,\ \xi'_{2}\neq\xi_{2}\neq0,\ \xi'_3\neq\xi_{3}\neq0$: $\vec{x} = \xi'_{1}\vec{g_{1}}+\xi'_{2}\vec{g_{2}}+\xi'_{3}\vec{g_{3}}$
Then, $\vec{x} - \vec{x} = 0 = (\xi_{1} - \xi'_{1})\vec{g_1}+(\xi_{2} - \xi'_{2})\vec{g_2}+(\xi_{3} - \xi'_{3})\vec{g_{3}}$$\Rightarrow |\xi_{1} - \xi'_{1}|+|\xi_{2} - \xi'_{2}|+|\xi_{3} - \xi'_{3}|>0$ - not trivial case, basis vectors are linear dependent. *Contradiction!*
### Task 1: Prove that for any $\vec{a}, \vec{b}, \vec{c}$ and any scalars $\alpha, \beta, \gamma$ the vectors $\alpha\vec{a} - \beta\vec{b}$, $\gamma\vec{b} - \alpha\vec{c}$, $\beta\vec{c} - \gamma\vec{a}$ - linearly dependent.
**Proof:**
$\vec{a}, \vec{b}, \vec{c} - basis \ \ \ \ \ \ \ \ \alpha\vec{a} - \beta\vec{b}$ = $\begin{psmallmatrix}\alpha\\-\beta\\0 \end{psmallmatrix}$
$\gamma\vec{b} - \alpha\vec{c} = \begin{psmallmatrix}0\\ \gamma\\-\alpha\end{psmallmatrix} \ \ \ \ \ \ \ \ \beta\vec{c} - \gamma\vec{a} = \begin{psmallmatrix}-\gamma \\ 0 \\ \beta\end{psmallmatrix}$ 
We need to prove that there exist u, v, w:
$u \begin{psmallmatrix}0\\\gamma\\-\alpha\end{psmallmatrix} + v\begin{psmallmatrix}\alpha\\-\beta\\0\end{psmallmatrix} + w\begin{psmallmatrix}-\gamma\\0\\\beta\end{psmallmatrix} = 0 = \begin{psmallmatrix}0\\0\\0\end{psmallmatrix}$
$$\begin{cases}\alpha v - \gamma w = 0  \rightarrow  \alpha v = \gamma w  ,\ v = \frac{\gamma}{\alpha}w \\
u\gamma - \beta b = 0 \rightarrow u\gamma = \beta v = \beta*\frac{\gamma}{\alpha}w \rightarrow u = \frac{\beta}{\alpha}w \\
-\alpha u + \beta w = 0 \rightarrow -\alpha*\frac{\beta}{\alpha}w + \beta w = 0 
\end{cases}$$
$\blacksquare$
**Task 2: Check that $\vec{a}(-5,-1),\ \vec{b}(-1,3)$ form a basis in the plane. Find the coordinates of $\vec{e}(-1,2), \ \vec{l}(2,-6)$(homework) in this basis.**
1. Check the collinearity: $\vec{a} = k\vec{b}$
$\begin{pmatrix}-5\\-1\end{pmatrix}= {\begin{pmatrix}-1*k\\3*k\end{pmatrix}}\Rightarrow \nexists \ k \Rightarrow basis$. 
2. $\vec{e} = \alpha\vec{a} +\beta\vec{b}\Leftrightarrow \begin{pmatrix}-1\\2\end{pmatrix} = \alpha\begin{pmatrix}-5\\-1\end{pmatrix}+\beta{\begin{pmatrix}-1\\3\end{pmatrix}}$ 
   ${\begin{cases}-5\alpha-\beta=-1\\-\alpha+3\beta=2\end{cases}}$ $\Rightarrow \beta=\frac{11}{16}; \ \alpha=\frac{1}{16}$ 
3. $\vec{l}=\lambda\vec{a}+\beta\vec{b}\Leftrightarrow{\begin{pmatrix}2\\-6\end{pmatrix}}= \alpha\begin{pmatrix}-5\\-1\end{pmatrix}+\beta{\begin{pmatrix}-1\\3\end{pmatrix}}$ 
   $\begin{cases}-5\alpha-\beta=2\\-\alpha+3\beta=-6\end{cases}$ $\Rightarrow \alpha=0; \ \beta=-2$  
## Dot product.
### Geometric view (int $\mathbb{R}^{2} \  and \ \mathbb{R}^{3}$):
- Scalar | dot product: $a*b = |a||b|\cos\theta$, where $\theta$ is the angle between $a$ and $b$.
  ![Photo|500](Pasted%20image%2020240903223757.png)
