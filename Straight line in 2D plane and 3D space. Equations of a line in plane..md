# Review:
---
>[!abstract] Locus
>"When a point moves so as to satisfy some geometrical condition or conditions, the path traced out by the point is called the **locus** of the point."
>
>**Example:**
>- Suppose a point $P(x,y)$ moves such that its distances from two fixed points $A(2,3)$ and $B(5,-3)$ are equal. Then the geometrical law is lengths $PA = PB$ hence hence $PA^{2}= PB^{2}$
>  $$(x-2)^{2} + (y-3)^{2} = (x-5)^{2}+ (y+3)^{2} \Rightarrow$$
>  $$2x - 4y - 7 = 0 - \text{locus is a straight line}$$

---
# Straight line in plane:
---
## Parametric Vector Equation:

![](Pasted%20image%2020241009095851.png)

**Equation:** $r - r_{0} = tq$, where $t$ is a parameter.

---
## Parametric Equation in 3D:

>[!note] In *rectangular Cartesian coordinate system*
>$$\text{Equation of a line: }\begin{cases} 
 x = x_{0} + q_{x}t \\
 y= y_{0} + q_{y}t  \\
 z = z_{0} + q_{z}t 
\end{cases}$$

$$r - r_{0} = [x-x_{0}, y-y_{0}, z-z_{0}]^\top$$
$$q = [q_{x},q_{y},q_{z}]^\top$$
---
## Canonical equation of a line:

Eliminating $t$ from the system:
$\begin{cases} x = x_{0} + q_{x}t\\ y = y_{0} + q_{y}t \\ z = z_{0} + q_{z}t\end{cases}$

>[!note] we get the *Canonical equation*
>$$\frac{x-x_{0}}{q_{x}}$$