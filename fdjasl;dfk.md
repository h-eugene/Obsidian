# Change of basis and coordinates:

- $(O, \overline{e}_{1},\overline{e}_{2},\overline{e}_{3})$ – is coordinates system ($\overline{e}_{1},\overline{e}_{2},\overline{e}_{3}$ - basis).
- $\overline{v} = x_{1}\overline{e}_{1}+x_{2}\overline{e}_{2}+x_{3}\overline{e}_{3} = \begin{bsmallmatrix}x_{1}\\ x_{2}\\ x_{3}\end{bsmallmatrix}$

![|600](Pasted%20image%2020240923093732.png)
$$\displaylines{ON = OO'+O'N \\
ON = x_{1}e_{1}+x_{2}e_{2}+x_{3}e_{3}\\
O'N = x_{1}'e_{1}'+x_{2}'e_{2}'+x_{3}'e_{3}'\\
OO' = b_{1}e_{1}+b_{2}e_{2}+b_{3}e_{3}
}$$
$$\displaylines{
e_{1}' = \alpha_{11}e_{1} + \alpha_{21}e_{2}+\alpha_{31}e_{3}\\
e_{1}' = \alpha_{12}e_{1} + \alpha_{22}e_{2}+\alpha_{32}e_{3}\\
e_{1}' = \alpha_{13}e_{1} + \alpha_{23}e_{2}+\alpha_{33}e_{3}\\ \\
A=\begin{bmatrix}
\alpha_{11}&\alpha_{12}&\alpha_{13}\\ \alpha_{21}&\alpha_{22}&\alpha_{23}\\ 
\alpha_{31}&\alpha_{32}&\alpha_{33}\\
\end{bmatrix}
-\texttt{the transition matrix}} $$
$$\displaylines{ON = b_{1}e_{1}+b_{2}e_{2}+b_{3}e_{3} + \\ x_{1}'(\alpha_{11}e_{1} + \alpha_{21}e_{2}+\alpha_{31}e_{3})+\\
x_{2}'(\alpha_{12}e_{1} + \alpha_{22}e_{2}+\alpha_{32}e_{3} + \\
x_{3}'(\alpha_{13}e_{1} + \alpha_{23}e_{2}+\alpha_{33}e_{3}) =\\
(b_{1}+ x_{1}' \alpha_{11}+x_{2}'\alpha_{12}+x_{3}'\alpha_{13})e_{1}+\\
(b_{2}+ x_{1}' \alpha_{21}+x_{2}'\alpha_{22}+x_{3}'\alpha_{23})e_{2}+\\
(b_{3}+ x_{1}' \alpha_{31}+x_{2}'\alpha_{32}+x_{3}'\alpha_{33})e_{3}
}$$

$$\displaylines{
\begin{bmatrix}
x_{1} \\ x_{2} \\ x_{3}
\end{bmatrix} = \begin{bmatrix}
b_{1} \\ b_{2}\\b_{3}
\end{bmatrix} + \begin{bmatrix}
\alpha_{11}&\alpha_{12}&\alpha_{13}\\ \alpha_{21}&\alpha_{22}&\alpha_{23}\\ 
\alpha_{31}&\alpha_{32}&\alpha_{33}\\
\end{bmatrix} \begin{bmatrix}
x_{1}' \\ x_{2}' \\ x_{3}'
\end{bmatrix} \\ x = b + Ax1
}$$
