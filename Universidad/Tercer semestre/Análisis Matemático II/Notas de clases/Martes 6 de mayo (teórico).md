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

\end{align}
$$