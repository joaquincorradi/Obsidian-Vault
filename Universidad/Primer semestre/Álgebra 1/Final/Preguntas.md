1. Deducir la ecuación vectorial de una recta definida por $2$ puntos y dar al menos $3$ representaciones algebraicas equivalentes de la misma:
	Si una recta está definida por dos puntos
$$P_1=(x_1,y_1,z_1),\qquad P_2=(x_2,y_2,z_2),$$
	primero se calcula un vector director como la diferencia de los puntos:
$$\vec v=\overrightarrow{P_1P_2}=(x_2-x_1,;y_2-y_1,;z_2-z_1).$$

	Esto tiene sentido porque el vector que va de $(P_1)$ a $(P_2)$ indica la dirección de la recta.
	Entonces, una ecuación vectorial de la recta es
$$\boxed{\vec r=\vec a+t\vec v,\qquad t\in\mathbb R}$$
	donde $\vec r_1=(x_1,y_1,z_1)$ es el vector posición de $P_1$ y $\vec v$ es el vector director.
	Desarrollando coordenada a coordenada, se obtiene la forma paramétrica:
$$\boxed{
\begin{cases}
x=x_1+t(x_2-x_1)\\
y=y_1+t(y_2-y_1)\\
z=z_1+t(z_2-z_1)
\end{cases}}$$
	Si las componentes del vector director son no nulas, se puede escribir la forma continua o simétrica:
$$\boxed{
\frac{x-x_1}{x_2-x_1}=
\frac{y-y_1}{y_2-y_1}=
\frac{z-z_1}{z_2-z_1}}$$
	Finalmente, en $\mathbb R^3$ también puede darse la forma implícita como intersección de dos planos, eliminando el parámetro $t$. Si se llama $\vec{v}=(v_{x}, v_{y}, v_{z})$, una forma implícita posible es
$$\boxed{
\begin{cases}
A(x-x_1)-B(y-y_1)=0\\
C(x-x_1)-A(z-z_1)=0
\end{cases}}$$
	En resumen, a partir de dos puntos de una recta se puede dar, al menos, estas representaciones equivalentes:

-  **Vectorial:** $\vec r=\vec r_1+t\vec v$
- **Paramétrica:** sistema en $(x,y,z)$
- **Simétrica:** igualdad de fracciones
- **Implícita:** intersección de dos planos

---

2. Realizar un gráfico representando los elementos involucrados en la ecuación vectorial de la recta.

![[ecuacion_vectorial.png|352]]

---

3. ¿Cómo se relaciona la pendiente de una recta con el ángulo que forma con el eje x?
	La relación es
	$$\boxed{m=\tan(\alpha)}$$
	donde
	- $m$: es la pendiente de la recta.
	- $\alpha$: es el ángulo que forma la recta con el semieje positivo $x$, medido en sentido antihorario.
	También se puede escribir
	$$\alpha=\arctan(m)$$

---

4. Dadas las ecuaciones explícitas de dos rectas en en plano: $y_{1}=a_{1}x+b_{1}$ y $y_{2}=a_{2}x+b_{2}$, ¿Qué condiciones deben cumplirse para que las dos rectas: se intersequen; sean paralelas; sean coincidentes?
	- **Se intersecan:** se cortan en un único punto si y solo si tienen pendientes distintas:
	$$\boxed{a_{1}\neq a_{2}}$$
	Porque al igualarlas,
	$$a_{1}x+b_{1}=a_{2}x+b_{2}$$
	queda una ecuación con una sola solución para $x$ cuando $a_{1}\neq a_{2}$.
	- Son paralelas

---

5. 