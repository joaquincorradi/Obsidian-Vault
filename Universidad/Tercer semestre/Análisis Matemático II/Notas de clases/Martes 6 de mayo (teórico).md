# Integrales triples
Orden de integración
- Tipo $1$: $z,y,x$.
- Tipo 2: $z,x,y$.

# Cambio de coordenadas en integrales dobles y triples
En una variable:
$$
\int_{a}^b f(x)dx=\int_{c}^df(u)u'du
$$
### Transformación coordenadas polares
$$
\begin{cases}
x=r\cos \theta \\
y=r\sin \theta
\end{cases}
$$
Al aplicar el teorema queda:
$$
\iint_{D}f(x,y)=xdx
$$
Teorema de cambio de variable (no se pide demostración).

*Ejemplo:*
Calcular la siguiente integral en la región que se indicada (parte superior de una circunferencia entre $-1$ y $1$):
$$
\int_{D}(x^2+y^2)dxdy
$$
Entonces, en base al la fórmula de la parte superior de una circunferencia $y=\sqrt{ 1-x^2 }$
$$
\begin{gather}
\int_{-1}^1dx \int_{x}^{\sqrt{ 1-x^2 }}(x^2+y^2)dy
\end{gather}
$$
Al ser complicado se utilizan coordenadas polares,
$$
\begin{align}
\iint_{D}(x^2+y^2)dxdy&=\iint_{D^\star}(r^2\cos^2\theta+r^2\sin^2\theta)r dr d\theta \\
&=\iint_{D^\star}r^3 dr d\theta \\
&=\int_{0}^\pi \int_{0}^1 r^3 dr d\theta \\
&=\int_{0}^\pi \left[ \frac{r^4}{4} \right]_{0}^1d\theta \\
&=\int_{0}^\pi \frac{1}{4}d\theta=\frac{1}{4}[\theta]_{0}^\pi=\frac{\pi}{4}
\end{align}
$$

*Ejemplo 2:*
Calcular el área del círculo unitario:
$$
A=\iint_{D}dxdy=\int_{-1}^1dx \int_{-\sqrt{ 1-x^2 }}^{\sqrt{ 1-x^2 }}dy
$$
Utilizando coordenadas polares:
$$
\begin{align}
A=\iint_{D^\star}r dr d\theta &=\int_{0}^{2\pi}\int_{0}^1 r dr d\theta \\
&=\int_{0}^{2\pi} \left[ \frac{r^2}{2} \right]_{0}^1 d\theta \\
&=\int_{0}^{2\pi} \frac{1}{2} d\theta=\pi
\end{align}
$$
*Ejemplo 3 (coordenadas cilindricas):*
Calcular el volumen de la región de $\mathbb{R}^3$, indicada en la figura
$$
\begin{gather}
z=4-r^2 \\
z=r
\end{gather}
$$
Entonces,
$$
\begin{gather}
4-r^2=r \\
r^2+r-4=0 \begin{cases}
r_{1}=1 \\
r_{2}=-2
\end{cases} \\
0\leqslant r\leqslant 1, \ \ 0\leqslant\theta\leqslant 2\pi
\end{gather}
$$
